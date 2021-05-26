---
title: 在 educationSynchronizationProfile 上重置同步
description: 重置租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 51a41991726ec9349f7f3f702973c8040031c39b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664732"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="4f598-103">在 educationSynchronizationProfile 上重置同步</span><span class="sxs-lookup"><span data-stu-id="4f598-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="4f598-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f598-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f598-105">重置租户中特定学校数据 [同步](../resources/educationsynchronizationprofile.md) 配置文件的同步。</span><span class="sxs-lookup"><span data-stu-id="4f598-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="4f598-106">**注意：** 此操作将导致同步重新启动。</span><span class="sxs-lookup"><span data-stu-id="4f598-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="4f598-107">将删除遇到的任何错误。</span><span class="sxs-lookup"><span data-stu-id="4f598-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="4f598-108">不会从 Azure AD Azure Active Directory (中删除任何) 。</span><span class="sxs-lookup"><span data-stu-id="4f598-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="4f598-109">权限</span><span class="sxs-lookup"><span data-stu-id="4f598-109">Permissions</span></span>
<span data-ttu-id="4f598-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f598-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f598-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f598-112">Permission type</span></span> | <span data-ttu-id="4f598-113">权限</span><span class="sxs-lookup"><span data-stu-id="4f598-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4f598-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f598-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4f598-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f598-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="4f598-116">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="4f598-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4f598-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f598-117">Not supported.</span></span>|
|<span data-ttu-id="4f598-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f598-118">Application</span></span>|<span data-ttu-id="4f598-119">EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f598-119">EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f598-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f598-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="4f598-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f598-121">Request headers</span></span>
| <span data-ttu-id="4f598-122">名称</span><span class="sxs-lookup"><span data-stu-id="4f598-122">Name</span></span>       | <span data-ttu-id="4f598-123">类型</span><span class="sxs-lookup"><span data-stu-id="4f598-123">Type</span></span> | <span data-ttu-id="4f598-124">说明</span><span class="sxs-lookup"><span data-stu-id="4f598-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f598-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f598-125">Authorization</span></span>  | <span data-ttu-id="4f598-126">string</span><span class="sxs-lookup"><span data-stu-id="4f598-126">string</span></span>  | <span data-ttu-id="4f598-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f598-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f598-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f598-129">Request body</span></span>
<span data-ttu-id="4f598-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f598-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4f598-131">响应</span><span class="sxs-lookup"><span data-stu-id="4f598-131">Response</span></span>
<span data-ttu-id="4f598-132">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4f598-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4f598-133">示例</span><span class="sxs-lookup"><span data-stu-id="4f598-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f598-134">请求</span><span class="sxs-lookup"><span data-stu-id="4f598-134">Request</span></span>
<span data-ttu-id="4f598-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f598-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f598-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f598-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="4f598-137">C#</span><span class="sxs-lookup"><span data-stu-id="4f598-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f598-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f598-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f598-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f598-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f598-140">Java</span><span class="sxs-lookup"><span data-stu-id="4f598-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-reset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f598-141">响应</span><span class="sxs-lookup"><span data-stu-id="4f598-141">Response</span></span>

<span data-ttu-id="4f598-142">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="4f598-142">There is no response body.</span></span>

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


