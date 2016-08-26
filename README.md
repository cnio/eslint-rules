# Eslint-rules
Between Google and Nodejs code style and some changes for company.
### Possible Errors
```js
'comma-dangle': [2, 'never'], // 去掉非必要逗号 比如[1,2,]
'no-constant-condition': 2, // 不使用常量判断条件
'no-control-regex': 2, // ASCII在0-31范围内的字符不用于正则表达式
'no-debugger': 2, // 不使用debugger
'no-dupe-args': 2, // 参数不能相同 比如fn(a, b, a)
'no-dupe-keys': 2, // key不能重复
'no-duplicate-case': 2, // case 不能重复
'no-empty-character-class': 2, // 在正则中不添加空字符条件
'no-ex-assign': 2, // 不允许对exception重新赋值
'no-extra-boolean-cast': 2, // 没必要转换成布尔类型
'no-extra-semi': 2, // 去掉不必要的分号
'no-func-assign': 2, // 重新对function赋值
'no-inner-declarations': 2, // function不能在内部声明
'no-invalid-regexp': 2,// 无效正则
'no-irregular-whitespace': 2, // 空格和制表符不能混用
'no-negated-in-lhs': 2, // replaced with `no-unsafe-negation` // 不安全的逻辑
'no-regex-spaces': 2, // 正则中间不加空格
'no-sparse-arrays': 2, // 稀疏数组 [,]
'no-unreachable': 2, // 逻辑是否执行 比如console一定要在return前执行
'use-isnan': 2, // 使用isNaN
'valid-typeof': 2, // 有效的typeof
'no-unexpected-multiline': 2, // 多行注意加分号
```
### Best Practices
```js
'no-fallthrough': 2,
'no-multi-spaces': 2,
'no-octal': 2,
'no-redeclare': 2,
'no-self-assign': 2,
'no-unused-labels': 2,
```
### Variables
```js
'no-shadow-restricted-names': 2, // 禁止使用关键字
'no-undef-init': 2, // 不允许初始化为undefined
'no-undef': [2, {typeof: true}], // 使用非全局声明的变量
'no-unused-vars': 2,
'no-use-before-define': [2, 'nofunc'],
```
### Node.js
```js
'handle-callback-err': 1, // 回调err可以不handle
'no-new-require': 2, // 不允许使用 new require('foo'); 这种形式
'no-path-concat': 2, // 使用path.join 或path.resolve 来操作路径,使其对不同平台进行兼容
```
### Stylistic Issues
```js
'array-bracket-spacing': [2, 'never'], // 数组括号空格
'brace-style': [2, '1tbs', {allowSingleLine: false}], // 大括号是否另起一行
'camelcase': [2, {properties: 'always'}], // 驼峰命名
'comma-spacing': [2, {before: false, after: true}], // 逗号空
'comma-style': [2, 'last'], // 逗号始终保持在每一行代码的末尾
'computed-property-spacing': [2, 'never'], // 获取对象属性时的空格写法
'eol-last': 2, // 空行
'indent': [2, 4, {SwitchCase: 1}],  // 缩进
'key-spacing': [2, {beforeColon: false, afterColon: true}], // key后面要加空格
'keyword-spacing': 2, // 关键字后加空格
'max-nested-callbacks': [1, 4], // 最大嵌套回调数
'max-statements-per-line': 2, // 每行最大声明数
'new-cap': [2, {newIsCap: true, capIsNew: true}], // 使用new时,类名需大写
'new-parens': 2, // 使用new时,类名需加括弧
'no-array-constructor': 2, // 不使用new Array()来创建数组,但可以用来指定创建的数组长度
'no-lonely-if': 2, // 不独立使用if关键字if()
'no-mixed-spaces-and-tabs': 2, // 混用空格和制表符
'no-multiple-empty-lines': [2, {max: 1}], // 多行空行
'no-negated-condition': 2, // 使用肯定判断条件
'no-new-object': 2, // 禁用 new Object() {}
'no-restricted-syntax': [2, 'WithStatement'], // 禁用with关键字
'no-whitespace-before-property': 2, // 禁用属性前使用空格
'no-spaced-func': 2, // replaced by 'func-call-spacing' 函数调用时括号需紧挨着函数名
'no-trailing-spaces': 2, // 每行末尾不许添加空白
'no-unneeded-ternary': 2, // 不使用没必要的三元表达式
'object-curly-spacing': [2, 'never'], // 对象中使用的花括号需去掉没必要的空格
'one-var': [2, 'never'], // 每个变量需用单独的var声明
'one-var-declaration-per-line': 2, // 每行最多只能有一个变量赋值
'operator-assignment': [2, 'always'], // 操作符写法  x += y 别写成 x = x + y
'operator-linebreak': [2, 'after'],
'padded-blocks': [2, 'never'], // 禁用填充
'quote-props': [2, 'consistent-as-needed'], // 需要时可加引号
'semi-spacing': [2, {before: false, after: true}], // 分号后面需加空格
'semi': [2, 'always'], // 分号
'space-before-blocks': [2, 'always'], // function foo()空格{}
'space-before-function-paren': [2, {anonymous: 'never', named: 'never'}],
'space-in-parens': [2, 'never'], // 括号中间不需要添加空格 ( 'foo' ) is wrong, should be ('foo')
'space-infix-ops': 2, // var sum = 1 + 2; 中间需要加入空格
'space-unary-ops': 2,// 一元操作符格式
'spaced-comment': [2, 'always', {markers: ['!']}] // 注释'//'前需加空格
```
