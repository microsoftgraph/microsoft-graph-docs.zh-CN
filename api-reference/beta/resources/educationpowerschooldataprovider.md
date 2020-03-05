---
title: educationPowerSchoolDataProvider 资源
description: 用于在将 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4fda7cc98c8041aad45a0ef8453affc9af34edc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501225"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider 资源

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于在将[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。

派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **connectionUrl** | String | 指向 PowerSchool 实例的连接 URL。 |
| **clientId** | String |  用于连接到 PowerSchool 的客户端 ID。 |
| **clientSecret** | String |  用于对与 PowerSchool 实例的连接进行身份验证的客户端密码。 |
| **schoolsIds** | String 集合 |  要同步的学校列表。 |
| **schoolYear** | String |  要同步的学校年。 |
| **allowTeachersInMultipleSchools** | 布尔 |  指示源是否具有单个学生或教师的多个标识符。 |
| **操作** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 要应用于同步配置文件的可选自定义项。|

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
