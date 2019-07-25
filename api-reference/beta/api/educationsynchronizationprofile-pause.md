---
title: 暂停 educationSynchronizationProfile 上的同步
description: 暂停租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cc96a75926a269a953cb7f7013858618be1c5733
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860051"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="be8a5-103">暂停 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="be8a5-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be8a5-104">暂停租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="be8a5-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="be8a5-105">权限</span><span class="sxs-lookup"><span data-stu-id="be8a5-105">Permissions</span></span>
<span data-ttu-id="be8a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be8a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be8a5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="be8a5-108">Permission type</span></span> | <span data-ttu-id="be8a5-109">权限</span><span class="sxs-lookup"><span data-stu-id="be8a5-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="be8a5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be8a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be8a5-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be8a5-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="be8a5-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="be8a5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="be8a5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="be8a5-113">Not supported.</span></span>|
|<span data-ttu-id="be8a5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="be8a5-114">Application</span></span>|<span data-ttu-id="be8a5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be8a5-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be8a5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be8a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="be8a5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="be8a5-117">Request headers</span></span>
| <span data-ttu-id="be8a5-118">名称</span><span class="sxs-lookup"><span data-stu-id="be8a5-118">Name</span></span>       | <span data-ttu-id="be8a5-119">类型</span><span class="sxs-lookup"><span data-stu-id="be8a5-119">Type</span></span> | <span data-ttu-id="be8a5-120">说明</span><span class="sxs-lookup"><span data-stu-id="be8a5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be8a5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be8a5-121">Authorization</span></span>  | <span data-ttu-id="be8a5-122">string</span><span class="sxs-lookup"><span data-stu-id="be8a5-122">string</span></span>  | <span data-ttu-id="be8a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be8a5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be8a5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="be8a5-125">Request body</span></span>
<span data-ttu-id="be8a5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be8a5-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="be8a5-127">响应</span><span class="sxs-lookup"><span data-stu-id="be8a5-127">Response</span></span>
<span data-ttu-id="be8a5-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="be8a5-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="be8a5-129">示例</span><span class="sxs-lookup"><span data-stu-id="be8a5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be8a5-130">请求</span><span class="sxs-lookup"><span data-stu-id="be8a5-130">Request</span></span>
<span data-ttu-id="be8a5-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be8a5-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be8a5-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="be8a5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="be8a5-133">C#</span><span class="sxs-lookup"><span data-stu-id="be8a5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be8a5-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="be8a5-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be8a5-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="be8a5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="be8a5-136">Java</span><span class="sxs-lookup"><span data-stu-id="be8a5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-synchronizationprofile-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="be8a5-137">响应</span><span class="sxs-lookup"><span data-stu-id="be8a5-137">Response</span></span>

<span data-ttu-id="be8a5-138">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="be8a5-138">There is no response body.</span></span>

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
