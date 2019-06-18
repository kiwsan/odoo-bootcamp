[![Build Status](http://runbot.odoo.com/runbot/badge/flat/1/11.0.svg)](http://runbot.odoo.com/runbot)
[![Tech Doc](http://img.shields.io/badge/11.0-docs-875A7B.svg?style=flat&colorA=8F8F8F)](http://www.odoo.com/documentation/11.0)
[![Help](http://img.shields.io/badge/11.0-help-875A7B.svg?style=flat&colorA=8F8F8F)](https://www.odoo.com/forum/help-1)
[![Nightly Builds](http://img.shields.io/badge/11.0-nightly-875A7B.svg?style=flat&colorA=8F8F8F)](http://nightly.odoo.com/)

Odoo
----

Odoo is a suite of web based open source business apps.

The main Odoo Apps include an <a href="https://www.odoo.com/page/crm">Open Source CRM</a>,
<a href="https://www.odoo.com/page/website-builder">Website Builder</a>,
<a href="https://www.odoo.com/page/e-commerce">eCommerce</a>,
<a href="https://www.odoo.com/page/warehouse">Warehouse Management</a>,
<a href="https://www.odoo.com/page/project-management">Project Management</a>,
<a href="https://www.odoo.com/page/accounting">Billing &amp; Accounting</a>,
<a href="https://www.odoo.com/page/point-of-sale">Point of Sale</a>,
<a href="https://www.odoo.com/page/employees">Human Resources</a>,
<a href="https://www.odoo.com/page/lead-automation">Marketing</a>,
<a href="https://www.odoo.com/page/manufacturing">Manufacturing</a>,
<a href="https://www.odoo.com/page/purchase">Purchase Management</a>,
<a href="https://www.odoo.com/#apps">...</a>

Odoo Apps can be used as stand-alone applications, but they also integrate seamlessly so you get
a full-featured <a href="https://www.odoo.com">Open Source ERP</a> when you install several Apps.

Getting started with Odoo
-------------------------
For a standard installation please follow the <a href="https://www.odoo.com/documentation/11.0/setup/install.html">Setup instructions</a>
from the documentation.

Then follow <a href="https://www.odoo.com/documentation/11.0/tutorials.html">the developer tutorials</a>

##  Quick start

1.  **Create a new superuser in postgresSql on Docker container.**

    ```sh
    $ docker exec -it <container-name> psql -U <username> -W <database-name> psql
    ```    
    - -U project -W project The command to execute to the running container
    - U user
    - W password
    - project the database you want to connect to.

    ```sh
    $ CREATE USER <username> WITH SUPERUSER PASSWORD '<password>';
    ```

    These are specified by you here
    
    ```sh
    environment:
        POSTGRES_DB: <database-name>
        POSTGRES_USER: <username>
        POSTGRES_PASSWORD: <password>
    ```
    
1.  **Configure Pycharm for Odoo**

    ![Pycharm](pycharm-setting.png)
    
1.  **Configure Eclipse for Odoo**

    ![Pycharm](eclipse-setting1.png)
    
    ![Pycharm](eclipse-setting2.png)
    
    ![Pycharm](eclipse-setting3.png)
    