---
title: educationSynchronizationLicenseAssignment 资源类型
description: 表示要分配给用户帐户的许可证信息。 创建新用户帐户时，资源将用于设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9d46e19c1869f7dff96a563dd54b1b9f303ce85a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434961"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>educationSynchronizationLicenseAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要分配给用户帐户的许可证信息。 创建新用户帐户时，资源将用于设置许可证分配。

## <a name="properties"></a>属性

| 属性  | 类型              | 说明                                                                                    |
| :-------- | :---------------- | :--------------------------------------------------------------------------------------------- |
| appliesTo | String            | 要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`、`faculty`。 |
| skuIds    | 字符串集合 | 表示要分配的许可证的 SKU 标识符。                                      |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "skuIds": ["String"]
}
```
