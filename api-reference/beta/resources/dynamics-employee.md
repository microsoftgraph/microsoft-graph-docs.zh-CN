---
title: 员工资源类型
description: Dynamics 365 Business Central 中的 employee 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366653"
---
# <a name="employees-resource-type"></a>员工资源类型
表示 Dynamics 365 Business Central 中的员工。

## <a name="methods"></a>方法

| 方法                                              | 返回类型|说明               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[获取员工](../api/dynamics-employee-get.md)      |员工  |获取一个 employee 对象。   |
|[过帐员工](../api/dynamics-create-employee.md)  |员工  |创建一个 employee 对象。|
|[修补员工](../api/dynamics-employee-update.md) |员工  |更新 employee 对象。|
|[删除员工](../api/dynamics-employee-delete.md)|无       |删除 employee 对象。|

## <a name="properties"></a>属性
| 属性           | 类型   |说明                                            |
|:-------------------|:-------|:------------------------------------------------------|
|id                  |GUID    |员工 ID。 不可编辑。                         |
|number              |string  |员工编号。 只读。                        |
|displayName         |string  |员工 givenName + 姓。 只读。           |
|givenName           |string  |员工的名字。                        |
|middleName          |string  |员工的中间名。                       |
|surname             |string  |员工的姓氏                            |
|jobTitle            |string  |员工的完整名称                          |
|address             |[翻.省略](../resources/dynamics-complextypes.md)|指定员工的地址。 此地址将显示在员工的所有资源文档中。|
|phoneNumber         |string  |指定员工的电话号码。             |
|mobilePhone         |string  |指定员工的移动电话号码。      |
|电子邮件               |string  |指定员工的电子邮件地址。                |
|personalEmail       |string  |指定员工的个人电子邮件地址。       |
|employmentDate      |date    |指定员工开始为公司工作的日期。|
|terminationDate     |date    |指定由于退休或开除而终止员工的日期。|
|status              |string  |指定员工的状态。 可能的值包括活动、非活动或已终止|
|birthDate           |date    |指定员工的出生日期。                |
|头像             |stream  |员工头像。 只读。                       |
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

