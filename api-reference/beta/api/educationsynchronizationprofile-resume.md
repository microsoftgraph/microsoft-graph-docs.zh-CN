---
title: 恢复 educationSynchronizationProfile 上的同步
description: 在租户中恢复特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 83007ef7a38189f6b50d286940af7e6c287700f8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259505"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="3ef16-103">恢复 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="3ef16-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ef16-104">在租户中恢复特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="3ef16-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ef16-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ef16-105">Permissions</span></span>
<span data-ttu-id="3ef16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ef16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ef16-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ef16-108">Permission type</span></span> | <span data-ttu-id="3ef16-109">权限</span><span class="sxs-lookup"><span data-stu-id="3ef16-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3ef16-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ef16-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ef16-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ef16-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="3ef16-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="3ef16-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3ef16-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ef16-113">Not supported.</span></span>|
|<span data-ttu-id="3ef16-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ef16-114">Application</span></span>|<span data-ttu-id="3ef16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ef16-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ef16-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ef16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="3ef16-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ef16-117">Request headers</span></span>
| <span data-ttu-id="3ef16-118">名称</span><span class="sxs-lookup"><span data-stu-id="3ef16-118">Name</span></span>       | <span data-ttu-id="3ef16-119">类型</span><span class="sxs-lookup"><span data-stu-id="3ef16-119">Type</span></span> | <span data-ttu-id="3ef16-120">说明</span><span class="sxs-lookup"><span data-stu-id="3ef16-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ef16-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ef16-121">Authorization</span></span>  | <span data-ttu-id="3ef16-122">string</span><span class="sxs-lookup"><span data-stu-id="3ef16-122">string</span></span>  | <span data-ttu-id="3ef16-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ef16-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ef16-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ef16-125">Request body</span></span>
<span data-ttu-id="3ef16-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ef16-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3ef16-127">响应</span><span class="sxs-lookup"><span data-stu-id="3ef16-127">Response</span></span>
<span data-ttu-id="3ef16-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3ef16-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ef16-129">示例</span><span class="sxs-lookup"><span data-stu-id="3ef16-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ef16-130">请求</span><span class="sxs-lookup"><span data-stu-id="3ef16-130">Request</span></span>
<span data-ttu-id="3ef16-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3ef16-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="3ef16-132">响应</span><span class="sxs-lookup"><span data-stu-id="3ef16-132">Response</span></span>

<span data-ttu-id="3ef16-133">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="3ef16-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3ef16-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3ef16-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3ef16-135">C#</span><span class="sxs-lookup"><span data-stu-id="3ef16-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ef16-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ef16-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3ef16-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="3ef16-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
