---
title: 'directoryObject: getByIds'
description: '返回 ID 列表中指定的目录对象。 '
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4ff5791cb14806f06ca6ae1c7895ce8009542eb3
ms.sourcegitcommit: 11be55b40804b07f4c422f09f601afa97c7d31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2021
ms.locfileid: "60256422"
---
# <a name="directoryobject-getbyids"></a>directoryObject: getByIds

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

返回 ID 列表中指定的目录对象。

该函数的一些常见用途是：

* 将返回 ID 集合的函数（例如 [getMemberObjects](./directoryobject-getmemberobjects.md) 或 [getMemberGroups](./directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。
* 将应用程序保存在外部存储中的 ID 解析到其后备目录对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。 |
| Content-type  | application/json. Required.  |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数   | 类型 |说明|
|:---------------|:--------|:----------|
|ids|String collection| 要返回其对象的 ID 集合。 ID 是 GUID，由字符串表示。 最多可以指定 1000 个 ID。 |
|types|String collection| 指定要搜索的资源集合集的资源类型集合。 如果未指定，则默认为 [directoryObject](../resources/directoryobject.md)，其包含目录中定义的所有资源类型。 可以在集合中指定从[directoryObject](../resources/directoryobject.md)派生的任何对象;例如[：user、group](../resources/user.md)[和设备](../resources/device.md)对象。 [](../resources/group.md) <br/><br/>若要搜索对[云解决方案提供商](https://partner.microsoft.com/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md)。 如果未指定，则默认为 [directoryObject](../resources/directoryobject.md)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/cloud-solution-provider)合作伙伴组织的引用除外。 </br><br/> 这些值不区分大小写。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
