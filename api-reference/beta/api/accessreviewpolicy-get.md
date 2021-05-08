---
title: 获取 accessReviewPolicy
description: 读取 accessReviewPolicy 对象的属性和关系。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c2acf367b269e47271e3f3629ed05ce283201c1c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240986"
---
# <a name="get-accessreviewpolicy"></a><span data-ttu-id="cc81c-103">获取 accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="cc81c-103">Get accessReviewPolicy</span></span>
<span data-ttu-id="cc81c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc81c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc81c-105">读取 [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc81c-105">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc81c-106">权限</span><span class="sxs-lookup"><span data-stu-id="cc81c-106">Permissions</span></span>
<span data-ttu-id="cc81c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc81c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc81c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc81c-109">Permission type</span></span>|<span data-ttu-id="cc81c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc81c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc81c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc81c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cc81c-112">Policy.Read.All、Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="cc81c-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="cc81c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc81c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc81c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc81c-114">Not supported.</span></span>|
|<span data-ttu-id="cc81c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc81c-115">Application</span></span>|<span data-ttu-id="cc81c-116">Policy.Read.All、Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="cc81c-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc81c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc81c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/accessReviewPolicy
GET /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="cc81c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc81c-118">Request headers</span></span>
|<span data-ttu-id="cc81c-119">名称</span><span class="sxs-lookup"><span data-stu-id="cc81c-119">Name</span></span>|<span data-ttu-id="cc81c-120">说明</span><span class="sxs-lookup"><span data-stu-id="cc81c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cc81c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc81c-121">Authorization</span></span>|<span data-ttu-id="cc81c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc81c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc81c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc81c-124">Request body</span></span>
<span data-ttu-id="cc81c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc81c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc81c-126">响应</span><span class="sxs-lookup"><span data-stu-id="cc81c-126">Response</span></span>

<span data-ttu-id="cc81c-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc81c-127">If successful, this method returns a `200 OK` response code and an [accessReviewPolicy](../resources/accessreviewpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc81c-128">示例</span><span class="sxs-lookup"><span data-stu-id="cc81c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc81c-129">请求</span><span class="sxs-lookup"><span data-stu-id="cc81c-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cc81c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc81c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/accessReviewPolicy
```
# <a name="c"></a>[<span data-ttu-id="cc81c-131">C#</span><span class="sxs-lookup"><span data-stu-id="cc81c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc81c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc81c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc81c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc81c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc81c-134">Java</span><span class="sxs-lookup"><span data-stu-id="cc81c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cc81c-135">响应</span><span class="sxs-lookup"><span data-stu-id="cc81c-135">Response</span></span>
<span data-ttu-id="cc81c-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc81c-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```

### <a name="request"></a><span data-ttu-id="cc81c-137">请求</span><span class="sxs-lookup"><span data-stu-id="cc81c-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cc81c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc81c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
```
# <a name="c"></a>[<span data-ttu-id="cc81c-139">C#</span><span class="sxs-lookup"><span data-stu-id="cc81c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewpolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc81c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc81c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewpolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc81c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc81c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewpolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc81c-142">Java</span><span class="sxs-lookup"><span data-stu-id="cc81c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewpolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cc81c-143">响应</span><span class="sxs-lookup"><span data-stu-id="cc81c-143">Response</span></span>
<span data-ttu-id="cc81c-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc81c-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```
