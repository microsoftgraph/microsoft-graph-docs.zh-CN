---
title: accessReviewHistoryInstance：generateDownloadUri
description: 生成可用于检索审阅历史记录数据的 URI。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 05634d27f98361fcf04d7ccd128a616c56f1fd6f
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698182"
---
# <a name="accessreviewhistoryinstance-generatedownloaduri"></a>accessReviewHistoryInstance：generateDownloadUri

命名空间：microsoft.graph

为 [accessReviewHistoryInstance](../resources/accessReviewHistoryInstance.md) 对象生成 **状态** 为 `done`的 URI。 每个 URI 可用于检索实例的审阅历史记录数据。 每个 URI 有效期为 24 小时，可以通过从 [accessReviewHistoryInstance](../resources/accessReviewHistoryInstance.md) 对象提取 **downloadUri** 属性来检索。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用|AccessReview.ReadWrite.All|

若要生成链接，登录用户必须是关联的评审历史记录定义的创建者，或分配了 *全局管理员* 或 *全局读者*[目录角色](/azure/active-directory/roles/permissions-reference)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identityGovernance/accessReviews/historyDefinitions/{accessReviewHistoryDefinitionId}/instances/{accessReviewHistoryInstanceId}/generateDownloadUri
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [accessReviewHistoryInstances](../resources/accessReviewHistoryInstance.md) 。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewhistoryinstance_generatedownloaduri"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38/instances/b2cb022f-b7e1-40f3-9854-c65a40861c38/generateDownloadUri
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewhistoryinstance-generatedownloaduri-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewhistoryinstance-generatedownloaduri-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewhistoryinstance-generatedownloaduri-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewhistoryinstance-generatedownloaduri-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accessreviewhistoryinstance-generatedownloaduri-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryInstance"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
    "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
    "reviewHistoryPeriodStartDateTime": "2000-06-19T08:00:00Z",
    "reviewHistoryPeriodEndDateTime": "2100-06-19T07:00:00Z",
    "status": "done",
    "runDateTime": "2022-01-20T17:46:54.6085806Z",
    "fulfilledDateTime": "2022-01-20T10:00:24.9114365-08:00",
    "downloadUri": "https://dfermconsolreportusc.blob.core.windows.net/df-erm-reports/Last months reviews for ELM-e642e792-9884-413d-9299-982b37bfe369.csv?skoid=fa04d013-9f36-4d7d-8b8e-7276fb3bd36e&sktid=33e01921-4d64-4f8c-a055-5bdaffd5e33d&skt=2022-01-20T18:03:59Z&ske=2022-01-20T18:05:59Z&sks=b&skv=2020-04-08&sv=2020-04-08&st=2022-01-20T18:04:01Z&se=2022-01-21T18:04:01Z&sr=b&sp=r&sig=...",
    "expiration": "2022-02-19T10:00:24.9114365-08:00"
}
```
