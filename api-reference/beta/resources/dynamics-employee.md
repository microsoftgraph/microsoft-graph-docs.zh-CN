---
title: employees 资源类型
description: Dynamics 365 Business Central 中的员工对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: eceea9e1811b61045c03fb8dc5d7710f33158ccc
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695971"
---
# <a name="employees-resource-type"></a>employees 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的员工。

## <a name="methods"></a>方法

| 方法                                              | 返回类型|说明               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[获取员工](../api/dynamics-employee-get.md)      |employees  |获取 employee 对象。   |
|[发布员工](../api/dynamics-create-employee.md)  |employees  |创建 employee 对象。|
|[修补员工](../api/dynamics-employee-update.md) |employees  |更新 employee 对象。|
|[删除员工](../api/dynamics-employee-delete.md)|无       |删除 employee 对象。|

## <a name="properties"></a>属性
| 属性           | 类型   |说明                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |GUID    |员工 ID。 不可编辑。                         |
|number              |string  |员工编号。 只读。                        |
|displayName         |string  |雇员 givenName + surname。 只读。           |
|givenName           |string  |雇员的给定名称。                        |
|middleName          |string  |员工的中间名。                       |
|surname             |string  |员工的姓氏                            |
|jobTitle            |string  |员工职务                          |
|address             |[导航。PostalAddress](../resources/dynamics-complextypes.md)|指定员工的地址。 此地址将显示在员工的所有资源文档上。|
|phoneNumber         |string  |指定员工的电话号码。             |
|mobilePhone         |string  |指定员工的移动电话号码。      |
|email               |string  |指定员工的电子邮件地址。                |
|personalEmail       |string  |指定员工的个人电子邮件地址。       |
|employmentDate      |date    |指定员工开始为公司工作的日期。|
|terminationDate     |date    |例如，指定员工因停用或离职而终止的日期。|
|状态              |string  |指定员工的状态。 可能的值是 Active、Inactive 或 Terminated|
|birthDate           |date    |指定员工出生日期。                |
|picture             |stream  |员工图片。 只读。                       |
|lastModifiedDateTime|datetime|上次修改员工的日期/时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```



