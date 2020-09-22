---
title: RiskyUser 的列表历史记录
description: 检索风险历史记录
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cd01599ac46a1fdac6f4c34522cea41c9cee30e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994475"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="f97b6-103">RiskyUser 的列表历史记录</span><span class="sxs-lookup"><span data-stu-id="f97b6-103">List history of riskyUser</span></span>

<span data-ttu-id="f97b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f97b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f97b6-105">获取 [riskyUser](../resources/riskyuser.md) 资源的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="f97b6-105">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="f97b6-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="f97b6-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="f97b6-107">权限</span><span class="sxs-lookup"><span data-stu-id="f97b6-107">Permissions</span></span>
<span data-ttu-id="f97b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f97b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f97b6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f97b6-110">Permission type</span></span>      | <span data-ttu-id="f97b6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f97b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f97b6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f97b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f97b6-113">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="f97b6-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="f97b6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f97b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f97b6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f97b6-115">Not supported.</span></span>    |
|<span data-ttu-id="f97b6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f97b6-116">Application</span></span> | <span data-ttu-id="f97b6-117">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="f97b6-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f97b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f97b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
GET /identityProtection/riskyUsers/{id}/history/
```


## <a name="request-headers"></a><span data-ttu-id="f97b6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f97b6-119">Request headers</span></span>
| <span data-ttu-id="f97b6-120">名称</span><span class="sxs-lookup"><span data-stu-id="f97b6-120">Name</span></span>      |<span data-ttu-id="f97b6-121">说明</span><span class="sxs-lookup"><span data-stu-id="f97b6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f97b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f97b6-122">Authorization</span></span>  | <span data-ttu-id="f97b6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f97b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f97b6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f97b6-125">Request body</span></span>
<span data-ttu-id="f97b6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f97b6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f97b6-127">响应</span><span class="sxs-lookup"><span data-stu-id="f97b6-127">Response</span></span>

<span data-ttu-id="f97b6-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f97b6-128">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f97b6-129">示例</span><span class="sxs-lookup"><span data-stu-id="f97b6-129">Examples</span></span>
### <a name="example-1-list-history-of-a-specific-user"></a><span data-ttu-id="f97b6-130">示例1：列出特定用户的历史记录</span><span class="sxs-lookup"><span data-stu-id="f97b6-130">Example 1: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="f97b6-131">请求</span><span class="sxs-lookup"><span data-stu-id="f97b6-131">Request</span></span>
<span data-ttu-id="f97b6-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f97b6-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f97b6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f97b6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="f97b6-134">C#</span><span class="sxs-lookup"><span data-stu-id="f97b6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f97b6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f97b6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f97b6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f97b6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f97b6-137">响应</span><span class="sxs-lookup"><span data-stu-id="f97b6-137">Response</span></span>
<span data-ttu-id="f97b6-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f97b6-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers('41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')/history",
    "value": [
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
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901009342322587",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "high",
            "riskState": "atRisk",
            "riskDetail": "none",
            "riskLastUpdatedDateTime": "2019-04-05T22:31:27Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": null,
            "activity": {
                "eventTypes": [
                    "anonymizedIPAddress"
                ],
                "detail": null
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901020140973557",
            "isDeleted": false,
            "isGuest": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-04-05T23:00:14.0973557Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        }
    ]
}

```
### <a name="example-2-list-history-of-a-specific-user"></a><span data-ttu-id="f97b6-139">示例2：列出特定用户的历史记录</span><span class="sxs-lookup"><span data-stu-id="f97b6-139">Example 2: List history of a specific user</span></span>
#### <a name="request"></a><span data-ttu-id="f97b6-140">请求</span><span class="sxs-lookup"><span data-stu-id="f97b6-140">Request</span></span>
<span data-ttu-id="f97b6-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f97b6-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f97b6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f97b6-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="f97b6-143">C#</span><span class="sxs-lookup"><span data-stu-id="f97b6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f97b6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f97b6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f97b6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f97b6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f97b6-146">响应</span><span class="sxs-lookup"><span data-stu-id="f97b6-146">Response</span></span>
<span data-ttu-id="f97b6-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f97b6-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers('41a31b00-3b3b-42d9-8f1c-6d4f14e74c69')/history",
    "value": [
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "isDeleted": false,
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
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901009342322587",
            "isDeleted": false,
            "isProcessing": false,
            "riskLevel": "high",
            "riskState": "atRisk",
            "riskDetail": "none",
            "riskLastUpdatedDateTime": "2019-04-05T22:31:27Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": null,
            "activity": {
                "eventTypes": [
                    "anonymizedIPAddress"
                ],
                "detail": null
            }
        },
        {
            "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69636901020140973557",
            "isDeleted": false,
            "isProcessing": false,
            "riskLevel": "none",
            "riskState": "remediated",
            "riskDetail": "userPerformedSecuredPasswordReset",
            "riskLastUpdatedDateTime": "2019-04-05T23:00:14.0973557Z",
            "userDisplayName": "Allan Deyoung",
            "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
            "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
            "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
            "activity": {
                "eventTypes": [],
                "detail": "userPerformedSecuredPasswordReset"
            }
        }
    ]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user risk history",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



