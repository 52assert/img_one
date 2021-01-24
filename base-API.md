# 基础数据接口文档

### 请求头(所有请求必须携带请求头)

|     参数名      | 参数类型 | 描述                                                         |
| :-------------: | :------: | ------------------------------------------------------------ |
| `Authorization` |  string  | 认证,value需要在前面加上`Bearer +token`(例如Bearer c693ad2d-6893-4bd8-b56e-65aaccb7f94a) |
| `Content-Type`  |  string  | application/json;charset=UTF-8                               |

### 客户录入API

> `POST`
>
> http://cloud.dowaycn.com/Gateway/BaseService/api/v1/input/customer

****

#### 1.请求参数

| 参数名         | 参数类型 | 描述       |
| -------------- | -------- | :--------- |
| `code`         | string   | 编码       |
| `name`         | string   | 名称       |
| `shortName`    | string   | 简称       |
| `abbreviation` | string   | 首字母缩写 |
| `companyClass` | string   | 公司类型   |
| `country`      | string   | 国家       |
| `city`         | string   | 城市       |
| `district`     | string   | 区         |
| `address`      | string   | 地址       |
| `areaCode`     | string   | 地区代码   |
| `tel`          | string   | 电话       |
| `fax`          | string   | 税率       |
| `postalCode`   | string   | 邮编       |
| `email`        | string   | 邮箱       |
| `remark`       | string   | 备注       |
| `salesGroup` | string    | 销售组   |
| `invoiceType` | string    | 发票类型   |
| `payType` | string    | 付款方式   |
| `paymentTerms` | string | 付款条件 |
| `taxRate` | decimal    | 税率   |
| `currencyCode` | string    | 币值   |
| `businessLicense` | string    | 营业执照   |
| `regBank` | string    | 开户行   |
| `regBankAccount` | string    | 银行账号   |
| `regAddressTel` | string    | 开户行地址   |
| `authorizationCode` | string    | 授权码   |
| `statementRule` | string    | 对账单规则(week/month)   |
| `statementTime` | string    | 对账单生成时间   |
| `customerContacts` | `array`  | `客户联系人` |

`**customerContacts**`

| 参数名 | 参数类型 | 描述 |
| ------ | -------- | ---- |
| `contacts` | string   | 联系人 |
| `department` | string   | 部门 |
| `tel` | string   | 电话 |
| `mobile` | string   | 手机号 |
| `email` | string   | 邮箱 |
| `remark` | string   | 备注 |

#### 2.响应参数

|  参数名   | 参数类型 |   描述   |
| :-------: | :------: | :------: |
|  `code`   |   int    | 200/500  |
| `content` |  object  | 响应数据 |
|   `msg`   |  string  | 响应消息 |



### 供应商录入API

`POST`

http://cloud.dowaycn.com/Gateway/BaseService/api/v1/input/supplier

#### 1.请求参数

| 参数名         | 参数类型 | 描述       |
| -------------- | -------- | ---------- |
| `code`         | string   | 编码       |
| `name`         | string   | 名称       |
| `shortName`    | string   | 简称       |
| `abbreviation` | string   | 首字母缩写 |
| `companyClass` | string   | 公司类型   |
| `country`      | string   | 国家       |
| `city`         | string   | 城市       |
| `district`     | string   | 区         |
| `address`      | string   | 地址       |
| `areaCode`     | string   | 地区代码   |
| `tel`          | string   | 电话       |
| `fax`          | string   | 税率       |
| `postalCode`   | string   | 邮编       |
| `email`        | string   | 邮箱       |
| `remark`       | string   | 备注       |
| `purchaseGroup` | string    | 采购组       |
| `payType` | string    | 付款方式   |
| `paymentTerms` | string | 付款条件 |
| `taxRate` | decimal    | 税率   |
| `currencyCode` | string    | 币值   |
| `businessLicense` | string    | 营业执照   |
| `invoiceType` | string | 发票类型 |
| `regBank` | string    | 开户行   |
| `regBankAccount` | string    | 银行账号   |
| `regAddressTel` | string    | 开户行地址   |
| `authorizationCode` | string    | 授权码   |
| `supplierContacts` | array    | 供应商联系人  |

**`supplierContacts`**

| 参数名 | 参数类型 | 描述 |
| ------ | -------- | ---- |
| `contacts` | string   | 联系人 |
| `department` | string   | 部门 |
| `tel` | string   | 电话 |
| `mobile` | string   | 手机号 |
| `email` | string   | 邮箱 |
| `remark` | string   | 备注 |

#### 2.响应参数

|  参数名   | 参数类型 |   描述   |
| :-------: | :------: | :------: |
|  `code`   |   int    | 200/500  |
| `content` |  object  | 响应数据 |
|   `msg`   |  string  | 响应消息 |