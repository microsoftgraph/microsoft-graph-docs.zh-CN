---
title: 在 educationSynchronizationProfile 上重置同步
description: 在租户中重置特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f98548765e185d6bb3f66bbec33b50cd496c4804
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415979"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="e56d2-103">在 educationSynchronizationProfile 上重置同步</span><span class="sxs-lookup"><span data-stu-id="e56d2-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e56d2-104">在租户中重置特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="e56d2-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="e56d2-105">**注意:** 此操作将导致重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="e56d2-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="e56d2-106">遇到的任何错误都将被删除。</span><span class="sxs-lookup"><span data-stu-id="e56d2-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="e56d2-107">将不会从 Azure Active Directory (Azure AD) 中删除任何数据。</span><span class="sxs-lookup"><span data-stu-id="e56d2-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e56d2-108">权限</span><span class="sxs-lookup"><span data-stu-id="e56d2-108">Permissions</span></span>
<span data-ttu-id="e56d2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e56d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e56d2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e56d2-111">Permission type</span></span> | <span data-ttu-id="e56d2-112">权限</span><span class="sxs-lookup"><span data-stu-id="e56d2-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e56d2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e56d2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e56d2-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e56d2-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e56d2-115">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e56d2-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e56d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e56d2-116">Not supported.</span></span>|
|<span data-ttu-id="e56d2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e56d2-117">Application</span></span>|<span data-ttu-id="e56d2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e56d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e56d2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e56d2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="e56d2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e56d2-120">Request headers</span></span>
| <span data-ttu-id="e56d2-121">名称</span><span class="sxs-lookup"><span data-stu-id="e56d2-121">Name</span></span>       | <span data-ttu-id="e56d2-122">类型</span><span class="sxs-lookup"><span data-stu-id="e56d2-122">Type</span></span> | <span data-ttu-id="e56d2-123">说明</span><span class="sxs-lookup"><span data-stu-id="e56d2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e56d2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e56d2-124">Authorization</span></span>  | <span data-ttu-id="e56d2-125">string</span><span class="sxs-lookup"><span data-stu-id="e56d2-125">string</span></span>  | <span data-ttu-id="e56d2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e56d2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e56d2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e56d2-128">Request body</span></span>
<span data-ttu-id="e56d2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e56d2-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e56d2-130">响应</span><span class="sxs-lookup"><span data-stu-id="e56d2-130">Response</span></span>
<span data-ttu-id="e56d2-131">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e56d2-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e56d2-132">示例</span><span class="sxs-lookup"><span data-stu-id="e56d2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e56d2-133">请求</span><span class="sxs-lookup"><span data-stu-id="e56d2-133">Request</span></span>
<span data-ttu-id="e56d2-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e56d2-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e56d2-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e56d2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e56d2-136">C#</span><span class="sxs-lookup"><span data-stu-id="e56d2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e56d2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e56d2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e56d2-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="e56d2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e56d2-139">响应</span><span class="sxs-lookup"><span data-stu-id="e56d2-139">Response</span></span>

<span data-ttu-id="e56d2-140">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="e56d2-140">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
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
