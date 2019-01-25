---
title: educationSynchronizationCustomization 资源类型
description: '提供用于自定义资源实体学校数据配置文件同步设置。 自定义项可以应用于正在同步的所有实体。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513604"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用于自定义资源实体学校数据配置文件同步设置。 自定义项可以应用于正在同步的所有实体。 

>**注意：****SynchronizationStartDate**属性仅适用于**StudentEnrollment**实体。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **optionalPropertiesToSync** | Collection of String |  要同步的属性名称的集合。如果设置为 null，所有属性将都为同步。       |
| **synchronizationStartDate** | 日期/时间 |  同步的开始日期。 此值应设置为未来日期。 如果配置文件安装完成后，将会同步设置为 null，资源。 **注意：** 这仅适用于**StudentEnrollment**属性。      |
|**isSyncDeferred** |Boolean | 指示是否对父实体的同步推迟到以后。 |
| **allowDisplayNameUpdate** | Boolean |  指示是否可以通过同步来覆盖资源的显示名称。         |


## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
