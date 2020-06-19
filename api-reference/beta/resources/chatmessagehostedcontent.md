---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 421ed3b1c439a7ae550100a113c651ab3e0a34b9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791067"
---
# <a name="chatmessagehostedcontent-resource-type"></a>chatMessageHostedContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在聊天消息中托管的团队内容，如图像或代码段。
[文件附件](chatmessageattachment.md)不是托管内容，它们存储在 SharePoint 或 OneDrive 中。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 chatMessageHostedContent](../api/chatmessage-list-chatmessagehostedcontents.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | 检索邮件的**chatMessageHostedContent**列表。 |
| [获取 chatMessageHostedContent](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | 读取**chatMessageHostedContent**对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
