---
title: chatMessageHostedImage 资源类型
description: 代表了 chatmessage 中的承载的图像。
localization_priority: Normal
author: clearab
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e217234b8ea6c6510b85af1bf1002e589e4366e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974001"
---
# <a name="chatmessagehostedimage-resource-type"></a>chatMessageHostedImage 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表[了 chatmessage](../resources/chatmessage.md)中的承载的图像。

托管图像是显示在邮件正文中的图像。包含以开头`https://graph.microsoft.com`的 src \<属性的 img> 标记中的**内容。**

并非邮件中的所有图像都承载图像, Microsoft 团队还支持公用图像 (其中 img src 属性指向公共网站)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[在了 chatmessage 中列出 chatMessageHostedImages](../api/chatmessagehostedimage-list-hostedimages.md) | [chatMessageHostedImage](chatmessagehostedimage.md)集合 | **了 chatmessage**中所有托管图像的列表。|
|[获取 chatMessageHostedImage](../api/chatmessagehostedimage-get.md) | [chatMessageHostedImage](chatmessagehostedimage.md) | 获取一个托管的图像。|
|[chatMessageHostedImage: getBytes](../api/chatmessagehostedimage-getbytes.md) | 内容类型: 图像/jpeg | 获取托管图像的原始字节。|

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 消息的唯一 ID。|
|URL| string | 从中检索图像内容的 url。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
