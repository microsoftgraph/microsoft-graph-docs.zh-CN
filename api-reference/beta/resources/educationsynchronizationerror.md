---
title: educationSynchronizationError 资源类型
description: 代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525141"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [获取同步错误](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**集合| 返回一个配置文件相关联的同步错误的列表。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **entryType** | string |  代表同步实体 （学校、 节、 学生、 教师）。       |
| errorCode | string |  表示此错误的错误代码。         |
| **ErrorMessage** | string |  包含错误的说明。        |
| **joiningValue** | string |  条目的唯一标识符。         |
| recordedDateTime | DateTimeOffset | 出现此错误的时间。         |
| **reportableIdentifier** | string | 此错误条目的标识符。       |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
