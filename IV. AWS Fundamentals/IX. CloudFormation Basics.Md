## Cloud Formation
- CloudFormation is an Infrastructure as Code (IaC) product in AWS which allows automation infrastructure creation, update and deletion.
- Templates created in YAML or JSON can be used to automate infrastructure operations
- Templates are used to create stacks, which are used to interact with resources in an AWS account.
![img_1.png](Images/img_1.png)
- All Template has a list of **resources**(only **mandatory** part of template) , resources section tells the cloud formation what needs to be done(out of CRUD operations).
- **Description** - non mandatory, however if used must follow the AWSTemplateFormatVersion
![img_2.png](Images/img_2.png)
- **Metadata** - Controls the UI
![img_3.png](Images/img_3.png)
- **Parameters** - Options provided from the UI
![img_4.png](Images/img_4.png)
- **Mappings** - Allows to create lookup table
![img_5.png](Images/img_5.png)
- **Conditions** - Used to create conditions , below creates EC2 instance only when CreateProdResources is true
![img_6.png](Images/img_6.png)
![img_7.png](Images/img_7.png)
![img_8.png](Images/img_8.png)
![img_9.png](Images/img_9.png)
- **Outputs** - 
![img_10.png](Images/img_10.png)

### Template to create EC2 instance :
![img_11.png](Images/img_11.png)
![img_12.png](Images/img_12.png)
![img_13.png](Images/img_13.png)

### YAML
- ***YAML*** is one of the languages, that Cloud uses as a template.
    - human readable 
    - define data 
    - configuration 
    - Key:Value pair 
      - supports:
        - string, integer, boolean, float, null 
    - Lists cats : ["a","b","c"] 
      - or cats:
        - "a"
        - "b"
        - "c"
    - dictionary 
      - turtle:
         - name: "Pixel"
         - color: ["green", "grey"]
         - name: "Sid"
         - color: ["black", "green"]
    - indentation matters

![img_14.png](Images/img_14.png)
![img_15.png](Images/img_15.png)

### JSON
- JavaScript Json Notation (JSON) -used broadly
- used for data-interchange format
- easy for humans to read and write
- easy for machines to parse and generate
- does not care about indentation -has brackets
- JSON object is an unordered set of key:value pairs enclosed by curly brackets {} -dictionary
- JSON array is an ordered collection of values, separated by commas and enclosed in square brackets [] -list
- Values can be: string, object, integer, array, boolean, null
![img_16.png](Images/img_16.png)
![img_17.png](Images/img_17.png)
![img_18.png](Images/img_18.png)
![img_19.png](Images/img_19.png)