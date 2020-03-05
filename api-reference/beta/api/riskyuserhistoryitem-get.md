---
title: 获取 riskyUser 的历史记录项
description: 获取 riskyUser 对象的历史记录项。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44839c87819f9be5fd857eebe2787bffcf8dc0ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453889"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="ba13d-103">获取 riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="ba13d-103">Get riskyUserHistoryItem</span></span>

<span data-ttu-id="ba13d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ba13d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba13d-105">获取[riskyUser](../resources/riskyuser.md)的[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ba13d-105">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="ba13d-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="ba13d-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba13d-107">权限</span><span class="sxs-lookup"><span data-stu-id="ba13d-107">Permissions</span></span>
<span data-ttu-id="ba13d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba13d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba13d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba13d-110">Permission type</span></span>      | <span data-ttu-id="ba13d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba13d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba13d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba13d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba13d-113">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="ba13d-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba13d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba13d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba13d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba13d-115">Not supported.</span></span>    |
|<span data-ttu-id="ba13d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba13d-116">Application</span></span> | <span data-ttu-id="ba13d-117">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="ba13d-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba13d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba13d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="ba13d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba13d-119">Request headers</span></span>
| <span data-ttu-id="ba13d-120">名称</span><span class="sxs-lookup"><span data-stu-id="ba13d-120">Name</span></span>      |<span data-ttu-id="ba13d-121">说明</span><span class="sxs-lookup"><span data-stu-id="ba13d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba13d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba13d-122">Authorization</span></span>  | <span data-ttu-id="ba13d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba13d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba13d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba13d-125">Request body</span></span>
<span data-ttu-id="ba13d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba13d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba13d-127">响应</span><span class="sxs-lookup"><span data-stu-id="ba13d-127">Response</span></span>

<span data-ttu-id="ba13d-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ba13d-128">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba13d-129">示例</span><span class="sxs-lookup"><span data-stu-id="ba13d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba13d-130">请求</span><span class="sxs-lookup"><span data-stu-id="ba13d-130">Request</span></span>
<span data-ttu-id="ba13d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba13d-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba13d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba13d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="ba13d-133">C#</span><span class="sxs-lookup"><span data-stu-id="ba13d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba13d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba13d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba13d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba13d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ba13d-136">响应</span><span class="sxs-lookup"><span data-stu-id="ba13d-136">Response</span></span>
<span data-ttu-id="ba13d-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ba13d-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
        "eventTypes": [],
        "detail": "userPerformedSecuredPasswordReset"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUserHistoryItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

