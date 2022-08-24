## <script  报错   Parsing error: '>' expected

原因：eslintrc.json 配置错误
```json
{
    // old config
    "parser": "@typescript-eslint/parser",
    "parserOptions": {   
        "ecmaVersion": "latest",
        "sourceType": "module"
    },
    
    // new config
    "parser": "vue-eslint-parser",
    "parserOptions": {
        "parser": "@typescript-eslint/parser",
        "ecmaVersion": "latest",
        "sourceType": "module"
    },
}

```