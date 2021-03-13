---
title: 凭据资源类型
description: 指示用于登录应用程序的单个凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0521f766a7a0da482cf67628c3816935ee9270b8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761679"
---
# <a name="credential-resource-type"></a>凭据资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示用于登录应用程序的单个凭据。 例如，username 是一个凭据，password 是另一个凭据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|fieldId|String|此凭据的字段名称。 例如用户名或密码或 phoneNumber。 这由应用程序定义。 必须与 singleSignOnSettings/password 对象上的 html 字段中的项匹配。|
|type|String|此凭据的类型。 有效值：用户名、密码或其他。|
|value|String|此凭据的值。 例如，mysuperhiddenpassword。 请注意，密码的值为仅写值，该值永远不能读回。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credential",
  "baseType": null
}-->

```json
{
  "fieldId": "param_username",
  "value": "myusername",
  "type": "username"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


