# Data Importation

## [Data table](https://material.io/components/data-tables): 
Data tables display sets of data across rows and columns. They organize information in a way that’s easy to scan so that users can look for patterns and develop insights from data.

## Data types

### [Categorical](https://towardsdatascience.com/what-are-categorical-variables-and-how-to-encode-them-6e77ddc263b3):
They are variables in the data set that unlike continuous variables take a finite set of values. For example, grades that students are given by a teacher for assignments (A, B, C, D, E, and F). In the dataset, categorical variables are often strings. 

### [Numerical](https://study.com/academy/lesson/data-types-in-programming-numbers-strings-and-others.html):
An **integer** is a numeric value without a decimal. Integers are whole numbers and can be positive or negative (1, -7).
A number with a decimal is referred to as a decimal, a **float** or a **double** (13.5, 20.03). The term 'float' comes from floating point, which means you can control where the decimal point is located. The term 'double' refers to using double the amount of storage relative to a float.

### [Boolean](https://techterms.com/definition/boolean): 
Boolean, or boolean logic, is a subset of algebra used for creating true/false statements. Boolean expressions use the operators AND, OR, XOR, and NOT to compare values and return a true or false result.

### [Dates](https://docs.microsoft.com/en-us/dotnet/visual-basic/language-reference/data-types/date-data-type#example):
Holds IEEE 64-bit (8-byte) values that represent dates ranging from January 1 of the year 0001 through December 31 of the year 9999, and times from 12:00:00 AM (midnight) through 11:59:59.9999999 PM. Each increment represents 100 nanoseconds of elapsed time since the beginning of January 1 of the year 1 in the Gregorian calendar. The maximum value represents 100 nanoseconds before the beginning of January 1 of the year 10000.

### [Strings](https://techterms.com/definition/string):
It is used to represent text rather than numbers. It is comprised of a set of characters that can also contain spaces and numbers. For example, the word "apple" and the phrase "I ate 3 apples" are both strings. 

## Data formats

### [csv](https://www.reviversoft.com/es/file-extensions/csv):
El contenido almacenado en el formato CSV se refieren a archivos de datos adjuntos con el .csv extensión, y estos archivos CSV también se llaman valores separados por comas archivos. El "CSV" en un archivo de puesta con el .csv extensión significa "valores separados por comas" debido a que los datos de estos archivos CSV son detalles dividido por comas en conjuntos particulares de información.
#### Example:
![Example](https://d117h1jjiq768j.cloudfront.net/images/default-source/default-album/csv-sample-file.gif?sfvrsn=cdb6772e_1)
### [json](https://www.json.org/json-en.html):
JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. JSON is built on two structures:

* A collection of name/value pairs. In various languages, this is realized as an object, record, struct, dictionary, hash table, keyed list, or associative array.
* An ordered list of values. In most languages, this is realized as an array, vector, list, or sequence.
#### Example:
![Example](https://static.goanywhere.com/images/tutorials/read-json/ExampleJSON2.png)

### [xml](https://fileinfo.com/extension/xml#:~:text=An%20XML%20file%20is%20an,open%20in%20Microsoft%20XML%20Notepad):
The XML format stores data in a structure that is machine-readable and human-readable. There are a large amount of programs that can open XML files. And since they are formatted as text documents, they can be viewed and edited by basic text editors.

XML files have become a standard way of storing and transferring data between programs and over the Internet. However, they can be used by many other types of programs. The XML syntax has been utilized in a large variety of file formats, such as Microsoft Office Open XML, LibreOffice OpenDocument, .XHTML, and .SVG.
#### Example:
![Example](https://www.mssqltips.com/tipimages2/2899_img5.jpg)
### xls:
An XLS file is a spreadsheet file created by Microsoft Excel or another spreadsheet program, such as OpenOffice Calc or Apple Numbers. It contains one or more worksheets, which store and display data in a table format. XLS files may also store mathematical functions, charts, styles, and formatting.
#### Example:
![Example](https://m6n6j6i4.stackpathcdn.com/wp-content/uploads/2018/01/Importing-an-XLS-or-XLSX-into-Microsoft-Project-Fig-1.jpg)

## Difference between local and remote repositories

### url:
A remote URL is Git's fancy way of saying "the place where your code is stored." That URL could be your repository on GitHub, or another user's fork, or even on a completely different server.

You can only push to two types of URL addresses:

An HTTPS URL like https://github.com/user/repo.git
An SSH URL, like git@github.com:user/repo.git

Git associates a remote URL with a name, and your default remote is usually called origin.

### apis: 
To interact with any defined repository, use the default repository APIs that are included in Pega Platform. Other methods of interacting with files, such as using custom java, are not supported.

For example, you can delete or retrieve a file in a repository. You can also add a new custom repository type so that your application can manage files in a remote file storage repository using the same API that you use for your default repository types. 

## Secure data transfer protocols
### [File Transfer Protocol (FTP)](https://www.sftpplus.com/articles/2018/sftpplus-best-protocols.html)
Shortform for File Transfer Protocol, the objectives of FTP are: 
1) to promote sharing of files (computer programs and/or data).

2) to encourage indirect or implicit (via programs) use of remote computers.
3) to shield a user from variations in file storage systems among hosts.
4) to transfer data reliably and efficiently.

### [Hypertext Transfer Protocol (HTTP)](https://www.sftpplus.com/articles/2018/sftpplus-best-protocols.html)
HTTP, shortform for Hypertext Transfer Protocol, is an application-level protocol for distributed, collaborative, hypermedia information systems. It is a generic, stateless, protocol which can be used for many tasks.

HTTP, in use by the World-Wide Web global initiative since 1990, is a protocol used in many tasks related to common usage of the web such as browsing websites. This is relevant to SFTPPlus since we offer a browser-based file management utility.

Without SSL/TLS, there is no way to encrypt data in transit. Other downsides to HTTP, in the context of SFTPPlus, include:

1) Packet capture through the use of packet capture tools.
2) Man-in-the-middle attack where the attacker intercepts and relays false malicious content between two parties.
3) Credentials are sent in a plain text encoding when using the SFTPPlus HTTP Basic Auth API.

## [Procedures for data importing](https://v8doc.sas.com/sashtml/accpc/z1227915.htm)
As in the Import/Export facility, the IMPORT and EXPORT procedures transfer data between SAS and external data sources. These external data sources can include DBMS tables, PC files, spreadsheets, and delimited external files, which are files containing columns of data values that are separated by a delimiter such as a blank or a comma.
``` 
DATAFILE=<"filename" | TABLE="tablename">
OUT=<libref.> SAS-data-set
<DBMS=identifier> <REPLACE>;
<data-source-statements;>

``` 