---
title: directoryObject： 增量
description: 获取新创建、 更新或删除以下类型的目录对象： 用户、 组和组织的联系人，请在单个增量查询。 请参阅修订的详细信息。
ms.openlocfilehash: 98674a141c0567defb06da7b1ccd95a209aaa4f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043348"
---
# <a name="directoryobject-delta"></a>directoryObject： 增量

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

获取新创建、 更新或删除以下类型的目录对象：[用户](../resources/user.md)、[组](../resources/group.md)和[组织的联系人](../resources/orgcontact.md)，请在单个增量查询。 有关详细信息，请参阅[修订](/graph/delta-query-overview)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.AccessAsUser.All  |
|委派（个人 Microsoft 帐户） | 不支持。  |
|应用程序 | Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

若要开始跟踪的更改，您发出请求包含增量函数对 directoryObjects 资源。

<!-- { "blockType": "ignored" } -->

```http
GET /directoryObjects/delta
```

## <a name="query-parameters"></a>查询参数

跟踪更改会导致一个或多个**增量**函数调用的往返。 如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。 Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。

只需预先指定所需的任何查询参数一次。

在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数 | 类型 |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

此方法支持可选的 OData 查询参数，以帮助自定义响应。

- 您可以使用`$filter`与特殊`isOf`派生自 directoryObject 运算符筛选类型的子集。
  - 您可以组合使用的多个表达式`or`，这使您能够具有跟踪多个类型的单个增量查询。 请参阅[第三个示例](#request-3)的详细信息。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者&lt;令牌&gt;|
| Content-Type  | application/json |
| Prefer | 返回 = 最少 <br><br>指定与请求使用此标头`deltaLink`会返回自上次循环后已更改的对象属性。 可选。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户](../resources/directoryobject.md)集合的对象。 响应还包括`nextLink`URL 或`deltaLink`URL。

- 如果`nextLink`返回 URL:
  - 这指示有会话中检索的数据的其他页面。 应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。
  - 响应包含一组相同的属性，如初始增量查询请求中所示。 这样，您可以在启动增量周期捕获对象的完整当前状态。

- 如果`deltaLink`返回 URL:
  - 这表明没有更多有关要返回的资源的现有状态数据。 保存并使用`deltaLink`URL 以了解如何更改为下一轮中的资源。
  - 您可以选择指定`Prefer:return=minimal`标头，以响应时间以来已经更改的属性值中包括`deltaLink`颁发。

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>默认值： 返回作为初始增量请求的同一属性

默认情况下，请求使用`deltaLink`或`nextLink`与选定初始增量查询中相同的属性返回以下方式：

- 如果已更改的属性，在响应中包含的新值。 这包括属性被设置为 null 值。
- 如果具有未更改的属性，在响应中包含的旧值。
- 如果从未它将不会包含在响应中根本之前设置该属性。


> **注意：** 与此行为，通过查看响应它不能以告知属性是否已更改或未。 此外，则 delta 响应容易很大，因为它们包含的所有属性值。

#### <a name="alternative-return-only-the-changed-properties"></a>可选： 仅返回已更改的属性

添加可选请求标头中的`prefer:return=minimal`-导致以下行为：

- 如果已更改的属性，在响应中包含的新值。 这包括属性被设置为 null 值。
- 如果具有未更改的属性，该属性不包括在响应中根本。 （不同于默认行为。）

> **注意：** 标头可以添加到`deltaLink`任何时间点的增量周期中的请求。 头只影响的响应中包括的属性集，而不会影响如何执行增量查询。

## <a name="example"></a>示例

### <a name="request-1"></a>请求 1

下面展示了示例请求。 没有任何`$select`参数，以便跟踪和返回一组默认属性。
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
```

### <a name="response-1"></a>响应 1

以下是时使用的响应示例`deltaLink`获取从查询初始化。 不`isOf`已使用筛选器，以便返回所有派生自 directoryObject 的类型。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": ["string"],
      "city": "string",
      "companyName": "string",
      "country": "string",
      "department": "string",
      "displayName": "string",
      "givenName": "string",
      "id": "string (identifier)",
      "jobTitle": "string",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-2"></a>请求 2

下一个示例演示如何使用备用内容最少响应行为：
<!-- {
  "blockType": "request",
  "name": "directoryObject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta
Prefer: return=minimal
```

### <a name="response-2"></a>响应 2

以下是时使用的响应示例`deltaLink`获取从查询初始化。 请注意会返回实际发生了更改的属性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "displayName": "John Smith"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "description": null,
      "displayName": "testgp"
    },
    {
      "@odata.type": "#microsoft.graph.orgContact",
      "id": "8f301319-4b4e-493f-8067-bce1dec76e7a",
      "businessPhones": "12345"
    },
    <...response trimmed for brevity...>
  ]
}
```

### <a name="request-3"></a>请求 3

下面的示例演示初始请求使用`isOf`运算符筛选出只有用户和组的实体：
<!-- {
  "blockType": "request",
  "name": "directoryobject_delta"
}-->

```http
GET https://graph.microsoft.com/beta/directoryObjects/delta?$filter=isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')
```

### <a name="response-3"></a>响应 3

以下是时使用的响应示例`deltaLink`获取从查询初始化。 请注意返回的唯一用户和组对象：

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.nextLink":"https://graph.microsoft.com/beta/directoryObjects/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "01754bb5-89de-4003-be72-9106a9fb16f2",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "city": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "createdDateTime": null,
      "department": null,
      "displayName": "John Smith",
      "givenName": null,
      "jobTitle": null,
      <...response trimmed for brevity...>
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "cf33844a-b6f8-4d4d-84f4-54e8d45094f0",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-06-20T16:50:09Z",
      "description": null,
      "displayName": "testgp",
      <...response trimmed for brevity...>
    },
    <...response trimmed for brevity...>
  ]
}
```

- [使用增量查询来跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。
- [获取用户的增量更改](/graph/delta-query-users)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
