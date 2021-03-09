---
title: 删除 educationSynchronizationProfile
description: 根据标识符删除租户中的学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2cc7d03b406888022fc8bab935af2b5118357c0c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574277"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="62270-103">删除 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="62270-103">Delete a educationSynchronizationProfile</span></span>

<span data-ttu-id="62270-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62270-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62270-105">根据 [标识符删除租户](../resources/educationsynchronizationprofile.md) 中的学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="62270-105">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="62270-106">权限</span><span class="sxs-lookup"><span data-stu-id="62270-106">Permissions</span></span>
<span data-ttu-id="62270-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62270-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62270-109">Permission type</span></span> | <span data-ttu-id="62270-110">权限</span><span class="sxs-lookup"><span data-stu-id="62270-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="62270-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62270-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62270-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62270-112">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="62270-113">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62270-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="62270-114">请求标头</span><span class="sxs-lookup"><span data-stu-id="62270-114">Request headers</span></span>
| <span data-ttu-id="62270-115">名称</span><span class="sxs-lookup"><span data-stu-id="62270-115">Name</span></span>       | <span data-ttu-id="62270-116">类型</span><span class="sxs-lookup"><span data-stu-id="62270-116">Type</span></span> | <span data-ttu-id="62270-117">说明</span><span class="sxs-lookup"><span data-stu-id="62270-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="62270-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="62270-118">Authorization</span></span>  | <span data-ttu-id="62270-119">string</span><span class="sxs-lookup"><span data-stu-id="62270-119">string</span></span>  | <span data-ttu-id="62270-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62270-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="62270-122">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="62270-122">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="62270-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="62270-123">Not supported.</span></span>|
|<span data-ttu-id="62270-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="62270-124">Application</span></span>|<span data-ttu-id="62270-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="62270-125">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62270-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="62270-126">Request body</span></span>
<span data-ttu-id="62270-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62270-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="62270-128">响应</span><span class="sxs-lookup"><span data-stu-id="62270-128">Response</span></span>
<span data-ttu-id="62270-129">如果成功，此方法将返回 `202 Accepted` 响应代码，并且不会返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="62270-129">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="62270-130">示例</span><span class="sxs-lookup"><span data-stu-id="62270-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62270-131">请求</span><span class="sxs-lookup"><span data-stu-id="62270-131">Request</span></span>
<span data-ttu-id="62270-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62270-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62270-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="62270-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="62270-134">C#</span><span class="sxs-lookup"><span data-stu-id="62270-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62270-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62270-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62270-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62270-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62270-137">Java</span><span class="sxs-lookup"><span data-stu-id="62270-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="62270-138">响应</span><span class="sxs-lookup"><span data-stu-id="62270-138">Response</span></span>
<span data-ttu-id="62270-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="62270-139">Here is an example of the response.</span></span>
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


