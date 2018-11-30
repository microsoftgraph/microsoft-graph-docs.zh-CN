---
title: chatMessageMention 资源类型
description: '代表 chatMessage 实体中的某个提及。 提及的可向用户、 团队、 自动程序或通道。 '
ms.openlocfilehash: 5f1e427b0ed2b8ffcfbc86417beb4719dc6fb2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041763"
---
# <a name="chatmessagemention-resource-type"></a>chatMessageMention 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表[chatMessage](chatmessage.md)实体中的某个提及。 提及的可向用户、 团队、 自动程序或通道。 

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ID|string|正在提到的实体的 id|
|mentionText|string|用来表示 Ex 提及的字符串： 用户的显示名称、 工作组名称等|
|提到|[identitySet](identityset.md)|已提及用户|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
