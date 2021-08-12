---
title: teamworkHostedContent 资源类型
description: 表示由网站托管的丰富Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7fca2d17db16e101edb22bd1ddfa31e4234e35ec6817f226209429f6cb97757a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189252"
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
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```
