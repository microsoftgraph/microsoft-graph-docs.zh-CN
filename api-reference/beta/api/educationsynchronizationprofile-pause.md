---
title: 暂停 educationSynchronizationProfile 上的同步
description: 暂停租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 44477aae7799922008b0a7623fd7e4c91c09e0aa
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574214"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="b1424-103">暂停 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="b1424-103">Pause sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="b1424-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1424-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1424-105">暂停租户中特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 的同步。</span><span class="sxs-lookup"><span data-stu-id="b1424-105">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1424-106">权限</span><span class="sxs-lookup"><span data-stu-id="b1424-106">Permissions</span></span>
<span data-ttu-id="b1424-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1424-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1424-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1424-109">Permission type</span></span> | <span data-ttu-id="b1424-110">权限</span><span class="sxs-lookup"><span data-stu-id="b1424-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="b1424-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1424-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b1424-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1424-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="b1424-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="b1424-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b1424-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1424-114">Not supported.</span></span>|
|<span data-ttu-id="b1424-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1424-115">Application</span></span>|<span data-ttu-id="b1424-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1424-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1424-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1424-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="b1424-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1424-118">Request headers</span></span>
| <span data-ttu-id="b1424-119">名称</span><span class="sxs-lookup"><span data-stu-id="b1424-119">Name</span></span>       | <span data-ttu-id="b1424-120">类型</span><span class="sxs-lookup"><span data-stu-id="b1424-120">Type</span></span> | <span data-ttu-id="b1424-121">说明</span><span class="sxs-lookup"><span data-stu-id="b1424-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1424-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1424-122">Authorization</span></span>  | <span data-ttu-id="b1424-123">string</span><span class="sxs-lookup"><span data-stu-id="b1424-123">string</span></span>  | <span data-ttu-id="b1424-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1424-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1424-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1424-126">Request body</span></span>
<span data-ttu-id="b1424-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1424-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b1424-128">响应</span><span class="sxs-lookup"><span data-stu-id="b1424-128">Response</span></span>
<span data-ttu-id="b1424-129">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b1424-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1424-130">示例</span><span class="sxs-lookup"><span data-stu-id="b1424-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1424-131">请求</span><span class="sxs-lookup"><span data-stu-id="b1424-131">Request</span></span>
<span data-ttu-id="b1424-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b1424-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1424-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1424-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="c"></a>[<span data-ttu-id="b1424-134">C#</span><span class="sxs-lookup"><span data-stu-id="b1424-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1424-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1424-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1424-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1424-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1424-137">Java</span><span class="sxs-lookup"><span data-stu-id="b1424-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-synchronizationprofile-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b1424-138">响应</span><span class="sxs-lookup"><span data-stu-id="b1424-138">Response</span></span>

<span data-ttu-id="b1424-139">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="b1424-139">There is no response body.</span></span>

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


