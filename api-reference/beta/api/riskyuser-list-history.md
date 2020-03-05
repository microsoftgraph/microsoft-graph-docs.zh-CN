---
title: RiskyUser 的列表历史记录
description: 检索风险历史记录
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 927d9b623c4aa35d3b1314d2152d1efa91633cb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453896"
---
# <a name="list-history-of-riskyuser"></a><span data-ttu-id="4c2b8-103">RiskyUser 的列表历史记录</span><span class="sxs-lookup"><span data-stu-id="4c2b8-103">List history of riskyUser</span></span>

<span data-ttu-id="4c2b8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4c2b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c2b8-105">获取[riskyUser](../resources/riskyuser.md)资源的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-105">Get the risk history of a [riskyUser](../resources/riskyuser.md) resource.</span></span>

><span data-ttu-id="4c2b8-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c2b8-107">权限</span><span class="sxs-lookup"><span data-stu-id="4c2b8-107">Permissions</span></span>
<span data-ttu-id="4c2b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c2b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c2b8-110">Permission type</span></span>      | <span data-ttu-id="4c2b8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c2b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c2b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c2b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c2b8-113">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="4c2b8-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c2b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c2b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c2b8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-115">Not supported.</span></span>    |
|<span data-ttu-id="4c2b8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c2b8-116">Application</span></span> | <span data-ttu-id="4c2b8-117">IdentityRiskyUser、IdentityRiskUser 和所有</span><span class="sxs-lookup"><span data-stu-id="4c2b8-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c2b8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c2b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}/history
```


## <a name="request-headers"></a><span data-ttu-id="4c2b8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c2b8-119">Request headers</span></span>
| <span data-ttu-id="4c2b8-120">名称</span><span class="sxs-lookup"><span data-stu-id="4c2b8-120">Name</span></span>      |<span data-ttu-id="4c2b8-121">说明</span><span class="sxs-lookup"><span data-stu-id="4c2b8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c2b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c2b8-122">Authorization</span></span>  | <span data-ttu-id="4c2b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c2b8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c2b8-125">Request body</span></span>
<span data-ttu-id="4c2b8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c2b8-127">响应</span><span class="sxs-lookup"><span data-stu-id="4c2b8-127">Response</span></span>

<span data-ttu-id="4c2b8-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-128">If successful, this method returns a `200 OK` response code and a collection of [riskyUsersHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c2b8-129">示例</span><span class="sxs-lookup"><span data-stu-id="4c2b8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c2b8-130">请求</span><span class="sxs-lookup"><span data-stu-id="4c2b8-130">Request</span></span>
<span data-ttu-id="4c2b8-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c2b8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c2b8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userriskhitsory",
  "sampleKeys": ["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```
# <a name="c"></a>[<span data-ttu-id="4c2b8-133">C#</span><span class="sxs-lookup"><span data-stu-id="4c2b8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userriskhitsory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c2b8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c2b8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userriskhitsory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c2b8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c2b8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userriskhitsory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c2b8-136">响应</span><span class="sxs-lookup"><span data-stu-id="4c2b8-136">Response</span></span>
<span data-ttu-id="4c2b8-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4c2b8-137">Here is an example of the response.</span></span>
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

