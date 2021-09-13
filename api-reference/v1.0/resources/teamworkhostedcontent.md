---
title: teamworkHostedContent 资源类型
description: 表示由网站托管的丰富Microsoft Teams。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d53614b4d4f699890be7d244d78f7f1ec01890c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128178"
---
# <a name="teamworkhostedcontent-resource-type"></a>teamworkHostedContent 资源类型

命名空间：microsoft.graph

表示应用程序中丰富的内容，如图像和Microsoft Teams。 有关频道和聊天 [消息中的丰富内容，](chatMessage.md)请参阅 [chatMessageHostedContent](chatMessageHostedContent.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentBytes|Binary|只写。 托管内容存储的字节 (如图像) 。|
|contentType|String|只写。 内容类型。 sicj 为 image/png，image/jpg。|
|id|String|托管内容的 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```
