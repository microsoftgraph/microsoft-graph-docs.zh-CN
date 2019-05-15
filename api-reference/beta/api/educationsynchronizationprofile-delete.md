---
title: 删除 educationSynchronizationProfile
description: 根据标识符删除租户中的学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 347efaf51f258535c1217252f4df5a22091fa7ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960863"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="361c3-103">删除 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="361c3-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="361c3-104">根据标识符删除租户中的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="361c3-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="361c3-105">权限</span><span class="sxs-lookup"><span data-stu-id="361c3-105">Permissions</span></span>
<span data-ttu-id="361c3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="361c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="361c3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="361c3-108">Permission type</span></span> | <span data-ttu-id="361c3-109">权限</span><span class="sxs-lookup"><span data-stu-id="361c3-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="361c3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="361c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="361c3-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="361c3-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="361c3-112">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="361c3-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="361c3-113">请求标头</span><span class="sxs-lookup"><span data-stu-id="361c3-113">Request headers</span></span>
| <span data-ttu-id="361c3-114">名称</span><span class="sxs-lookup"><span data-stu-id="361c3-114">Name</span></span>       | <span data-ttu-id="361c3-115">类型</span><span class="sxs-lookup"><span data-stu-id="361c3-115">Type</span></span> | <span data-ttu-id="361c3-116">说明</span><span class="sxs-lookup"><span data-stu-id="361c3-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="361c3-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="361c3-117">Authorization</span></span>  | <span data-ttu-id="361c3-118">string</span><span class="sxs-lookup"><span data-stu-id="361c3-118">string</span></span>  | <span data-ttu-id="361c3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="361c3-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="361c3-121">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="361c3-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="361c3-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="361c3-122">Not supported.</span></span>|
|<span data-ttu-id="361c3-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="361c3-123">Application</span></span>|<span data-ttu-id="361c3-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="361c3-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="361c3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="361c3-125">Request body</span></span>
<span data-ttu-id="361c3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="361c3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="361c3-127">响应</span><span class="sxs-lookup"><span data-stu-id="361c3-127">Response</span></span>
<span data-ttu-id="361c3-128">如果成功, 此方法将`202 Accepted`返回响应代码, 不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="361c3-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="361c3-129">示例</span><span class="sxs-lookup"><span data-stu-id="361c3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="361c3-130">请求</span><span class="sxs-lookup"><span data-stu-id="361c3-130">Request</span></span>
<span data-ttu-id="361c3-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="361c3-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="361c3-132">响应</span><span class="sxs-lookup"><span data-stu-id="361c3-132">Response</span></span>
<span data-ttu-id="361c3-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="361c3-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="361c3-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="361c3-134">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="361c3-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="361c3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="361c3-136">C#</span><span class="sxs-lookup"><span data-stu-id="361c3-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Cs-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
