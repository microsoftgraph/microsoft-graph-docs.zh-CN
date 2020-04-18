---
title: passwordAuthenticationMethod 资源类型
description: 注册到用户的密码的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba932538e984af37a4f005ddcc2167c29d2267d0
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557911"
---
# <a name="passwordauthenticationmethod-resource-type"></a>passwordAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户密码的表示形式。 出于安全考虑，密码本身永远不会返回到对象中，但可以采取措施重置密码。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[列出 passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md)集合 | 读取此用户的所有**passwordAuthenticationMethod**对象的属性和关系。 |
|[获取 passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | 读取**passwordAuthenticationMethod**对象的属性和关系。 |
|[重置密码](../api/passwordauthenticationmethod-resetpassword.md)|无|在云中重置用户的密码，如果同步，则在本地进行同步。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|上次更新此密码的日期和时间。 当前未填充此属性。 只读。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|字符串| 为此用户注册的此密码的标识符。 只读。|
|密码|String|出于安全的的情况，密码始终在列表或 GET 操作中以 null 的形式返回。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "baseType": "",
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
