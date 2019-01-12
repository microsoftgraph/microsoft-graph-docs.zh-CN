---
title: appHostedMediaConfig 资源类型
description: 媒体堆栈承载的应用程序。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 36f869be347e2d55ec90079c62c5b6ebef85f144
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928582"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

媒体堆栈承载的应用程序。

## <a name="properties"></a>属性

| 属性                          | 类型    | Description                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| blob                              | 字符串  | 媒体配置 blob 智能媒体代理生成。    |
| removeFromDefaultAudioGroup       | 布尔 | 从默认音频组中删除音频                       |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "appHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
