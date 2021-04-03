---
title: 列出 appConsentRequests
description: 检索 appConsentRequest 对象及其属性
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 82013c90f4a90be14bf6ba57750bf8cafc62e4e0
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508181"
---
# <a name="list-appconsentrequests"></a><span data-ttu-id="ecc5a-103">列出 appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="ecc5a-103">List appConsentRequests</span></span>
<span data-ttu-id="ecc5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecc5a-105">检索 [appConsentRequest](../resources/appconsentrequest.md) 对象及其属性。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-105">Retrieve [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecc5a-106">权限</span><span class="sxs-lookup"><span data-stu-id="ecc5a-106">Permissions</span></span>

<span data-ttu-id="ecc5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecc5a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecc5a-109">Permission type</span></span>|<span data-ttu-id="ecc5a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ecc5a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecc5a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecc5a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ecc5a-112">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecc5a-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="ecc5a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecc5a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecc5a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-114">Not supported.</span></span>|
|<span data-ttu-id="ecc5a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecc5a-115">Application</span></span>|<span data-ttu-id="ecc5a-116">ConsentRequest.Read.All、ConsentRequest.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecc5a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecc5a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecc5a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ecc5a-118">Optional query parameters</span></span>

<span data-ttu-id="ecc5a-119">此方法支持使用  `$select` 、 、 、 和 OData 查询参数 `$skip` `$top` `$filter` `$orderby` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ecc5a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecc5a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecc5a-121">Request headers</span></span>

|<span data-ttu-id="ecc5a-122">名称</span><span class="sxs-lookup"><span data-stu-id="ecc5a-122">Name</span></span>|<span data-ttu-id="ecc5a-123">说明</span><span class="sxs-lookup"><span data-stu-id="ecc5a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ecc5a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecc5a-124">Authorization</span></span>|<span data-ttu-id="ecc5a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecc5a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecc5a-127">Request body</span></span>

<span data-ttu-id="ecc5a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecc5a-129">响应</span><span class="sxs-lookup"><span data-stu-id="ecc5a-129">Response</span></span>

<span data-ttu-id="ecc5a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [appConsentRequest](../resources/appconsentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-130">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecc5a-131">示例</span><span class="sxs-lookup"><span data-stu-id="ecc5a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecc5a-132">请求</span><span class="sxs-lookup"><span data-stu-id="ecc5a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ecc5a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecc5a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests
```
# <a name="c"></a>[<span data-ttu-id="ecc5a-134">C#</span><span class="sxs-lookup"><span data-stu-id="ecc5a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appconsentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecc5a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecc5a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appconsentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecc5a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecc5a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appconsentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecc5a-137">Java</span><span class="sxs-lookup"><span data-stu-id="ecc5a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appconsentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecc5a-138">响应</span><span class="sxs-lookup"><span data-stu-id="ecc5a-138">Response</span></span>

<span data-ttu-id="ecc5a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ecc5a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```
