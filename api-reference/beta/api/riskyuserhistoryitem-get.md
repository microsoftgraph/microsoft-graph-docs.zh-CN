---
title: 获取 riskyUser 的历史记录项
description: 获取 riskyUser 对象的历史记录项。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db2743525ecb291f4d07afe6ea6ce379b938bfe4
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863521"
---
# <a name="get-riskyuserhistoryitem"></a><span data-ttu-id="6686d-103">获取 riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="6686d-103">Get riskyUserHistoryItem</span></span>

<span data-ttu-id="6686d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6686d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6686d-105">获取[riskyUser](../resources/riskyuser.md)的[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6686d-105">Get a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object of a [riskyUser](../resources/riskyuser.md).</span></span>

><span data-ttu-id="6686d-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="6686d-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="6686d-107">权限</span><span class="sxs-lookup"><span data-stu-id="6686d-107">Permissions</span></span>
<span data-ttu-id="6686d-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6686d-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6686d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6686d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6686d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6686d-110">Permission type</span></span>      | <span data-ttu-id="6686d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6686d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6686d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6686d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6686d-113">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="6686d-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="6686d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6686d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6686d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6686d-115">Not supported.</span></span>    |
|<span data-ttu-id="6686d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6686d-116">Application</span></span> | <span data-ttu-id="6686d-117">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="6686d-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6686d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6686d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{userid}/history/{id}
GET /identityProtection/riskyUsers/{userid}/history/{id}
```


## <a name="request-headers"></a><span data-ttu-id="6686d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6686d-119">Request headers</span></span>
| <span data-ttu-id="6686d-120">名称</span><span class="sxs-lookup"><span data-stu-id="6686d-120">Name</span></span>      |<span data-ttu-id="6686d-121">说明</span><span class="sxs-lookup"><span data-stu-id="6686d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6686d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6686d-122">Authorization</span></span>  | <span data-ttu-id="6686d-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6686d-123">Bearer {token}.</span></span> <span data-ttu-id="6686d-124">Required.</span><span class="sxs-lookup"><span data-stu-id="6686d-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6686d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6686d-125">Request body</span></span>
<span data-ttu-id="6686d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6686d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6686d-127">响应</span><span class="sxs-lookup"><span data-stu-id="6686d-127">Response</span></span>

<span data-ttu-id="6686d-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6686d-128">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6686d-129">示例</span><span class="sxs-lookup"><span data-stu-id="6686d-129">Examples</span></span>
### <a name="example-1-get-history-of-a-risky-user"></a><span data-ttu-id="6686d-130">示例1：获取有风险的用户的历史记录</span><span class="sxs-lookup"><span data-stu-id="6686d-130">Example 1: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="6686d-131">请求</span><span class="sxs-lookup"><span data-stu-id="6686d-131">Request</span></span>
<span data-ttu-id="6686d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6686d-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6686d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6686d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="6686d-134">C#</span><span class="sxs-lookup"><span data-stu-id="6686d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6686d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6686d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6686d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6686d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6686d-137">响应</span><span class="sxs-lookup"><span data-stu-id="6686d-137">Response</span></span>
<span data-ttu-id="6686d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6686d-138">Here is an example of the response.</span></span>
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

### <a name="example-2-get-history-of-a-risky-user"></a><span data-ttu-id="6686d-139">示例2：获取有风险的用户的历史记录</span><span class="sxs-lookup"><span data-stu-id="6686d-139">Example 2: Get history of a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="6686d-140">请求</span><span class="sxs-lookup"><span data-stu-id="6686d-140">Request</span></span>
<span data-ttu-id="6686d-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6686d-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6686d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6686d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser_historyitem",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69
```
# <a name="c"></a>[<span data-ttu-id="6686d-143">C#</span><span class="sxs-lookup"><span data-stu-id="6686d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-historyitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6686d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6686d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-historyitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6686d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6686d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6686d-146">响应</span><span class="sxs-lookup"><span data-stu-id="6686d-146">Response</span></span>
<span data-ttu-id="6686d-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6686d-147">Here is an example of the response.</span></span>
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

