---
title: userAgent 资源类型
description: userAgent 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a32c74957d0d0a2c41323c1f76d4e990897d61948892821e2d56154eceec271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189917"
---
# <a name="useragent-resource-type"></a>userAgent 资源类型

命名空间：microsoft.graph.callRecords

表示呼叫中终结点的用户代理。
[clientUserAgent](callrecords-clientuseragent.md)和[serviceUserAgent](callrecords-serviceuseragent.md)) 继承自此类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
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
