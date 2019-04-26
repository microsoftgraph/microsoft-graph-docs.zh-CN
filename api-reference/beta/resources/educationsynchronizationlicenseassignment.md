---
title: educationSynchronizationLicenseAssignment 资源类型
description: 表示要分配给用户帐户的许可证信息。 创建新用户帐户时, 资源将用于设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ae9b89d9fe921967b50b8e290ce29026dbc35ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334049"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>educationSynchronizationLicenseAssignment 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要分配给用户帐户的许可证信息。 创建新用户帐户时, 资源将用于设置许可证分配。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string | 要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`。         |
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
