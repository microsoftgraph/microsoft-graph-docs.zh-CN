---
title: teamworkHostedContent 资源类型
description: 表示 Microsoft Teams 托管的丰富内容
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 93b3b4fc817c1fe3aa3973a112b9cf887c825b6e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578849"
---
# <a name="teamworkhostedcontent-resource-type"></a>teamworkHostedContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft Teams 中的丰富内容，如图像和代码段。 有关频道和聊天消息[中的丰富内容](chatMessage.md)，请参阅[chatMessageHostedContent。](chatMessageHostedContent.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentBytes|Binary|仅写入。 托管内容存储的字节 (例如图像) 。|
|contentType|String|仅写入。 内容类型，如 image/png、image/jpg。|
|id|字符串|托管内容的 ID。|

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

