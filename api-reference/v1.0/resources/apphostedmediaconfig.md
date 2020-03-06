---
title: appHostedMediaConfig 资源类型
description: 由应用程序托管的媒体堆栈。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43cc6f690ce2c491b4e49de4c1d641964df7a07d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533164"
---
# <a name="apphostedmediaconfig-resource-type"></a>appHostedMediaConfig 资源类型

命名空间：microsoft.graph

由应用程序托管的媒体堆栈。

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                                                     |
| :-------------------------------- | :------ | :---------------------------------------------------------------|
| 块                              | 字符串  | 由智能媒体代理生成的媒体配置 blob。    |

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
