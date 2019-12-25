---
title: appHostedMediaConfig 资源类型
description: 由应用程序托管的媒体堆栈。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a5596e8e549cc22fe448de67669dde1d70727c3e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871090"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig 资源类型

由应用程序托管的媒体堆栈。

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| 块                              | String  | 由智能媒体代理生成的媒体配置 blob。    |

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
  "blob": "String"
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
