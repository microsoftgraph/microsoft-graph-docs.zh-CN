---
title: reportRoot： getCredentialUserRegistrationCount
description: 报告您的组织中的多少用户为自助密码重置和多重身份验证（MFA）功能注册的用户的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 4b15f41298ae4c6e411d5a8de832f243b277d84e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454494"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="a5705-103">reportRoot： getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="a5705-103">reportRoot: getCredentialUserRegistrationCount</span></span>

<span data-ttu-id="a5705-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a5705-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5705-105">报告您的组织中的多少用户为自助密码重置和多重身份验证（MFA）功能注册的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a5705-105">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5705-106">权限</span><span class="sxs-lookup"><span data-stu-id="a5705-106">Permissions</span></span>

<span data-ttu-id="a5705-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5705-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5705-109">Permission type</span></span>                        | <span data-ttu-id="a5705-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5705-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5705-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5705-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5705-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5705-112">Reports.Read.All</span></span> |
| <span data-ttu-id="a5705-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5705-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5705-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5705-114">Not supported.</span></span> |
| <span data-ttu-id="a5705-115">应用</span><span class="sxs-lookup"><span data-stu-id="a5705-115">Application</span></span>                            | <span data-ttu-id="a5705-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5705-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5705-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5705-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="a5705-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5705-118">Request headers</span></span>

| <span data-ttu-id="a5705-119">名称</span><span class="sxs-lookup"><span data-stu-id="a5705-119">Name</span></span>          | <span data-ttu-id="a5705-120">说明</span><span class="sxs-lookup"><span data-stu-id="a5705-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a5705-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5705-121">Authorization</span></span> | <span data-ttu-id="a5705-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a5705-122">Bearer {token}</span></span> |
| <span data-ttu-id="a5705-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5705-123">Content-Type</span></span> | <span data-ttu-id="a5705-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a5705-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5705-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5705-125">Request body</span></span>

<span data-ttu-id="a5705-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5705-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5705-127">响应</span><span class="sxs-lookup"><span data-stu-id="a5705-127">Response</span></span>

<span data-ttu-id="a5705-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="a5705-128">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5705-129">示例</span><span class="sxs-lookup"><span data-stu-id="a5705-129">Examples</span></span>

<span data-ttu-id="a5705-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a5705-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a5705-131">请求</span><span class="sxs-lookup"><span data-stu-id="a5705-131">Request</span></span>

<span data-ttu-id="a5705-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a5705-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5705-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5705-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="c"></a>[<span data-ttu-id="a5705-134">C#</span><span class="sxs-lookup"><span data-stu-id="a5705-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5705-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5705-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5705-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5705-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5705-137">响应</span><span class="sxs-lookup"><span data-stu-id="a5705-137">Response</span></span>

<span data-ttu-id="a5705-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a5705-138">The following is an example of the response.</span></span>

> <span data-ttu-id="a5705-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a5705-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5705-140">所有属性都是从实际调用返回的。</span><span class="sxs-lookup"><span data-stu-id="a5705-140">All the properties are returned from an actual call.</span></span>

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
