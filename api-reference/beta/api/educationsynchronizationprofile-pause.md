---
title: 暂停 educationSynchronizationProfile 上的同步
description: 暂停租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 79f184d0816fa3c9d3e5a9dd58737b8cf0ab657c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415993"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="332c7-103">暂停 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="332c7-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="332c7-104">暂停租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="332c7-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="332c7-105">权限</span><span class="sxs-lookup"><span data-stu-id="332c7-105">Permissions</span></span>
<span data-ttu-id="332c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="332c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="332c7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="332c7-108">Permission type</span></span> | <span data-ttu-id="332c7-109">权限</span><span class="sxs-lookup"><span data-stu-id="332c7-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="332c7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="332c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="332c7-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="332c7-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="332c7-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="332c7-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="332c7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="332c7-113">Not supported.</span></span>|
|<span data-ttu-id="332c7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="332c7-114">Application</span></span>|<span data-ttu-id="332c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="332c7-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="332c7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="332c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="332c7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="332c7-117">Request headers</span></span>
| <span data-ttu-id="332c7-118">名称</span><span class="sxs-lookup"><span data-stu-id="332c7-118">Name</span></span>       | <span data-ttu-id="332c7-119">类型</span><span class="sxs-lookup"><span data-stu-id="332c7-119">Type</span></span> | <span data-ttu-id="332c7-120">说明</span><span class="sxs-lookup"><span data-stu-id="332c7-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="332c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="332c7-121">Authorization</span></span>  | <span data-ttu-id="332c7-122">string</span><span class="sxs-lookup"><span data-stu-id="332c7-122">string</span></span>  | <span data-ttu-id="332c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="332c7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="332c7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="332c7-125">Request body</span></span>
<span data-ttu-id="332c7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="332c7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="332c7-127">响应</span><span class="sxs-lookup"><span data-stu-id="332c7-127">Response</span></span>
<span data-ttu-id="332c7-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="332c7-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="332c7-129">示例</span><span class="sxs-lookup"><span data-stu-id="332c7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="332c7-130">请求</span><span class="sxs-lookup"><span data-stu-id="332c7-130">Request</span></span>
<span data-ttu-id="332c7-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="332c7-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="332c7-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="332c7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="332c7-133">C#</span><span class="sxs-lookup"><span data-stu-id="332c7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="332c7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="332c7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="332c7-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="332c7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="332c7-136">响应</span><span class="sxs-lookup"><span data-stu-id="332c7-136">Response</span></span>

<span data-ttu-id="332c7-137">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="332c7-137">There is no response body.</span></span>

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
