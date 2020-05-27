---
title: samlSingleSignOnSettings 资源类型
description: 表示 SAML 单一登录设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 60d7f28de54cd772ac440e6f72f61cd2bb08fe00
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383866"
---
# <a name="samlsinglesignonsettings-resource-type"></a>samlSingleSignOnSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与 SAML single sign-on 相关的设置的容器。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:---------------|:--------|:----------|
|relayState|String| 单一登录流完成后，服务提供程序将重定向到的相对 URI。 |


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
}-->

```json
{
    "relayState": "string",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "samlSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
