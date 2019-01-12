---
title: educationPowerSchoolDataProvider 资源
description: 用于 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a22c3cf68a4a5b4c12dc4e7105f17eed4fc006f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982755"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider 资源

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

用于[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。

派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **connectionUrl** | 字符串 | 连接到 PowerSchool 实例 URL。 |
| **clientId** | 字符串 |  用于连接到 PowerSchool 客户端 ID。 |
| **clientSecret** | 字符串 |  客户端机密进行身份验证与 PowerSchool 实例的连接。 |
| **schoolsIds** | String 集合 |  学校同步的列表。 |
| **schoolYear** | 字符串 |  要同步的学校年份。 |
| **allowTeachersInMultipleSchools** | Boolean |  指示源是否有多个标识符是单个学生或教师。 |
| **自定义项** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 可选自定义要应用于同步配置文件。|

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
