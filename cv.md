# **Andrey Kozyrin**

## About myself
Hello, my name is ***Andrew***. I work in LLC "IT-Plus" this is a Russian electricity generation company part of the Renova Group. My position Application Developer, i work in this title last 3 years. In my responsibility include backend develop, desktop application, write scripts, program support.
### Personal qualities:
* Learns Quickly
* Resilient
* Willing
* Logical
* Thorough
* Self-Motivated

## Skills  

### Programming languages and frameworks:
* C, C++
    * Qt 5
* Python
    * PyQt5
* Java
    * (learning Spring)
* Lua
* PHP  

### Databases:
* SQL
    * MySQL
    * PostgreSQL
    * MSSQL  

### Tools:
* SDK Man
* Git
* Postman
* Maven
* pip  

### IDE:
* IntelliJ
    * IDEA
    * PHPStorm
    * PyCharm
* Qt Creator
* ZeroBrane Studio  

## Code examples:
### Java:
You can see my little education project where i learn how work IOC programming principle, pattern di, di-container:

**[IOC-DI](https://github.com/AndrewKozyrin/ioc-di)**

I participate in a training project:

**[Java-education-base](https://github.com/jegius/java-education-base)**

### Python:  
I have private projects on Github use Python 3.6  
A small piece of project "Connect to OPC", this code create config file to connect to database:
````
    def create_config_database(self, cfg_name: str, source_name: str, message: QMessageBox):
        try:
            encode_password = base64.b64encode(self.ui.lineEdit_password.text().encode('utf-8'))

            cfg_data = {
                'database_index': self.ui.comboBox_select_server.currentIndex(),
                'host': self.ui.lineEdit_adress.text(),
                'port': self.ui.lineEdit_port.text(),
                'username': self.ui.lineEdit_user.text(),
                'password': str(encode_password, 'utf-8'),
                'database': self.ui.lineEdit_base.text(),
                'opc_server_name': '',
                'used_tag': self.used_tag,
            }
            with io.open(cfg_name, 'w', encoding='utf-8') as cfg_file:
                json.dump(cfg_data, cfg_file, indent=2, ensure_ascii=False)
            # Если ошибок нет записываем изменения в main_config
            save_data_to_main_config_json(source_name, cfg_name, message)
        except:
            message.setWindowTitle('Конфигурационный файл ' + cfg_name)
            message.setIcon(QMessageBox.Critical)
            message.setText('Невозможно создать конфигурационный файл базы данных')
            message.exec_()
````

### C++(Qt5):  
I have private projects on Github.  
A small piece of project "Monitor", this code find table name use OPC tag:
````
QString LastValue::findTableName(QString tag)
{
    QString tableName;
    tableName.clear();
    if(!query.exec("confidential information")){
        messageBox.critical(this,"Ошибка",query.lastError().text());
    }
    while(query.next()){
        tableName = query.value(0).toString();
    }
    query.clear();
    return tableName;
}
````  

## Work experience  

Data | Organization | Position
---- | -------------| --------|
04.20.2011 - 08.18.2011 | Togliatti State University (research department) | Laboratory assistant 
04.23.2012 - 12.10.2012 | Volga Region State University of Service | System Administrator
10.01.2012 - 08.01.2016 | LLC "Detail Resource" | System Administrator, Web Developer, Application Developer
09.01.2016 - 04.01.2018 | "Pro guild" | Full Stack Developer ([Victory](https://xn---63-5cdesg4ei.xn--p1ai))
04.04.2018 - 03.01.2021 | PJSC "T-Plus" | Application Developer
03.01.2021 - till now | LLC "IT-Plus" | Application Developer

## Education

Date | University (Course) | Specialization
---- | ------------------- | --------------
2006-2011 | Volga Region State University of Service | Electronic engineer
2011-2014 | Volga Region State University of Service Graduate school | Electromechanics and electrical apparatus
2016-2017 | Learning Center "Netcracker" | Software Developer
2018 | Learning Center LLC "SMS-Automatization" | SIEMENS Simatic, SIEMENS WinCC
2019 | Learning Center "ProSoft Technology Inc" | PLC Regul

## Language

English - A2 [Anglomir](https://anglomirtlt.ru/online)  
I have language practice withe few american friends lives in New-York and Georgia state.

## Contacts  
Phone: +79276596236  
E-mail: kozyrin.ai@gmail.com

