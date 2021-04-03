---
title: appConsentRequest：filterByCurrentUser
description: 检索当前用户是审阅者的 appConsentRequests。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cf1e0dcf104c540f8a223678adfc2e9eb8fe432e
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508263"
---
# <a name="appconsentrequest-filterbycurrentuser"></a><span data-ttu-id="d57f1-103">appConsentRequest：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="d57f1-103">appConsentRequest: filterByCurrentUser</span></span>

<span data-ttu-id="d57f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d57f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d57f1-105">检索 [appConsentRequests，](../resources/appconsentrequest.md) 当前用户是审阅者，userConsentRequest 的状态为 `InProgress` 。</span><span class="sxs-lookup"><span data-stu-id="d57f1-105">Retrieve [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d57f1-106">权限</span><span class="sxs-lookup"><span data-stu-id="d57f1-106">Permissions</span></span>

<span data-ttu-id="d57f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d57f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d57f1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d57f1-109">Permission type</span></span>|<span data-ttu-id="d57f1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d57f1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d57f1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d57f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d57f1-112">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d57f1-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="d57f1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d57f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d57f1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d57f1-114">Not supported.</span></span>|
|<span data-ttu-id="d57f1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d57f1-115">Application</span></span>|<span data-ttu-id="d57f1-116">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d57f1-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d57f1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d57f1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="d57f1-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="d57f1-118">Function parameters</span></span>

<span data-ttu-id="d57f1-119">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="d57f1-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d57f1-120">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="d57f1-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d57f1-121">参数</span><span class="sxs-lookup"><span data-stu-id="d57f1-121">Parameter</span></span>|<span data-ttu-id="d57f1-122">类型</span><span class="sxs-lookup"><span data-stu-id="d57f1-122">Type</span></span>|<span data-ttu-id="d57f1-123">说明</span><span class="sxs-lookup"><span data-stu-id="d57f1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d57f1-124">on</span><span class="sxs-lookup"><span data-stu-id="d57f1-124">on</span></span>|<span data-ttu-id="d57f1-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="d57f1-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="d57f1-126">筛选以查询当前用户是审阅者的 appConsentRequests。</span><span class="sxs-lookup"><span data-stu-id="d57f1-126">Filter to query appConsentRequests for which the current user is a reviewer.</span></span> <span data-ttu-id="d57f1-127">允许的值为 `reviewer` 。</span><span class="sxs-lookup"><span data-stu-id="d57f1-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="d57f1-128">必填。</span><span class="sxs-lookup"><span data-stu-id="d57f1-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="d57f1-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d57f1-129">Optional query parameters</span></span>

<span data-ttu-id="d57f1-130">此函数需要  `$filter` OData 查询参数以返回状态为 的 [userConsentRequests](../resources/userconsentrequest.md) 集合 `InProgress` 。</span><span class="sxs-lookup"><span data-stu-id="d57f1-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequests](../resources/userconsentrequest.md) for which the status is `InProgress`.</span></span> <span data-ttu-id="d57f1-131">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d57f1-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d57f1-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="d57f1-132">Request headers</span></span>

|<span data-ttu-id="d57f1-133">名称</span><span class="sxs-lookup"><span data-stu-id="d57f1-133">Name</span></span>|<span data-ttu-id="d57f1-134">说明</span><span class="sxs-lookup"><span data-stu-id="d57f1-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d57f1-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="d57f1-135">Authorization</span></span>|<span data-ttu-id="d57f1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d57f1-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d57f1-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="d57f1-138">Request body</span></span>

<span data-ttu-id="d57f1-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d57f1-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d57f1-140">响应</span><span class="sxs-lookup"><span data-stu-id="d57f1-140">Response</span></span>

<span data-ttu-id="d57f1-141">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [appConsentRequest](../resources/appconsentrequest.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d57f1-141">If successful, this function returns a `200 OK` response code and a [appConsentRequest](../resources/appconsentrequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d57f1-142">示例</span><span class="sxs-lookup"><span data-stu-id="d57f1-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d57f1-143">请求</span><span class="sxs-lookup"><span data-stu-id="d57f1-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d57f1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d57f1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```
# <a name="c"></a>[<span data-ttu-id="d57f1-145">C#</span><span class="sxs-lookup"><span data-stu-id="d57f1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/appconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d57f1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d57f1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/appconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d57f1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d57f1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/appconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d57f1-148">Java</span><span class="sxs-lookup"><span data-stu-id="d57f1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/appconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d57f1-149">响应</span><span class="sxs-lookup"><span data-stu-id="d57f1-149">Response</span></span>

<span data-ttu-id="d57f1-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d57f1-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(appConsentRequest)",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "consentType": "Dynamic",
      "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

