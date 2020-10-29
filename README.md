
# Generamba Templates

### Install
1. To generate templates, you need to install Generamba:
    ```sh
    gem install generamba
    ```

2. Run generamba setup in the project root folder. This command helps to create Rambafile that define all configuration needed to generate code. You can modify this file directly in future.
    ```sh   
    generamba setup
    ```

3. Next step, installing templates. 
Replace all templates created in .rambafile with the following. 
    
    ```### Templates
    catalogs:
    - 'https://github.com/Harseko/Generamba_Templates'
    templates:
    - {name: swift_mvvm}
    ```
    And run install

    ```sh   
    generamba template install
    ```
### Usage

Run `generamba gen [MODULE_NAME] [TEMPLATE_NAME] --module_path '[MODULE_PATH]'` - It creates module with specific name from specific template.

To generate template module use:
```sh
generamba gen [MODULE_NAME] [TEMPLATE_NAME] --module_path '[MODULE_PATH]'
```

For Example: 
```sh
generamba gen Login swift_mvvm --module_path 'Modules/Auth'
```
