---
title: credential 资源类型
description: 指示用于登录应用程序的单个凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3b23249d7c0b898344113c5bcfe950c207891250
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658882"
---
# <a name="credential-resource-type"></a>credential 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示用于登录应用程序的单个凭据。 例如，username 是一个凭据，即 "密码" 是另一个凭据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|fieldId|字符串|此凭据的字段名称。 例如，username、password 或 phoneNumber。 这是由应用程序定义的。 必须与 singleSignOnSettings/password 对象上的 html 字段中的内容相匹配。|
|type|字符串|此凭据的类型。 有效值： username、password 或其他值。|
|value|String|此凭据的值。 例如，mysuperhiddenpassword。 注意：密码的值是只写的，该值永远不能读回。|

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
