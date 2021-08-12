---
title: clientUserAgent 资源类型
description: clientUserAgent 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6c1150cf60b3b042358ff1a854944b14722e2a9717daaed064d9d63392e475aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212211"
---
# <a name="clientuseragent-resource-type"></a>clientUserAgent 资源类型

命名空间：microsoft.graph.callRecords

表示呼叫中终结点的客户端用户代理。 继承自 [userAgent](callrecords-useragent.md) 类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|applicationVersion|String|标识此终结点使用的应用程序软件的版本。|
|headerValue|String|此终结点报告的用户代理标头值。|
|平台|microsoft.graph.callRecords.clientPlatform|标识此终结点使用的平台。 可取值为：`unknown`、`windows`、`macOS`、`iOS`、`android`、`web`、`ipPhone`、`roomSystem`、`surfaceHub`、`holoLens`、`unknownFutureValue`。|
|productFamily|microsoft.graph.callRecords.productFamily|标识此终结点使用的应用程序软件系列。 可取值为：`unknown`、`teams`、`skypeForBusiness`、`lync`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.clientUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "platform": "String",
  "productFamily": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "clientUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
