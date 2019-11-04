---
title: 创建 externalItem
description: 创建新的 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d2859ddf78933dee925466c95884e26257f8af5b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938069"
---
# <a name="create-externalitem"></a>创建 externalItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)。

此 API 可用于创建自定义项或文件。 通过在 JSON 正文中包含`@odata.type`属性来指定要创建的类型。 包含的[externalConnection](../resources/externalconnection.md)必须具有相应类型的已注册[架构](../resources/schema.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | ExternalItem |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>路径参数

| 参数     | 类型   | 描述                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | string | 包含`id` [externalConnection](../resources/externalconnection.md)的属性 |
| item-id       | string | 开发人员提供`id`的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)属性。 如果不存在具有此`id`项的项目，则会创建一个新项目。 如果某个项目已经存在`id`，则会被在正文中发送的对象覆盖。 |

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供[externalItem](../resources/externalitem.md)或[EXTERNALFILE](../resources/externalfile.md)对象的 JSON 表示形式。 有效负载限制为 4 MB。

### <a name="creating-an-externalitem"></a>创建 externalItem

在创建时`externalItem`，需要以下字段： `@odata.type`、 `acl`和。 `properties` 该`properties`对象必须至少包含一个属性。

所有`DateTime`类型属性都必须采用 ISO 8601 格式。

中的属性`externalItem`应在以下方案中使用有效负载中的类型说明符：

- 对于`String` type 属性，如果该值包含非 ASCII 字符。

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- 适用于所有集合类型。

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > 如果包含类型`Collection(DateTime)`的属性，则必须使用类型说明符`Collection(DateTimeOffset)`。

### <a name="creating-an-externalfile"></a>创建 externalFile

在创建时`externalFile`，需要以下字段`@odata.type`：、 `acl` `name`、和。 `url`

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-create-a-custom-item"></a>示例1：创建自定义项

#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "deny",
      "identitySource": "Azure Active Directory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": "Textual content of the file"
}
```

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

### <a name="example-2-create-a-file"></a>示例2：创建文件

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a>请求
<!-- markdownlint-enable MD024 -->

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "create_externalfile_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosofiles/items/myFile01
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalFile",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ],
  "createdDateTime": "2019-01-31T03:44:19.0354159Z",
  "modifiedDateTime": "2019-01-31T03:44:19.0354159Z",
  "createdBy": "Pradeep Gupta",
  "lastModifiedBy": "Adele Vance",
  "title": "Enterprise Search Graph Ingestion API",
  "url": "file://filesrv02.corp.contoso.com/data/project/Enterprise Search.docx",
  "name": "Enterprise Search.docx",
  "extension": "docx",
  "size": 8676776,
  "content": "The quick brown fox jumps over the lazy dog."
}
```

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
