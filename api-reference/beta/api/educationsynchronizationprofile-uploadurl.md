---
title: educationSynchronizationProfile： uploadUrl
description: 检索共享访问签名 (SAS) ，以将源文件上载到租户中特定学校数据同步配置文件的 Azure blob 存储。 SAS 令牌的有效期为 1 小时。
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dafd238642c49572ec776326584b75fd902b149a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109062"
---
# <a name="educationsynchronizationprofile-uploadurl"></a>educationSynchronizationProfile： uploadUrl

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索共享访问签名 (SAS) ，以将源文件上载到租户中特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 的 Azure blob 存储。 SAS 令牌的有效期为 1 小时。

上载 URL 仅为 CSV 数据 [提供程序提供](../resources/educationcsvdataprovider.md)。

> **注意：** 若要使用 SAS 令牌访问 blob 存储，请使用 Azure 存储 [SDK](https://github.com/search?q=org%3AAzure+azure-storage) 或 [AzCopy](/azure/storage/storage-use-azcopy)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限 |
|:-----------|:----------|
| 委派（工作或学校帐户） | EduAdministration.ReadWrite |
|委派 (个人 Microsoft 帐户|不支持。|
|应用程序|EduAdministration.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) 的响应代码和 SAS URL。

如果上一个请求仍在处理中，此方法将返回 指示当前已阻止 `409 Conflict` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)的上载。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-uploadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-uploadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-uploadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-uploadurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-educationsynchronizationprofile-uploadurl-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


