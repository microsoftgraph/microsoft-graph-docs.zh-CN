---
title: 在 educationSynchronizationProfile 上恢复同步
description: 恢复租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0f1cd4ca3e1569825bda00a16723801521d1bc08
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664725"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="2fee6-103">在 educationSynchronizationProfile 上恢复同步</span><span class="sxs-lookup"><span data-stu-id="2fee6-103">Resume sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="2fee6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fee6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fee6-105">恢复租户中特定学校 [数据同步](../resources/educationsynchronizationprofile.md) 配置文件的同步。</span><span class="sxs-lookup"><span data-stu-id="2fee6-105">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fee6-106">权限</span><span class="sxs-lookup"><span data-stu-id="2fee6-106">Permissions</span></span>
<span data-ttu-id="2fee6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fee6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fee6-109">Permission type</span></span> | <span data-ttu-id="2fee6-110">权限</span><span class="sxs-lookup"><span data-stu-id="2fee6-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2fee6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fee6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2fee6-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fee6-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2fee6-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="2fee6-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2fee6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fee6-114">Not supported.</span></span>|
|<span data-ttu-id="2fee6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fee6-115">Application</span></span>|<span data-ttu-id="2fee6-116">EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fee6-116">EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fee6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fee6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="2fee6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fee6-118">Request headers</span></span>
| <span data-ttu-id="2fee6-119">名称</span><span class="sxs-lookup"><span data-stu-id="2fee6-119">Name</span></span>       | <span data-ttu-id="2fee6-120">类型</span><span class="sxs-lookup"><span data-stu-id="2fee6-120">Type</span></span> | <span data-ttu-id="2fee6-121">说明</span><span class="sxs-lookup"><span data-stu-id="2fee6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2fee6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fee6-122">Authorization</span></span>  | <span data-ttu-id="2fee6-123">string</span><span class="sxs-lookup"><span data-stu-id="2fee6-123">string</span></span>  | <span data-ttu-id="2fee6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2fee6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2fee6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fee6-126">Request body</span></span>
<span data-ttu-id="2fee6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2fee6-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2fee6-128">响应</span><span class="sxs-lookup"><span data-stu-id="2fee6-128">Response</span></span>
<span data-ttu-id="2fee6-129">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2fee6-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2fee6-130">示例</span><span class="sxs-lookup"><span data-stu-id="2fee6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fee6-131">请求</span><span class="sxs-lookup"><span data-stu-id="2fee6-131">Request</span></span>
<span data-ttu-id="2fee6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2fee6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fee6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fee6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="c"></a>[<span data-ttu-id="2fee6-134">C#</span><span class="sxs-lookup"><span data-stu-id="2fee6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fee6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fee6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fee6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fee6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fee6-137">Java</span><span class="sxs-lookup"><span data-stu-id="2fee6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-resume-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2fee6-138">响应</span><span class="sxs-lookup"><span data-stu-id="2fee6-138">Response</span></span>

<span data-ttu-id="2fee6-139">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="2fee6-139">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
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


