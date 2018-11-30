---
title: appHostedMediaConfig 资源类型
description: 媒体堆栈承载的应用程序。
ms.openlocfilehash: 39080a8fdb5688ed9f1a5a8daba43266a0e7003e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042771"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

媒体堆栈承载的应用程序。

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                                                     |
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
