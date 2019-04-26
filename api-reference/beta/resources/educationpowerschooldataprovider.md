---
title: educationPowerSchoolDataProvider 资源
description: 用于在将 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cee763995dd5a75b64d94e5f170d6fea992c20b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340563"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider 资源

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
| **allowTeachersInMultipleSchools** | Boolean |  指示源是否具有单个学生或教师的多个标识符。 |
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
