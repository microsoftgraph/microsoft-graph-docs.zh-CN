---
title: passwordSingleSignOnField 资源类型
description: 用于捕获密码 SSO 凭据的字段
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e0db6198d61715603acee54e7351c9fd5f2fed88
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761547"
---
# <a name="passwordsinglesignonfield-resource-type"></a>passwordSingleSignOnField 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含用于填充基于密码的单一登录的使用凭据的要捕获的字段。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|customizedLabel|String|自定义的标题/标签替代。|
|defaultLabel|String|如果未提供 customizedLabel，则使用的标签。 只读。|
|fieldId|String|用于标识字段类型的 ID。 这是一个内部 ID，可能的值是 `param_1` `param_2` `param_userName` 、、、。 `param_password`|
|type|String|   凭据的类型。 值可以是 `text` `password` 、。|

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

