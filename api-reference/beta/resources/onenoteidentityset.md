---
title: oneNoteIdentitySet 资源类型
description: '**支持即将推出**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 32c4d7001f0ab8a7341470e749aa4dc6833599e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039214"
---
# <a name="onenoteidentityset-resource-type"></a>oneNoteIdentitySet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**支持即将推出**

OneNoteIdentitySet 类型是 [OneNoteIdentity](onenoteidentity.md) 对象的键控集合。
它用于表示一组与 _笔记本_、 _节_ 或 _页面_的各种事件相关联的标识，如 " _创建者_ " 或 " _上次修改者_"。 
 
当前它包含单个密钥，即 _**user**_。  将来，可能会添加用于更改项目的设备或应用程序等键。

将来，此类型将与[了解 identityset](identityset.md)合并。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|user|[onenoteIdentity](onenoteidentity.md)|一个代表用户的 OneNoteIdentity 资源。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


