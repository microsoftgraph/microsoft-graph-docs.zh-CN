---
title: 应用程序： 增量
description: 获取新创建、 更新或删除应用程序，而无需执行的整个资源集的完全读取。 有关详细信息，请参阅使用增量查询。
localization_priority: Normal
ms.openlocfilehash: 594b7c05afdc8e3e3c89e8d2fb8e59f25cf4d4ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825471"
---
# <a name="application-delta"></a>应用程序： 增量

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

获取新创建、 更新或删除应用程序，而无需执行的整个资源集的完全读取。 有关详细信息，请参阅[使用增量查询](/graph/delta-query-overview)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.All Directory.Read.All |

## <a name="http-request"></a>HTTP 请求

若要开始跟踪的更改，您发出包含增量函数对应用程序资源请求。 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a>查询参数

跟踪更改会导致一个或多个**增量**函数调用的往返。 如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。 Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。 只需预先指定所需的任何查询参数一次。 在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 返回一个[状态标记](/graph/delta-query-overview)`deltaLink`指示完成的修订的往返相同的资源集合，以前**增量**函数调用的 URL。 保存并应用整个`deltaLink`下一轮更改跟踪集合的第一个请求中包括此令牌的 URL。|
| $skiptoken | string | 返回一个[状态标记](/graph/delta-query-overview)`nextLink`的以前的**增量**函数调用，指示有进一步的更改跟踪相同的资源集合中的 URL。 |

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。 

- 支持是有限的`$filter`:
  * 仅支持`$filter`按其 id 跟踪的特定资源，更改为表达式：`$filter=id+eq+{value}`或`$filter=id+eq+{value1}+or+id+eq+{value2}`。 您可以指定的 id 数受最大 URL 长度限制。


## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者&lt;令牌&gt;|
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应正文中的响应代码和[应用程序](../resources/application.md)集合的对象。 响应还包括 nextLink 或 deltaLink URL。 

- 如果`nextLink`返回 URL、 有会话中检索的数据的其他页。 应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。

- 如果`deltaLink`返回 URL、 没有更多有关要返回的资源的现有状态数据。 保留和使用`deltaLink`URL 将来了解到的资源的更改。

请参阅：</br>
- [使用增量查询](/graph/delta-query-overview)了解更多详细信息</br>
- [获取用户的增量更改](/graph/delta-query-users)获取示例请求。</br>

### <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```

##### <a name="response"></a>响应
注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
