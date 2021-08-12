---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: e0c60cdde2d636321f3777b4b41bdf11bfe1da69d3303169f4fce1a3a71b3acc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178386"
---
# <a name="informationalurl-resource-type"></a>informationalUrl 资源类型

命名空间：microsoft.graph

应用程序的基本配置文件信息。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|logoUrl|String|CDN指向应用程序徽标的 URL，只读。|
|marketingUrl|String| 链接到应用程序的营销页面。 例如，https://www.contoso.com/app/marketing |
|privacyStatementUrl|String| 指向应用程序隐私声明的链接。 例如，https://www.contoso.com/app/privacy |
|supportUrl|String| 链接到应用程序的支持页面。 例如，https://www.contoso.com/app/support |
|termsOfServiceUrl|String| 指向应用程序的服务声明条款的链接。 例如，https://www.contoso.com/app/termsofservice |

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

