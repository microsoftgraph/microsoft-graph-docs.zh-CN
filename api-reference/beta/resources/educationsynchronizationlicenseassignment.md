---
title: educationSynchronizationLicenseAssignment 资源类型
description: 代表分配给用户帐户的许可信息。 该资源将用于创建新的用户帐户时设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c60b868ab8d973f6249d7e9ea2b30415d4b8a1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409676"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>educationSynchronizationLicenseAssignment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表分配给用户帐户的许可信息。 该资源将用于创建新的用户帐户时设置许可证分配。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string | 要分配许可证的用户角色类型。 可取值为：`student`、`teacher`。         |
| **skuIds** | 字符串集合 |  表示分配的许可证的 SKU 标识符。        |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
