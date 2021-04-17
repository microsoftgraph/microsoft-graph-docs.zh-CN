---
title: teamworkHostedContent 资源类型
description: 表示由 Microsoft Teams 托管的丰富内容
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da0b157bab78867bd3309b4529afe8ef734f0144
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882311"
---
# <a name="teamworkhostedcontent-resource-type"></a>teamworkHostedContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft Teams 中的丰富内容，如图像和代码段。 有关频道和聊天 [消息中的丰富内容，](chatMessage.md)请参阅 [chatMessageHostedContent](chatMessageHostedContent.md)。

## <a name="methods"></a>方法

| 方法                                            | 返回类型                                       | 说明                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [获取应用图标字节数](../api/teamsappicon-get.md)     | [teamworkHostedContent](teamworkhostedcontent.md)                   | 获取支持 Teams 应用图标的托管内容的字节数。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentBytes|Binary|只写。 托管内容存储的字节 (如图像) 。|
|contentType|String|只写。 内容类型，如 image/png、image/jpg。|
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

