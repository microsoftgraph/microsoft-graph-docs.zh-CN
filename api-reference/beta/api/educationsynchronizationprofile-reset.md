---
title: 在 educationSynchronizationProfile 上重置同步
description: 在租户中重置特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00ed8f14dd2b84b0fab48c31dd352d53fffc805a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007099"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="ab228-103">在 educationSynchronizationProfile 上重置同步</span><span class="sxs-lookup"><span data-stu-id="ab228-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="ab228-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab228-105">在租户中重置特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 的同步。</span><span class="sxs-lookup"><span data-stu-id="ab228-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="ab228-106">**注意：** 此操作将导致重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="ab228-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="ab228-107">遇到的任何错误都将被删除。</span><span class="sxs-lookup"><span data-stu-id="ab228-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="ab228-108">将不会从 Azure Active Directory (Azure AD) 中删除任何数据。</span><span class="sxs-lookup"><span data-stu-id="ab228-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ab228-109">权限</span><span class="sxs-lookup"><span data-stu-id="ab228-109">Permissions</span></span>
<span data-ttu-id="ab228-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab228-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab228-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab228-112">Permission type</span></span> | <span data-ttu-id="ab228-113">权限</span><span class="sxs-lookup"><span data-stu-id="ab228-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ab228-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab228-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ab228-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab228-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ab228-116">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ab228-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ab228-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab228-117">Not supported.</span></span>|
|<span data-ttu-id="ab228-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab228-118">Application</span></span>|<span data-ttu-id="ab228-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab228-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab228-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab228-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="ab228-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab228-121">Request headers</span></span>
| <span data-ttu-id="ab228-122">名称</span><span class="sxs-lookup"><span data-stu-id="ab228-122">Name</span></span>       | <span data-ttu-id="ab228-123">类型</span><span class="sxs-lookup"><span data-stu-id="ab228-123">Type</span></span> | <span data-ttu-id="ab228-124">说明</span><span class="sxs-lookup"><span data-stu-id="ab228-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ab228-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab228-125">Authorization</span></span>  | <span data-ttu-id="ab228-126">string</span><span class="sxs-lookup"><span data-stu-id="ab228-126">string</span></span>  | <span data-ttu-id="ab228-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab228-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab228-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab228-129">Request body</span></span>
<span data-ttu-id="ab228-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab228-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ab228-131">响应</span><span class="sxs-lookup"><span data-stu-id="ab228-131">Response</span></span>
<span data-ttu-id="ab228-132">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ab228-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ab228-133">示例</span><span class="sxs-lookup"><span data-stu-id="ab228-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab228-134">请求</span><span class="sxs-lookup"><span data-stu-id="ab228-134">Request</span></span>
<span data-ttu-id="ab228-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab228-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab228-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab228-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="ab228-137">C#</span><span class="sxs-lookup"><span data-stu-id="ab228-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab228-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab228-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab228-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab228-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ab228-140">响应</span><span class="sxs-lookup"><span data-stu-id="ab228-140">Response</span></span>

<span data-ttu-id="ab228-141">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="ab228-141">There is no response body.</span></span>

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


