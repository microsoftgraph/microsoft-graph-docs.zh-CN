---
title: appHostedMediaConfig 资源类型
description: 由应用程序托管的媒体堆栈。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6bafd755ef2c806b703bf9ec5ac872f826de1e1c
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006773"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

由应用程序托管的媒体堆栈。

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| 块                              | String  | 由智能媒体代理生成的媒体配置 blob。    |
| removeFromDefaultAudioGroup       | 布尔 | 从默认音频组中删除音频                       |

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
