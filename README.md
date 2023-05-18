# sql-server-string-splitter

This repository contains a SQL Server function named dbo.Split_String that splits a string into multiple substrings based on a specified delimiter.

**Function Overview**
The dbo.Split_String function takes two parameters:

@String (nvarchar(max)): The input string that needs to be split.
@Delimiter (nchar(1)): The delimiter used to split the string.
The function returns a table with two columns:

Id (bigint): An identity column that provides a sequential ID for each split substring.
Data (nvarchar(max)): The individual substrings extracted from the input string.

**Usage**
To use the dbo.Split_String function, you need to provide the input string and the delimiter. The function will split the string into substrings at each occurrence of the delimiter and return the result as a table.

Here's an example of how to use the function:
SELECT * FROM dbo.Split_String('sqlserver,string,splitter', ',');

This will split the input string 'sqlserver,string,splitter' into three substrings: 'sqlserver', 'string', and 'splitter'. The result will be returned as a table with two columns: Id and Data.

**Compatibility**
The dbo.Split_String function is specific to SQL Server and utilizes SQL Server syntax. It may not be directly compatible with other database systems, such as Oracle or MySQL. If you need a similar function for Oracle or other databases, please refer to the appropriate documentation or consult the specific database's functions for string manipulation.

**Contributing**
Contributions to this repository are welcome. If you encounter any issues, have suggestions for improvements, or would like to add new features, please feel free to submit a pull request or open an issue.

**License**
This repository is licensed under the MIT License. You are free to use, modify, and distribute the function as per the terms of the license.

Please note that this is just a sample description, and you can customize it according to your specific requirements and additional information you want to provide about the repository.
