---
title: tenantAllowBlockListEntryResult 资源类型
description: 表示租户允许块列表条目结果。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9e5a92fbc215c814ce2f55a1e9a16407bc60f147
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856663"
---
# <a name="tenantallowblocklistentryresult-resource-type"></a>tenantAllowBlockListEntryResult 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户允许块列表条目的结果。 租户允许块列表项的条目可以是 URL、附件或发件人。

## <a name="properties"></a>属性
| 属性           | 类型                          | 说明                                             |
|:-------------------|:------------------------------|:--------------------------------------------------------|
| entryType          | tenantAllowBlockListEntryType | 租户的条目类型允许块列表。 可能的值是：`url`、`fileHash`、`sender``recipient`和 `unkownFutureValue`。  |
| expirationDateTime | DateTimeOffset                | 指定此条目将在日期时间到期的时间。 |
| 身份           | String                        | 指定租户生成的条目允许块列表系统的标识。 |
| status             | longRunningOperationStatus    | 指定租户是否允许阻止列表条目创建操作成功。 可能的值是：`notStarted`、`running`、`succeeded`、`failed``skipped`和 `unkownFutureValue`。 |
| value              | String                        | 指定创建的租户允许块列表条目的值。  |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.tenantAllowBlockListEntryResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.tenantAllowBlockListEntryResult",
  "identity": "String",
  "value": "String",
  "entryType": "String",
  "expirationDateTime": "String (timestamp)",
  "status": "String"
}
```

