---
title: educationSynchronizationError 资源类型
description: 表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory (Azure AD) 进行同步的每个条目，都会生成一个唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2af4ef9f17452714373d42b67af6e87a7f87fe1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989645"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory (Azure AD) 进行同步的每个条目，都会生成一个唯一的错误。

## <a name="methods"></a>方法

| 方法                                                                     | 返回类型                                  | 说明                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [获取同步错误](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError** 集合 | 返回与配置文件关联的同步错误的列表。 |

## <a name="properties"></a>属性

| 属性             | 类型           | 说明                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| id                   | String         | 资源的唯一标识符。  (只读)              |
| entryType            | String         | 表示 (学校、section、student、教师) 的同步实体。 |
| errorCode            | String         | 表示此错误的错误代码。                       |
| errorMessage         | String         | 包含错误的说明。                            |
| joiningValue         | String         | 条目的唯一标识符。                            |
| recordedDateTime     | DateTimeOffset | 出现此错误的时间。                           |
| reportableIdentifier | String         | 此错误项的标识符。                             |

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


