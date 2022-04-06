---
title: passwordAuthenticationMethod 资源类型
description: 注册到用户的密码的表示形式。
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 196964495c93a6d9dcdd35e58803500abee9c4a7
ms.sourcegitcommit: dab085b74666e190974a35e6a124d3ff1645fa25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/05/2022
ms.locfileid: "64646576"
---
# <a name="passwordauthenticationmethod-resource-type"></a>passwordAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户密码的表示形式。 为安全，不会在对象中返回密码本身，但可以采取措施重置密码。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[列出 passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) 集合 | 读取该用户的所有 **passwordAuthenticationMethod** 对象的属性和关系。 |
|[获取 passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | 读取 **passwordAuthenticationMethod 对象的属性和** 关系。 |
|[重置密码](../api/passwordauthenticationmethod-resetpassword.md)|无|在云中重置用户密码，如果已同步，则重置本地密码。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|上次更新此密码的日期和时间。 此属性当前未填充。 只读。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|id|字符串| 此密码的标识符已注册到此用户。 这通常是 `28c10230-6103-485e-b985-444c60001490`。 只读。|
|密码|String|为安全，始终从 LIST 或 GET 操作 `null` 返回密码。|

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


