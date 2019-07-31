---
title: informationalUrl 资源类型
description: 应用程序的基本配置文件信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e2eaad003f4669623a4db4af1b364e05198515d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006253"
---
# <a name="informationalurl-resource-type"></a>informationalUrl 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

应用程序的基本配置文件信息。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|部门|String| 指向应用程序的市场营销页面的链接。 例如，https://www.contoso.com/app/marketing |
|私密性|String| 指向应用程序的隐私声明的链接。 例如，https://www.contoso.com/app/privacy |
|支持|String| 指向应用程序的支持页的链接。 例如，https://www.contoso.com/app/support |
|termsOfService|String| 指向应用程序的服务条款声明的链接。 例如，https://www.contoso.com/app/termsofservice |

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
