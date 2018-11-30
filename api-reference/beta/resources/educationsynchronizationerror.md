---
title: educationSynchronizationError 资源类型
description: 代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。
ms.openlocfilehash: 91a633ab4056e8e86854a0e2d45ae13e22da19a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042099"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-|:-|:-|
| [获取同步错误](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**集合| 返回一个配置文件相关联的同步错误的列表。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **entryType** | string |  代表同步实体 （学校、 节、 学生、 教师）。       |
| **errorCode** | string |  表示此错误的错误代码。         |
| **errorMessage** | string |  包含错误的说明。        |
| **joiningValue** | string |  条目的唯一标识符。         |
| **recordedDateTime** | DateTimeOffset | 出现此错误的时间。         |
| **reportableIdentifier** | string | 此错误条目的标识符。       |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
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
