---
title: educationSynchronizationLicenseAssignment 资源类型
description: 表示要分配给用户帐户的许可证信息。 创建新用户帐户时, 资源将用于设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5d1aaf2784434525e2fa750ad78966d6cbf15bc8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750134"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>educationSynchronizationLicenseAssignment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要分配给用户帐户的许可证信息。 创建新用户帐户时, 资源将用于设置许可证分配。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string | 要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`、`faculty`。         |
| **skuIds** | 字符串集合 |  表示要分配的许可证的 SKU 标识符。        |

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
