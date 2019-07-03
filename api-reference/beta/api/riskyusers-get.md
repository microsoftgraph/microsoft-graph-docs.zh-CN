---
title: 获取 riskyUser
description: 检索**riskyUser**对象的属性和关系。
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f40bbfad74860d17fbe8259405cc5b6637a96119
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450378"
---
# <a name="get-riskyuser"></a><span data-ttu-id="1284a-103">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="1284a-103">Get riskyUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1284a-104">检索**riskyUser**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1284a-104">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="1284a-105">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="1284a-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="1284a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1284a-106">Permissions</span></span>
<span data-ttu-id="1284a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1284a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1284a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1284a-109">Permission type</span></span>      | <span data-ttu-id="1284a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1284a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1284a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1284a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1284a-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1284a-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="1284a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1284a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1284a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1284a-114">Not supported.</span></span>    |
|<span data-ttu-id="1284a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1284a-115">Application</span></span> | <span data-ttu-id="1284a-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="1284a-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1284a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1284a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="1284a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1284a-118">Request headers</span></span>
| <span data-ttu-id="1284a-119">名称</span><span class="sxs-lookup"><span data-stu-id="1284a-119">Name</span></span>      |<span data-ttu-id="1284a-120">说明</span><span class="sxs-lookup"><span data-stu-id="1284a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1284a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1284a-121">Authorization</span></span>  | <span data-ttu-id="1284a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1284a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1284a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1284a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1284a-125">用于确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="1284a-125">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="1284a-126">可选。</span><span class="sxs-lookup"><span data-stu-id="1284a-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1284a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1284a-127">Request body</span></span>
<span data-ttu-id="1284a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1284a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1284a-129">响应</span><span class="sxs-lookup"><span data-stu-id="1284a-129">Response</span></span>

<span data-ttu-id="1284a-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskyUser](../resources/riskyuser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1284a-130">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1284a-131">示例</span><span class="sxs-lookup"><span data-stu-id="1284a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1284a-132">请求</span><span class="sxs-lookup"><span data-stu-id="1284a-132">Request</span></span>
<span data-ttu-id="1284a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1284a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1284a-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1284a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```http
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1284a-135">C#</span><span class="sxs-lookup"><span data-stu-id="1284a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1284a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1284a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1284a-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="1284a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1284a-138">响应</span><span class="sxs-lookup"><span data-stu-id="1284a-138">Response</span></span>
<span data-ttu-id="1284a-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1284a-139">Here is an example of the response.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

