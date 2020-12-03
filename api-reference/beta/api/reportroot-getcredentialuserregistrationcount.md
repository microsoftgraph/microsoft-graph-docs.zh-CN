---
title: reportRoot： getCredentialUserRegistrationCount
description: 报告您的组织中的多少用户为自助服务密码重置和多重身份验证 (MFA) 功能注册的用户的当前状态。
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 8fd2b2d950055eb778242664b95e0eaafe95dbc9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523054"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="c2796-103">reportRoot： getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="c2796-103">reportRoot: getCredentialUserRegistrationCount</span></span>

<span data-ttu-id="c2796-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2796-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2796-105">报告您的组织中的多少用户为自助服务密码重置和多重身份验证 (MFA) 功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c2796-105">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2796-106">权限</span><span class="sxs-lookup"><span data-stu-id="c2796-106">Permissions</span></span>

<span data-ttu-id="c2796-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2796-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2796-109">Permission type</span></span>                        | <span data-ttu-id="c2796-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2796-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2796-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2796-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2796-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2796-112">Reports.Read.All</span></span> |
| <span data-ttu-id="c2796-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2796-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2796-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2796-114">Not supported.</span></span> |
| <span data-ttu-id="c2796-115">应用</span><span class="sxs-lookup"><span data-stu-id="c2796-115">Application</span></span>                            | <span data-ttu-id="c2796-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2796-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2796-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2796-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="c2796-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2796-118">Request headers</span></span>

| <span data-ttu-id="c2796-119">名称</span><span class="sxs-lookup"><span data-stu-id="c2796-119">Name</span></span>          | <span data-ttu-id="c2796-120">说明</span><span class="sxs-lookup"><span data-stu-id="c2796-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c2796-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2796-121">Authorization</span></span> | <span data-ttu-id="c2796-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c2796-122">Bearer {token}</span></span> |
| <span data-ttu-id="c2796-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2796-123">Content-Type</span></span> | <span data-ttu-id="c2796-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c2796-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2796-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2796-125">Request body</span></span>

<span data-ttu-id="c2796-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2796-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2796-127">响应</span><span class="sxs-lookup"><span data-stu-id="c2796-127">Response</span></span>

<span data-ttu-id="c2796-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的 [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c2796-128">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2796-129">示例</span><span class="sxs-lookup"><span data-stu-id="c2796-129">Examples</span></span>

<span data-ttu-id="c2796-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c2796-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c2796-131">请求</span><span class="sxs-lookup"><span data-stu-id="c2796-131">Request</span></span>

<span data-ttu-id="c2796-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2796-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2796-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2796-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="c"></a>[<span data-ttu-id="c2796-134">C#</span><span class="sxs-lookup"><span data-stu-id="c2796-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2796-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2796-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2796-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2796-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2796-137">Java</span><span class="sxs-lookup"><span data-stu-id="c2796-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialuserregistrationcount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2796-138">响应</span><span class="sxs-lookup"><span data-stu-id="c2796-138">Response</span></span>

<span data-ttu-id="c2796-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c2796-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c2796-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c2796-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c2796-141">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="c2796-141">All the properties are returned from an actual call.</span></span>

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


