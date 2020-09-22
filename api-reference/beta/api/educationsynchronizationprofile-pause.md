---
title: 暂停 educationSynchronizationProfile 上的同步
description: 暂停租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 003505dcfc00631f6d7ed9c40dbd9e4c8c3cebd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007201"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="7a587-103">暂停 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="7a587-103">Pause sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="7a587-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a587-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a587-105">暂停租户中特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 的同步。</span><span class="sxs-lookup"><span data-stu-id="7a587-105">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a587-106">权限</span><span class="sxs-lookup"><span data-stu-id="7a587-106">Permissions</span></span>
<span data-ttu-id="7a587-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a587-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a587-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a587-109">Permission type</span></span> | <span data-ttu-id="7a587-110">权限</span><span class="sxs-lookup"><span data-stu-id="7a587-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7a587-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a587-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a587-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a587-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="7a587-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="7a587-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7a587-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a587-114">Not supported.</span></span>|
|<span data-ttu-id="7a587-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a587-115">Application</span></span>|<span data-ttu-id="7a587-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a587-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a587-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a587-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="7a587-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a587-118">Request headers</span></span>
| <span data-ttu-id="7a587-119">名称</span><span class="sxs-lookup"><span data-stu-id="7a587-119">Name</span></span>       | <span data-ttu-id="7a587-120">类型</span><span class="sxs-lookup"><span data-stu-id="7a587-120">Type</span></span> | <span data-ttu-id="7a587-121">说明</span><span class="sxs-lookup"><span data-stu-id="7a587-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a587-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a587-122">Authorization</span></span>  | <span data-ttu-id="7a587-123">string</span><span class="sxs-lookup"><span data-stu-id="7a587-123">string</span></span>  | <span data-ttu-id="7a587-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a587-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a587-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a587-126">Request body</span></span>
<span data-ttu-id="7a587-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a587-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7a587-128">响应</span><span class="sxs-lookup"><span data-stu-id="7a587-128">Response</span></span>
<span data-ttu-id="7a587-129">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7a587-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7a587-130">示例</span><span class="sxs-lookup"><span data-stu-id="7a587-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a587-131">请求</span><span class="sxs-lookup"><span data-stu-id="7a587-131">Request</span></span>
<span data-ttu-id="7a587-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7a587-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a587-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a587-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="c"></a>[<span data-ttu-id="7a587-134">C#</span><span class="sxs-lookup"><span data-stu-id="7a587-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a587-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a587-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a587-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a587-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7a587-137">响应</span><span class="sxs-lookup"><span data-stu-id="7a587-137">Response</span></span>

<span data-ttu-id="7a587-138">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="7a587-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```http
HTTP/1.1 200 OK
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


