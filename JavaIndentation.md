### [HOME](https://krishna-waidande-dev.github.io/krishna-waidande.github.io/)

# Rules for Indentation in a code

### Variable Name

+ The variable names should be valid to the point.

```  
String name 		(It is valid attribute name for the class Company)
String companyname 	(It is invalid attribute name for the class Company)
```
In above example, we are creating a class for Company so it is obvious that the name variable defined in the scope of the Company class contains the name of the company.

+ The variable names should be in Camel-Case :

```
int errorCode 				is valid. 
int errorcode,ErrorCode,Errorcode 	are invalid.
```

### Class Name

+ The class name should follow “JAVA naming conventions”. For every subsequent word in the class name the first character should be an upper-case.

```java
public class CompanyDetail {
/*
Class body
*/
}
```

+ The class name should be same as your file name.

### Method Name 

+ The method names should be relevant to the scenario and should be written in Camel-Case.


```java
void createCompany() { //valid name	
/* method body */
}	

void CreateCompany() { //invalid name	
/* method body */
}     
```


### Import statements

+ It is good practice to add setting in IDE to alphabetically sort the importing statements.


+ Import statements for same package names should be one after another on next lines without an interrupting blank space. 	


> Valid:

```java
import com.krishagni.CRM.rest.Company;
import com.krishagni.CRM.rest.Factory;
import com.krishagni.CRM.rest.Dao.CompanyDao;
```

> Invalid :

```java
import com.krishagni.CRM.rest.Company;

import com.krishagni.CRM.rest.Factory;
import com.krishagni.CRM.rest.Dao.CompanyDao;
```

### Curly braces


+ The curly braces used in any class, method, loops and statements should be in proper format for enhancing the readability of the code.


> Good practice
```
public String getName() {
return name;
}
```


### Alignment 

+ The code must be aligned in the proper way keeping 4 spaces before any method or variables.


> Sample code with proper alignment

```java 	
public class Company {
    CompanyDao dao;
    Company comp = new Company();    
    
    public Factory getAddcomp() {
	        return addcomp;
    }
}
```

There should be proper spacing before and after an operator.


> Like :
int name = 10; 


> Unlike:
int name=10;


### Remove unwanted spaces 

Spaces which are not needed should not be used, the code should be kept in compact size and in readable format.


### Line Length :

Maximum characters in a line should not be more than 120.


### XML and HTML indentation


+ Before every tag two spaces need to be given to make it in standard format.


> Like :

```xml
<bean id = "dao" class = "com.krishagni.CRM.rest.Dao.CompanyDaoImpl">
  <property name = "sessionFactory" ref = "sessionFactory"> </property>
</bean>
```

> Unlike :

```xml
<bean id = "dao" class = "com.krishagni.CRM.rest.Dao.CompanyDaoImpl">
   	 <property name="sessionFactory" ref = "sessionFactory"></property>
</bean>
```
