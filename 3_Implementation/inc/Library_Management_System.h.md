/\*\*

` `\* @file Library\_Managment\_System.h

` `\* @author Swaykutty28 (swathi.thulasi@ltts.com)

` `\* @brief 

` `\* @version 0.1

` `\* @date 2021-07-11

` `\* 

` `\* @copyright Copyright (c) 2021

` `\* 

` `\*/

#ifndef \_\_LIBRARY\_MANAGEMENT\_SYSTEM\_H\_\_

#define \_\_LIBRARY\_MANAGEMENT\_SYSTEM\_H\_\_

#include<stdio.h>

#include<stdlib.h>

#include<string.h>


/\*\*

` `\* @brief structure for Book Record

` `\* 

` `\*/

typedef struct library

{

`    `int book\_id;

`    `char book\_name[20];

`    `char author\_name[20];

}book;

/\*\*

` `\* @brief return type for funtions for unit testing

` `\* 

` `\*/

typedef enum test\_values {

`    `pass = 1,

`    `fail = 0

}test\_values;

/\*\*

` `\* @brief function to find a book by its ID

` `\* @param id 

` `\* @return test\_values 

` `\*/

test\_values searchbook(int id);

/\*\*

` `\* @brief function to add new books to the library

` `\* 

` `\* @return test\_values 

` `\*/

test\_values addition(int id,char name[],char author[]);

/\*\*

` `\* @brief funtion to denote discarded books

` `\* 

` `\* @param id 

` `\* @return test\_values 

` `\*/

test\_values deletebook(int id);

/\*\*

` `\* @brief function to view all the books

` `\* 

` `\* @return test\_values 

` `\*/

test\_values issuebook(int id);

/\*\*

` `\* @brief function to issue the books

` `\* 

` `\* @return test\_values 

` `\*/

test\_values viewbook(void);

#endif
