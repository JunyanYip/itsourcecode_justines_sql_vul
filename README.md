# itsourcecode_justines_sql_vul

### Some information

CVE ID: CVE-2023-34487

Vendor of Product: https://itsourcecode.com/

Affected Product: justines(https://itsourcecode.com/free-projects/php-project/hotel-management-system-project-php/) - v1.0.0

Attack Type: Remote

Vulnerability type: SQL injection

Description: itsourcecode Online Hotel Management System Project In PHP v1.0.0 is vulnerable to SQL Injection. SQL injection points exist in the login password input box. This vulnerability can be exploited through time-based blind injection.

Position: "body"

ParamKey: "log_pword"

payload: "1234'and(select*from(select+sleep(5))a/\*\*/union/\*\*/select+1)='"

### Process description

On the justines home page, enter payload in the login password field. The injection is effective.

![sql_1](https://github.com/JunyanYip/itsourcecode_justines_sql_vul/blob/main/sql_1.JPG)

Packet capture data.

![sql_2](https://github.com/JunyanYip/itsourcecode_justines_sql_vul/blob/main/sql_2.JPG)

