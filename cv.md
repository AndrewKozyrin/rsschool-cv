# **Andrey Kozyrin**

## About myself
Hello, my name is ***Andrew***. I work in LLC "IT-Plus" this is a Russian electricity generation company part of the Renova Group. My position Application Developer, i work in this title last 5 years. In my responsibility include backend develop, desktop application, write scripts, program support.
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

Create many project use Python 3.6  
A small piece of project "Connect to OPC", this code create config file to database
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
A small piece of project "Monitor", this code find table name use OPC tag.
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

## Contacts
____
Phone: +79276596236  
E-mail: kozyrin.ai@gmail.com

