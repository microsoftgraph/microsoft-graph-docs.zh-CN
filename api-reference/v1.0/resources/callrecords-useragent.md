---
title: userAgent 资源类型
description: UserAgent 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 795332d58359d0a0a5dd2776f6c93923fe1bafd8
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492010"
---
# <a name="useragent-resource-type"></a>userAgent 资源类型

命名空间：microsoft.graph.callRecords

表示调用中终结点的用户代理。
[ClientUserAgent](callrecords-clientuseragent.md)和[serviceUserAgent](callrecords-serviceuseragent.md)）类型继承自此类型。

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|applicationVersion|String|标识此终结点使用的应用程序软件的版本。|
|headerValue|String|此终结点报告的用户代理标头值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userAgent",
  "baseType": null
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->