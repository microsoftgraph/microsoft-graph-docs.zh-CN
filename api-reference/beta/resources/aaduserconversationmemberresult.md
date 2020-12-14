---
title: aadUserConversationMemberResult 资源类型
description: 用于对 aadUserConversationMember 上的批量操作响应建模的资源。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8251107c325bdbe2c5ff9e6df95a2d08277dde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663903"
---
# <a name="aaduserconversationmemberresult-resource-type"></a>aadUserConversationMemberResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示由请求中的 [aadUserConversationMember ](aadUserConversationMember.md) () 中指定的每个成员的个人响应。
此资源是 [actionResultPart 资源的派生](actionresultpart.md) 项。

## <a name="properties"></a>属性

| 属性 | 类型   | 描述 |
|:---------------|:--------|:----------|
|userId|`String`|作为批量操作一部分添加的 Azure AD 用户的用户对象 ID。|
|error|[publicError](publicerror.md) |在批量操作过程中发生的错误（如果有）。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserConversationMemberResult"
}-->

```json
{
    "userId": "string",
    "error": "microsoft.graph.publicError"
}
```

## <a name="see-also"></a>另请参阅

- [将成员批量添加到团队](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


