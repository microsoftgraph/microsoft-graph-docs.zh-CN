---
title: educationSynchronizationError 资源类型
description: 表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory （Azure AD）同步的每个条目，都会生成一个唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59650bc56554b9bd4dd7135ae44d53e153c159f8
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434835"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory （Azure AD）同步的每个条目，都会生成一个唯一的错误。

## <a name="methods"></a>方法

| 方法                                                                     | 返回类型                                  | 说明                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [获取同步错误](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**集合 | 返回与配置文件关联的同步错误的列表。 |

## <a name="properties"></a>属性

| 属性             | 类型           | 说明                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| id                   | 字符串         | 资源的唯一标识符。 （只读）             |
| entryType            | 字符串         | 表示 sync 实体（学校、节、学生、教师）。 |
| errorCode            | String         | 表示此错误的错误代码。                       |
| errorMessage         | 字符串         | 包含错误的说明。                            |
| joiningValue         | 字符串         | 条目的唯一标识符。                            |
| recordedDateTime     | DateTimeOffset | 出现此错误的时间。                           |
| reportableIdentifier | 字符串         | 此错误项的标识符。                             |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
  "id": "String",
  "entryType": "String",
  "errorCode": "String",
  "errorMessage": "String",
  "joiningValue": "String",
  "recordedDateTime": "DateTimeOffset",
  "reportableIdentifier": "String"
}
```
