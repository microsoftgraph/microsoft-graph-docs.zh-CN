---
title: 在 educationSynchronizationProfile 上重置同步
description: 重置租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2afd14b647b02897c140287e96f8bd1f5fdd89fe
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574172"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="15110-103">在 educationSynchronizationProfile 上重置同步</span><span class="sxs-lookup"><span data-stu-id="15110-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="15110-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15110-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15110-105">重置租户中特定学校数据 [同步](../resources/educationsynchronizationprofile.md) 配置文件的同步。</span><span class="sxs-lookup"><span data-stu-id="15110-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="15110-106">**注意：** 此操作将导致同步重新启动。</span><span class="sxs-lookup"><span data-stu-id="15110-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="15110-107">将删除遇到的任何错误。</span><span class="sxs-lookup"><span data-stu-id="15110-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="15110-108">不会从 Azure Active Directory 和 Azure AD (中删除) 。</span><span class="sxs-lookup"><span data-stu-id="15110-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="15110-109">权限</span><span class="sxs-lookup"><span data-stu-id="15110-109">Permissions</span></span>
<span data-ttu-id="15110-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15110-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15110-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="15110-112">Permission type</span></span> | <span data-ttu-id="15110-113">权限</span><span class="sxs-lookup"><span data-stu-id="15110-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="15110-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15110-114">Delegated (work or school account)</span></span> | <span data-ttu-id="15110-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15110-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="15110-116">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="15110-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="15110-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="15110-117">Not supported.</span></span>|
|<span data-ttu-id="15110-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="15110-118">Application</span></span>|<span data-ttu-id="15110-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="15110-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15110-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15110-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="15110-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="15110-121">Request headers</span></span>
| <span data-ttu-id="15110-122">名称</span><span class="sxs-lookup"><span data-stu-id="15110-122">Name</span></span>       | <span data-ttu-id="15110-123">类型</span><span class="sxs-lookup"><span data-stu-id="15110-123">Type</span></span> | <span data-ttu-id="15110-124">说明</span><span class="sxs-lookup"><span data-stu-id="15110-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15110-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="15110-125">Authorization</span></span>  | <span data-ttu-id="15110-126">string</span><span class="sxs-lookup"><span data-stu-id="15110-126">string</span></span>  | <span data-ttu-id="15110-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15110-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15110-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="15110-129">Request body</span></span>
<span data-ttu-id="15110-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="15110-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="15110-131">响应</span><span class="sxs-lookup"><span data-stu-id="15110-131">Response</span></span>
<span data-ttu-id="15110-132">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="15110-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="15110-133">示例</span><span class="sxs-lookup"><span data-stu-id="15110-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15110-134">请求</span><span class="sxs-lookup"><span data-stu-id="15110-134">Request</span></span>
<span data-ttu-id="15110-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15110-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15110-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="15110-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="15110-137">C#</span><span class="sxs-lookup"><span data-stu-id="15110-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15110-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15110-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15110-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15110-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15110-140">Java</span><span class="sxs-lookup"><span data-stu-id="15110-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-reset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="15110-141">响应</span><span class="sxs-lookup"><span data-stu-id="15110-141">Response</span></span>

<span data-ttu-id="15110-142">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="15110-142">There is no response body.</span></span>

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


