---
title: educationSynchronizationError 资源类型
description: 表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory (Azure AD) 同步的每个条目, 都会生成一个唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 11e5be9893c6a50615774e0d2a8e4d51c9576da6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972409"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory (Azure AD) 同步的每个条目, 都会生成一个唯一的错误。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [获取同步错误](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**集合| 返回与配置文件关联的同步错误的列表。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **entryType** | string |  表示 sync 实体 (学校、节、学生、教师)。       |
| **错误** | string |  表示此错误的错误代码。         |
| **errorMessage** | string |  包含错误的说明。        |
| **joiningValue** | string |  条目的唯一标识符。         |
| **recordedDateTime** | DateTimeOffset | 出现此错误的时间。         |
| **reportableIdentifier** | string | 此错误项的标识符。       |

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
