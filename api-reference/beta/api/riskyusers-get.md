---
title: 获取 riskyUser
description: 检索**riskyUser**对象的属性和关系。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82eb470bf977321def10b66c0ec8199a3bec07a5
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639019"
---
# <a name="get-riskyuser"></a><span data-ttu-id="2fb7c-103">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="2fb7c-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fb7c-104">检索**riskyUser**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="2fb7c-105">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fb7c-106">权限</span><span class="sxs-lookup"><span data-stu-id="2fb7c-106">Permissions</span></span>
<span data-ttu-id="2fb7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb7c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fb7c-109">Permission type</span></span>      | <span data-ttu-id="2fb7c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fb7c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fb7c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fb7c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2fb7c-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fb7c-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="2fb7c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fb7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fb7c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-114">Not supported.</span></span>    |
|<span data-ttu-id="2fb7c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fb7c-115">Application</span></span> | <span data-ttu-id="2fb7c-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fb7c-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fb7c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fb7c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="2fb7c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fb7c-118">Request headers</span></span>
| <span data-ttu-id="2fb7c-119">名称</span><span class="sxs-lookup"><span data-stu-id="2fb7c-119">Name</span></span>      |<span data-ttu-id="2fb7c-120">说明</span><span class="sxs-lookup"><span data-stu-id="2fb7c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2fb7c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fb7c-121">Authorization</span></span>  | <span data-ttu-id="2fb7c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fb7c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2fb7c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2fb7c-125">用于确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="2fb7c-126">可选。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb7c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fb7c-127">Request body</span></span>
<span data-ttu-id="2fb7c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fb7c-129">响应</span><span class="sxs-lookup"><span data-stu-id="2fb7c-129">Response</span></span>

<span data-ttu-id="2fb7c-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskyUser](../resources/riskyUser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fb7c-131">示例</span><span class="sxs-lookup"><span data-stu-id="2fb7c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fb7c-132">请求</span><span class="sxs-lookup"><span data-stu-id="2fb7c-132">Request</span></span>
<span data-ttu-id="2fb7c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
##### <a name="response"></a><span data-ttu-id="2fb7c-134">响应</span><span class="sxs-lookup"><span data-stu-id="2fb7c-134">Response</span></span>
<span data-ttu-id="2fb7c-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2fb7c-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
  "isGuest": true,
  "isProcessing": true,
  "isDeleted": true,
  "riskDetail": "adminConfirmedSigninCompromised",
  "riskLevel": "high",
  "riskState": "atRisk",
  "userDisplayName": "Alex Wilbur",
  "userPrincipalName": "alexw@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2fb7c-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2fb7c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2fb7c-137">语言</span><span class="sxs-lookup"><span data-stu-id="2fb7c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fb7c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fb7c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_riskyuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

