---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: 报告您的组织中的多少用户为自助密码重置和多重身份验证 (MFA) 功能注册的用户的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 88483b85cdf653ce14e5722a666b8ded8d279ff5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723187"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="decf0-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="decf0-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="decf0-104">报告您的组织中的多少用户为自助密码重置和多重身份验证 (MFA) 功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="decf0-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="decf0-105">权限</span><span class="sxs-lookup"><span data-stu-id="decf0-105">Permissions</span></span>

<span data-ttu-id="decf0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="decf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="decf0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="decf0-108">Permission type</span></span>                        | <span data-ttu-id="decf0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="decf0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="decf0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="decf0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="decf0-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="decf0-111">Reports.Read.All</span></span> |
| <span data-ttu-id="decf0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="decf0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="decf0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="decf0-113">Not supported.</span></span> |
| <span data-ttu-id="decf0-114">应用</span><span class="sxs-lookup"><span data-stu-id="decf0-114">Application</span></span>                            | <span data-ttu-id="decf0-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="decf0-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="decf0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="decf0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="decf0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="decf0-117">Request headers</span></span>

| <span data-ttu-id="decf0-118">名称</span><span class="sxs-lookup"><span data-stu-id="decf0-118">Name</span></span>          | <span data-ttu-id="decf0-119">说明</span><span class="sxs-lookup"><span data-stu-id="decf0-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="decf0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="decf0-120">Authorization</span></span> | <span data-ttu-id="decf0-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="decf0-121">Bearer {token}</span></span> |
| <span data-ttu-id="decf0-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="decf0-122">Content-Type</span></span> | <span data-ttu-id="decf0-123">application/json</span><span class="sxs-lookup"><span data-stu-id="decf0-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="decf0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="decf0-124">Request body</span></span>

<span data-ttu-id="decf0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="decf0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="decf0-126">响应</span><span class="sxs-lookup"><span data-stu-id="decf0-126">Response</span></span>

<span data-ttu-id="decf0-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和新的[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="decf0-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="decf0-128">示例</span><span class="sxs-lookup"><span data-stu-id="decf0-128">Examples</span></span>

<span data-ttu-id="decf0-129">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="decf0-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="decf0-130">请求</span><span class="sxs-lookup"><span data-stu-id="decf0-130">Request</span></span>

<span data-ttu-id="decf0-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="decf0-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="decf0-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="decf0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="decf0-133">C#</span><span class="sxs-lookup"><span data-stu-id="decf0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="decf0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="decf0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="decf0-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="decf0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="decf0-136">响应</span><span class="sxs-lookup"><span data-stu-id="decf0-136">Response</span></span>

<span data-ttu-id="decf0-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="decf0-137">The following is an example of the response.</span></span>

> <span data-ttu-id="decf0-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="decf0-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="decf0-139">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="decf0-139">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationCount)",
  "value": [
    {
      "id" : "id-value",
      "totalUserCount" : 23123,
      "userRegistrationCounts" :
      [
        { "userRegistrationStatus":"registered", 
          "userRegistationCount": 23423 }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUserRegistrationCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
