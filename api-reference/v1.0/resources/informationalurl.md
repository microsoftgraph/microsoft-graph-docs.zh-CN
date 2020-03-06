---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ebf2a79931936e8f45f93cba46b1fefdbf0163b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532885"
---
# <a name="informationalurl-resource-type"></a>informationalUrl 资源类型

命名空间：microsoft.graph

应用程序的基本配置文件信息。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|logoUrl|字符串|指向应用程序徽标的 CDN URL，只读。|
|marketingUrl|字符串| 指向应用程序的市场营销页面的链接。 例如，https://www.contoso.com/app/marketing |
|privacyStatementUrl|字符串| 指向应用程序的隐私声明的链接。 例如，https://www.contoso.com/app/privacy |
|supportUrl|字符串| 指向应用程序的支持页的链接。 例如，https://www.contoso.com/app/support |
|termsOfServiceUrl|字符串| 指向应用程序的服务条款声明的链接。 例如，https://www.contoso.com/app/termsofservice |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "logoUrl": "String",
  "marketingUrl": "String",
  "privacyStatementUrl": "String",
  "supportUrl": "String",
  "termsOfServiceUrl": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
