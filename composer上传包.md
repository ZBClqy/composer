## 构建composer包

### 一、建立composer.json文件

{
    "name": "xlsx/array", //包的名称
    "description": "xlsx/array - Read, Create and Write Spreadsheet documents in PHP - Spreadsheet engine",//包的讲解
    "keywords": [//该包相关的关键词的数组
        "PHP",
        "OpenXML",
        "Excel",
        "xlsx",
        "xls",
        "ods",
        "gnumeric",
        "spreadsheet"
    ],
    "homepage": "https://github.com/ZBClqy/xlsx-array",//github地址
    "type": "library",//library: 这是默认类型，它会简单的将文件复制到 vendor 目录
    "license": "MIT",//包的许可协议
    "authors": [
        {
            "name": "zbc"//作者名称
        }
    ],
    "require": {//包的引用依赖和php版本
        "php": "^7.4 || ^8.0",
        "ext-ctype": "*",
        "ext-dom": "*",
        "ext-fileinfo": "*",
        "ext-gd": "*",
        "ext-iconv": "*",
        "ext-libxml": "*",
        "ext-mbstring": "*",
        "ext-simplexml": "*",
        "ext-xml": "*",
        "ext-xmlreader": "*",
        "ext-xmlwriter": "*",
        "ext-zip": "*",
        "ext-zlib": "*",
        "ezyang/htmlpurifier": "^4.15",
        "maennchen/zipstream-php": "^2.1 || ^3.0",
        "markbaker/complex": "^3.0",
        "markbaker/matrix": "^3.0",
        "psr/http-client": "^1.0",
        "psr/http-factory": "^1.0",
        "psr/simple-cache": "^1.0 || ^2.0 || ^3.0"
    },
    "minimum-stability":"dev",//来筛选require包的稳定性
    "autoload": {//自动加载命名空间的配置，和指定根目录（命名空间的根路径）
        "psr-4": {
            "PhpOffice\\PhpSpreadsheet\\": "src/PhpSpreadsheet"
        }
    }
}

二、然后上传到github，这里记得要上传tag

git tag v3.0

git push -tag