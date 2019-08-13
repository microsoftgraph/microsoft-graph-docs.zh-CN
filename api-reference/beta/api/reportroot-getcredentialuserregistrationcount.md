---
title: 'reportRoot: getCredentialUserRegistrationCount'
description: 报告您的组织中的多少用户为自助密码重置和多重身份验证 (MFA) 功能注册的用户的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: bffd0856d158e3ffff897d160fd832d87c2028ed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308785"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="a8f5a-103">reportRoot: getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="a8f5a-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f5a-104">报告您的组织中的多少用户为自助密码重置和多重身份验证 (MFA) 功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8f5a-105">权限</span><span class="sxs-lookup"><span data-stu-id="a8f5a-105">Permissions</span></span>

<span data-ttu-id="a8f5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8f5a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8f5a-108">Permission type</span></span>                        | <span data-ttu-id="a8f5a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8f5a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a8f5a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8f5a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8f5a-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8f5a-111">Reports.Read.All</span></span> |
| <span data-ttu-id="a8f5a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8f5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8f5a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-113">Not supported.</span></span> |
| <span data-ttu-id="a8f5a-114">应用</span><span class="sxs-lookup"><span data-stu-id="a8f5a-114">Application</span></span>                            | <span data-ttu-id="a8f5a-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8f5a-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8f5a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8f5a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="a8f5a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8f5a-117">Request headers</span></span>

| <span data-ttu-id="a8f5a-118">名称</span><span class="sxs-lookup"><span data-stu-id="a8f5a-118">Name</span></span>          | <span data-ttu-id="a8f5a-119">说明</span><span class="sxs-lookup"><span data-stu-id="a8f5a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a8f5a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8f5a-120">Authorization</span></span> | <span data-ttu-id="a8f5a-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a8f5a-121">Bearer {token}</span></span> |
| <span data-ttu-id="a8f5a-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8f5a-122">Content-Type</span></span> | <span data-ttu-id="a8f5a-123">application/json</span><span class="sxs-lookup"><span data-stu-id="a8f5a-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8f5a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8f5a-124">Request body</span></span>

<span data-ttu-id="a8f5a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8f5a-126">响应</span><span class="sxs-lookup"><span data-stu-id="a8f5a-126">Response</span></span>

<span data-ttu-id="a8f5a-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和新的[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8f5a-128">示例</span><span class="sxs-lookup"><span data-stu-id="a8f5a-128">Examples</span></span>

<span data-ttu-id="a8f5a-129">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a8f5a-130">请求</span><span class="sxs-lookup"><span data-stu-id="a8f5a-130">Request</span></span>

<span data-ttu-id="a8f5a-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8f5a-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a8f5a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8f5a-133">C#</span><span class="sxs-lookup"><span data-stu-id="a8f5a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8f5a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8f5a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8f5a-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="a8f5a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a8f5a-136">Java</span><span class="sxs-lookup"><span data-stu-id="a8f5a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialuserregistrationcount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8f5a-137">响应</span><span class="sxs-lookup"><span data-stu-id="a8f5a-137">Response</span></span>

<span data-ttu-id="a8f5a-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-138">The following is an example of the response.</span></span>

> <span data-ttu-id="a8f5a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a8f5a-140">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="a8f5a-140">All the properties are returned from an actual call.</span></span>

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
