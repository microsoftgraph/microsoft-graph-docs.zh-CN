---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8f1577ab7ded60dfd3cad88641bfb11f83d6ad5b
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630289"
---
# <a name="chatmessagehostedcontent-resource-type"></a>chatMessageHostedContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在聊天消息中托管的团队内容，如图像或代码段。
[文件附件](chatmessageattachment.md)不是托管内容;它们存储在 SharePoint 或 OneDrive 中。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 chatMessageHostedContent](../api/chatmessage-list-chatmessagehostedcontents.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | 检索邮件的**chatMessageHostedContent**列表。 |
| [获取 chatMessageHostedContent](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | 读取**chatMessageHostedContent**对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id            |字符串       | 只读。 表示聊天消息承载的内容标识符。|
|contentBytes  |Edm.Binary   | 只写。 发布新的聊天邮件承载的内容时，表示有效负载的字节数。 它们表示为 base64Encoded 字符串。|
|contentType   |String       | 只写。 发布新的聊天邮件承载的内容时，表示内容的类型，如 image/png。|

### <a name="instance-attributes"></a>实例属性

实例属性是具有特殊行为的属性。
这些属性是临时性的，可定义服务应执行的行为，也可以提供短期属性值，如项目的下载 URL 过期。

| 属性名称                     | 类型   | 说明
|:----------------------------------|:-------|:--------------------------------
| @microsoft temporaryId      | string | 只写。 表示在发布邮件时承载的内容的 temporaryId，以引用正在发送的**了 chatmessage**资源中的托管内容。|

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
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String",
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
