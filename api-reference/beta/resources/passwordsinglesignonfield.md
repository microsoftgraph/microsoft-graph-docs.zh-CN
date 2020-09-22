---
title: passwordSingleSignOnField 资源类型
description: 用于捕获密码 SSO 凭据的字段
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d79f2347acabae0323e008a43adb7938d70d3768
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998192"
---
# <a name="passwordsinglesignonfield-resource-type"></a>passwordSingleSignOnField 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含要捕获以填充基于密码的单一登录的使用凭据的字段。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|customizedLabel|String|用于自定义的标题/标签覆盖。|
|defaultLabel|String|未提供 customizedLabel 时将使用的标签。 只读。|
|fieldId|String|用于标识字段类型的 Id。 这是一个内部 id，可能的值为、、、 `param_1` `param_2` `param_userName` `param_password` 。|
|type|String|   凭据的类型。 值可以是 `text` ， `password` 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnField",
  "baseType": null
}-->

```json
{
  "customizedLabel": "String",
  "defaultLabel": "String",
  "fieldId": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

