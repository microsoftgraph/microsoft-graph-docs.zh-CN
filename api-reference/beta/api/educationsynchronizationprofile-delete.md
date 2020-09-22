---
title: 删除 educationSynchronizationProfile
description: 根据标识符删除租户中的学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39bc4909e63e6e7ff908481873f32324703bf549
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991255"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="55008-103">删除 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="55008-103">Delete a educationSynchronizationProfile</span></span>

<span data-ttu-id="55008-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55008-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55008-105">根据标识符删除租户中的学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 。</span><span class="sxs-lookup"><span data-stu-id="55008-105">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="55008-106">权限</span><span class="sxs-lookup"><span data-stu-id="55008-106">Permissions</span></span>
<span data-ttu-id="55008-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55008-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55008-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="55008-109">Permission type</span></span> | <span data-ttu-id="55008-110">权限</span><span class="sxs-lookup"><span data-stu-id="55008-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="55008-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55008-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55008-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55008-112">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55008-113">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55008-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="55008-114">请求标头</span><span class="sxs-lookup"><span data-stu-id="55008-114">Request headers</span></span>
| <span data-ttu-id="55008-115">名称</span><span class="sxs-lookup"><span data-stu-id="55008-115">Name</span></span>       | <span data-ttu-id="55008-116">类型</span><span class="sxs-lookup"><span data-stu-id="55008-116">Type</span></span> | <span data-ttu-id="55008-117">说明</span><span class="sxs-lookup"><span data-stu-id="55008-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="55008-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="55008-118">Authorization</span></span>  | <span data-ttu-id="55008-119">string</span><span class="sxs-lookup"><span data-stu-id="55008-119">string</span></span>  | <span data-ttu-id="55008-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55008-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="55008-122">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="55008-122">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="55008-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="55008-123">Not supported.</span></span>|
|<span data-ttu-id="55008-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="55008-124">Application</span></span>|<span data-ttu-id="55008-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="55008-125">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55008-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="55008-126">Request body</span></span>
<span data-ttu-id="55008-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55008-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="55008-128">响应</span><span class="sxs-lookup"><span data-stu-id="55008-128">Response</span></span>
<span data-ttu-id="55008-129">如果成功，此方法将返回 `202 Accepted` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="55008-129">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="55008-130">示例</span><span class="sxs-lookup"><span data-stu-id="55008-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55008-131">请求</span><span class="sxs-lookup"><span data-stu-id="55008-131">Request</span></span>
<span data-ttu-id="55008-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55008-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55008-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="55008-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="55008-134">C#</span><span class="sxs-lookup"><span data-stu-id="55008-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55008-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55008-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55008-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55008-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55008-137">响应</span><span class="sxs-lookup"><span data-stu-id="55008-137">Response</span></span>
<span data-ttu-id="55008-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55008-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


