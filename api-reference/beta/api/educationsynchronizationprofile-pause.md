---
title: 暂停 educationSynchronizationProfile 上的同步
description: 暂停租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: abe0d94691608c245757b53b4417c88d19679409
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587480"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="f17a2-103">暂停 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="f17a2-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f17a2-104">暂停租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="f17a2-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f17a2-105">权限</span><span class="sxs-lookup"><span data-stu-id="f17a2-105">Permissions</span></span>
<span data-ttu-id="f17a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f17a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f17a2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f17a2-108">Permission type</span></span> | <span data-ttu-id="f17a2-109">权限</span><span class="sxs-lookup"><span data-stu-id="f17a2-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f17a2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f17a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f17a2-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f17a2-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f17a2-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="f17a2-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f17a2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f17a2-113">Not supported.</span></span>|
|<span data-ttu-id="f17a2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f17a2-114">Application</span></span>|<span data-ttu-id="f17a2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f17a2-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f17a2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f17a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="f17a2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f17a2-117">Request headers</span></span>
| <span data-ttu-id="f17a2-118">名称</span><span class="sxs-lookup"><span data-stu-id="f17a2-118">Name</span></span>       | <span data-ttu-id="f17a2-119">类型</span><span class="sxs-lookup"><span data-stu-id="f17a2-119">Type</span></span> | <span data-ttu-id="f17a2-120">说明</span><span class="sxs-lookup"><span data-stu-id="f17a2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f17a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f17a2-121">Authorization</span></span>  | <span data-ttu-id="f17a2-122">string</span><span class="sxs-lookup"><span data-stu-id="f17a2-122">string</span></span>  | <span data-ttu-id="f17a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f17a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f17a2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f17a2-125">Request body</span></span>
<span data-ttu-id="f17a2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f17a2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f17a2-127">响应</span><span class="sxs-lookup"><span data-stu-id="f17a2-127">Response</span></span>
<span data-ttu-id="f17a2-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f17a2-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f17a2-129">示例</span><span class="sxs-lookup"><span data-stu-id="f17a2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f17a2-130">请求</span><span class="sxs-lookup"><span data-stu-id="f17a2-130">Request</span></span>
<span data-ttu-id="f17a2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f17a2-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="f17a2-132">响应</span><span class="sxs-lookup"><span data-stu-id="f17a2-132">Response</span></span>

<span data-ttu-id="f17a2-133">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="f17a2-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="f17a2-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f17a2-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f17a2-135">语言</span><span class="sxs-lookup"><span data-stu-id="f17a2-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_synchronizationProfile_pause-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f17a2-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="f17a2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_synchronizationProfile_pause-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
