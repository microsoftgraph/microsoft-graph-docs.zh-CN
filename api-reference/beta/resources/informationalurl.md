---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816980"
---
# <a name="informationalurl-resource-type"></a>informationalUrl 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

应用程序的基本配置文件信息。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:---------------|:--------|:----------|
|市场营销|字符串| 链接到应用程序的市场营销页。 例如，https://www.contoso.com/app/marketing |
|隐私|字符串| 链接到应用程序的隐私声明。 例如，https://www.contoso.com/app/privacy |
|支持|字符串| 链接到应用程序的支持网页。 例如，https://www.contoso.com/app/support |
|termsOfService|字符串| 链接到的服务语句的应用程序的术语。 例如，https://www.contoso.com/app/termsofservice |

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
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
