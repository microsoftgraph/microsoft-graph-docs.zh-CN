---
title: 获取 riskyUser
description: 检索**riskyUser**对象的属性和关系。
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: edbbfc520ac40ca5532f6d44c503c61dab808e5a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791109"
---
# <a name="get-riskyuser"></a><span data-ttu-id="55c1f-103">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="55c1f-103">Get riskyUser</span></span>

<span data-ttu-id="55c1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55c1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55c1f-105">检索**riskyUser**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55c1f-105">Retrieve the properties and relationships of a **riskyUser** object.</span></span>

><span data-ttu-id="55c1f-106">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="55c1f-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="55c1f-107">权限</span><span class="sxs-lookup"><span data-stu-id="55c1f-107">Permissions</span></span>
<span data-ttu-id="55c1f-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="55c1f-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="55c1f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55c1f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55c1f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="55c1f-110">Permission type</span></span>      | <span data-ttu-id="55c1f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55c1f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55c1f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55c1f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="55c1f-113">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="55c1f-113">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="55c1f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55c1f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55c1f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="55c1f-115">Not supported.</span></span>    |
|<span data-ttu-id="55c1f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="55c1f-116">Application</span></span> | <span data-ttu-id="55c1f-117">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="55c1f-117">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55c1f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55c1f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers/{id}
```


## <a name="request-headers"></a><span data-ttu-id="55c1f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="55c1f-119">Request headers</span></span>
| <span data-ttu-id="55c1f-120">名称</span><span class="sxs-lookup"><span data-stu-id="55c1f-120">Name</span></span>      |<span data-ttu-id="55c1f-121">说明</span><span class="sxs-lookup"><span data-stu-id="55c1f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55c1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55c1f-122">Authorization</span></span>  | <span data-ttu-id="55c1f-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="55c1f-123">Bearer {token}.</span></span> <span data-ttu-id="55c1f-124">Required.</span><span class="sxs-lookup"><span data-stu-id="55c1f-124">Required.</span></span> |
| <span data-ttu-id="55c1f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="55c1f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="55c1f-126">用于确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="55c1f-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="55c1f-127">可选。</span><span class="sxs-lookup"><span data-stu-id="55c1f-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55c1f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="55c1f-128">Request body</span></span>
<span data-ttu-id="55c1f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55c1f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55c1f-130">响应</span><span class="sxs-lookup"><span data-stu-id="55c1f-130">Response</span></span>

<span data-ttu-id="55c1f-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[riskyUser](../resources/riskyuser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="55c1f-131">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/riskyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55c1f-132">示例</span><span class="sxs-lookup"><span data-stu-id="55c1f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55c1f-133">请求</span><span class="sxs-lookup"><span data-stu-id="55c1f-133">Request</span></span>
<span data-ttu-id="55c1f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55c1f-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55c1f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="55c1f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="55c1f-136">C#</span><span class="sxs-lookup"><span data-stu-id="55c1f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55c1f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55c1f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55c1f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55c1f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55c1f-139">响应</span><span class="sxs-lookup"><span data-stu-id="55c1f-139">Response</span></span>
<span data-ttu-id="55c1f-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55c1f-140">Here is an example of the response.</span></span>
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

