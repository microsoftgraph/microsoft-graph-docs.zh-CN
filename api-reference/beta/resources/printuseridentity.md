---
title: printUserIdentity 资源类型
description: 代表通用打印服务中的用户标识。 映射到 Azure AD 用户。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8a695bed829d6c7e8825898da366737427195e1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070653"
---
# <a name="printuseridentity-resource-type"></a>printUserIdentity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表通用打印服务中的用户标识。 映射到 [Azure Active Directory (AZURE AD) 用户](user.md)。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|PrintUserIdentity 的标识符。 只读。|
|displayName|String|PrintUserIdentity 的显示名称。|
|ipAddress|String|PrintUserIdentity 的 IP 地址。 未填充。|
|userPrincipalName|String|PrintUserIdentity 的用户主体名称 (UPN) 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUserIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUserIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


