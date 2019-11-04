---
title: 创建 extensionProperty
description: 创建新的 extensionProperty。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb6ac47f3b33bb963181e71d7f5d7c83e2bf13b0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939689"
---
# <a name="create-extensionproperty"></a>创建 extensionProperty

创建新的[extensionProperty](../resources/extensionproperty.md)定义。 您可以使用此操作将自定义属性值添加到**extensionProperty**中定义的目标对象类型，使用目标对象的标准创建和更新请求。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:----------|
| Authorization  | Bearer {token}。必需。  |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下属性的[extensionProperty](../resources/extensionproperty.md)对象。


| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|DataType|String| 指定 extension 属性可以包含的值的数据类型。 支持以下值。 不可为空。 <ul><li>`Binary`-最多为256字节</li><li>`Boolean`</li><li>`DateTime`-必须以 ISO 8601 格式指定。 存储为 UTC 格式。</li><li>`Integer`-32-位值。</li><li>`LargeInteger`-64-位值。</li><li>`String`-最多为-256 个字符</li></ul>|
|name|String| 扩展属性的名称。 不可为空。 |
|targetObjects|String collection| 支持以下值。 不可为空。 <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a>响应

如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[extensionProperty](../resources/extensionproperty.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```

### <a name="response"></a>响应

如果成功，此方法在`201 Created`响应正文中返回响应代码和[extensionProperty](../resources/extensionProperty.md)对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
    "deletedDateTime": null,
    "appDisplayName": "Display name",
    "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "targetObjects": [
        "Application"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
