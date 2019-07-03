---
title: RiskyUser 的列表历史记录
description: 检索风险历史记录
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 66da1eeaf8fc6c357be987e54a76b8d2adeb689d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447695"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="0cdc1-103">RiskyUser 的列表历史记录</span><span class="sxs-lookup"><span data-stu-id="0cdc1-103">List history of riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cdc1-104">获取[riskyUser](../resources/riskyuser.md)资源的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-104">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="0cdc1-105">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cdc1-106">权限</span><span class="sxs-lookup"><span data-stu-id="0cdc1-106">Permissions</span></span>
<span data-ttu-id="0cdc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cdc1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cdc1-109">Permission type</span></span>      | <span data-ttu-id="0cdc1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0cdc1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cdc1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cdc1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0cdc1-112">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="0cdc1-112">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="0cdc1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cdc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cdc1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-114">Not supported.</span></span>    |
|<span data-ttu-id="0cdc1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cdc1-115">Application</span></span> | <span data-ttu-id="0cdc1-116">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="0cdc1-116">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cdc1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cdc1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
```


## <a name="request-headers"></a><span data-ttu-id="0cdc1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cdc1-118">Request headers</span></span>
| <span data-ttu-id="0cdc1-119">名称</span><span class="sxs-lookup"><span data-stu-id="0cdc1-119">Name</span></span>      |<span data-ttu-id="0cdc1-120">说明</span><span class="sxs-lookup"><span data-stu-id="0cdc1-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0cdc1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cdc1-121">Authorization</span></span>  | <span data-ttu-id="0cdc1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cdc1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cdc1-124">Request body</span></span>
<span data-ttu-id="0cdc1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cdc1-126">响应</span><span class="sxs-lookup"><span data-stu-id="0cdc1-126">Response</span></span>

<span data-ttu-id="0cdc1-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-127">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cdc1-128">示例</span><span class="sxs-lookup"><span data-stu-id="0cdc1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cdc1-129">请求</span><span class="sxs-lookup"><span data-stu-id="0cdc1-129">Request</span></span>
<span data-ttu-id="0cdc1-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0cdc1-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0cdc1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0cdc1-132">C#</span><span class="sxs-lookup"><span data-stu-id="0cdc1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0cdc1-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="0cdc1-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0cdc1-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="0cdc1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0cdc1-135">响应</span><span class="sxs-lookup"><span data-stu-id="0cdc1-135">Response</span></span>
<span data-ttu-id="0cdc1-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0cdc1-136">Here is an example of the response.</span></span>
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

