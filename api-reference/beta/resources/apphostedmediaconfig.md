---
title: appHostedMediaConfig 资源类型
description: 由应用程序托管的媒体堆栈。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0cb34d0673404c90607a8f1ac442ca1b7c504ce9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339179"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

由应用程序托管的媒体堆栈。

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| 块                              | String  | 由智能媒体代理生成的媒体配置 blob。    |
| removeFromDefaultAudioGroup       | Boolean | 从默认音频组中删除音频                       |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.appHostedMediaConfig"
}-->
```json
{
  "blob": "String",
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
