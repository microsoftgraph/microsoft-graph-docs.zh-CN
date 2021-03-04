---
title: passwordAuthenticationMethod 资源类型
description: 向用户注册的密码的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2982b79df70b65bf09dff8f9b906ed85a8854b52
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444082"
---
# <a name="passwordauthenticationmethod-resource-type"></a>passwordAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户密码的表示形式。 出于安全考虑，密码本身永远不会在对象中返回，但可以采取措施重置密码。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[列出 passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) 集合 | 读取该用户的所有 **passwordAuthenticationMethod** 对象的属性和关系。 |
|[获取 passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | 读取 **passwordAuthenticationMethod 对象的属性和** 关系。 |
|[重置密码](../api/passwordauthenticationmethod-resetpassword.md)|无|在云中重置用户密码，如果同步，则重置本地密码。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|上次更新此密码的日期和时间。 此属性当前未填充。 只读。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|String| 此密码的标识符已注册到此用户。 只读。|
|密码|String|为了安全，密码始终从 LIST 或 GET 操作返回为 null。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "creationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "password": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


