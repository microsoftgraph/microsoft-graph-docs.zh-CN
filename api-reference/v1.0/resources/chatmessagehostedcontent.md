---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
ms.localizationpriority: medium
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5d414e83e2de99aefbd264784adcad2ca90a8a40
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094385"
---
# <a name="chatmessagehostedcontent-resource-type"></a>chatMessageHostedContent 资源类型

命名空间：microsoft.graph

表示Teams消息中承载的内容，如图像或代码段。
[文件附件](chatmessageattachment.md)不是托管内容;它们存储在SharePoint或OneDrive。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 chatMessageHostedContent](../api/chatmessage-list-hostedcontents.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) 集合 | 检索消息的 **chatMessageHostedContent** 列表。 |
| [获取 chatMessageHostedContent](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | 读取 **chatMessageHostedContent** 对象的属性和关系。 |

## <a name="properties"></a>属性

chatMessageHostedContent 派生自 [teamworkHostedContent](teamworkhostedcontent.md)

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id            |String       | 只读。 表示聊天消息托管的内容标识符。|
|contentBytes  |Edm.Binary   | 只写。 发布新的聊天消息托管内容时，表示有效负载的字节数。 这些字符串表示为 base64Encoded 字符串。|
|contentType   |String       | 只写。 发布新的聊天消息托管内容时，表示内容类型，如 image/png。|

### <a name="instance-attributes"></a>实例属性

实例属性是具有特殊行为的属性。
这些属性是临时的，可以定义服务应执行的行为或提供短期属性值，如过期项目的下载 URL。

| 属性名称                     | 类型   | 说明
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.temporaryId      | string | 只写。 表示托管内容的 temporaryId，同时发布消息以引用要发送的 **chatMessage** 资源中的托管内容。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String"
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


