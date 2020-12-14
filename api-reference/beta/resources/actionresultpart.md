---
title: actionResultType 资源类型
description: 为批量操作的响应建模的抽象类型。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a092fa4a322d0d207550947559cb5dfff4ad4625
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663998"
---
# <a name="actionresultpart-resource-type"></a>actionResultPart 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用作批量操作响应建模基础的抽象类型。 根据 **响应** 是否表示错误，选择性地填充错误属性。

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:---------------|:--------|:----------|
|error|[publicError](publicerror.md) |在批量操作过程中发生的错误（如果有）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.actionResultPart"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.actionResultPart",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  }
}
```
## <a name="see-also"></a>另请参阅

- [aadUserConversationMemberResult](aadUserConversationMemberResult.md)
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


