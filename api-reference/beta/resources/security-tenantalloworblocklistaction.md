---
title: tenantAllowOrBlockListAction 资源类型
description: 表示租户允许或阻止列表操作
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 26dc913078122a1bbb994369e63e2e2c0336f6c0
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856684"
---
# <a name="tenantalloworblocklistaction-resource-type"></a>tenantAllowOrBlockListAction 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户允许或阻止列表操作。 当管理员创建电子邮件威胁提交时，还可以提供租户允许阻止列表操作。 提供租户允许阻止列表操作时，威胁提交会自动向租户允许块列表添加相关项目 (URL、附件、发件人) 。

## <a name="properties"></a>属性
| 属性           | 类型                                        | 说明                                                                      |
|:-------------------|:--------------------------------------------|:---------------------------------------------------------------------------------|
| action             | tenantAllowBlockListAction                  | 指定租户允许块列表是允许还是阻止。 可能的值为： `allow`、 `block`和 `unkownFutureValue`。|
| expirationDateTime | DateTimeOffset                              | 指定租户 allow-block-list 在日期时间到期的时间。  |
| 注意               | String                                      | 指定添加到租户的便笺允许字符串格式的块列表条目。 |
| results            | collection ([security.tenantAllowBlockListEntryResult](../resources/security-tenantallowblocklistentryresult.md))  | 包含导致创建租户 allow-block-list 条目的提交结果。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.tenantAllowOrBlockListAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.tenantAllowOrBlockListAction",
  "action": "String",
  "results": [
    {
      "@odata.type": "microsoft.graph.security.tenantAllowBlockListEntryResult"
    }
  ],
  "expirationDateTime": "String (timestamp)",
  "note": "String"
}
```

