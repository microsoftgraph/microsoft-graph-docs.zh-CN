---
title: 获取 educationSynchronizationProfile 的状态
description: 获取租户中特定学校数据同步配置文件的状态。 响应将指示同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 68a40e061eada2f6d02e06bba3b47460589baf74
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720268"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="bb43d-104">获取 educationSynchronizationProfile 的状态</span><span class="sxs-lookup"><span data-stu-id="bb43d-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb43d-105">获取租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="bb43d-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="bb43d-106">响应将指示同步的状态。</span><span class="sxs-lookup"><span data-stu-id="bb43d-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb43d-107">权限</span><span class="sxs-lookup"><span data-stu-id="bb43d-107">Permissions</span></span>
<span data-ttu-id="bb43d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb43d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb43d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb43d-110">Permission type</span></span> | <span data-ttu-id="bb43d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb43d-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="bb43d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb43d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bb43d-113">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="bb43d-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="bb43d-114">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="bb43d-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bb43d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb43d-115">Not supported.</span></span>|
|<span data-ttu-id="bb43d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb43d-116">Application</span></span>| <span data-ttu-id="bb43d-117">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="bb43d-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb43d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb43d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="bb43d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb43d-119">Request headers</span></span>
| <span data-ttu-id="bb43d-120">名称</span><span class="sxs-lookup"><span data-stu-id="bb43d-120">Name</span></span>       | <span data-ttu-id="bb43d-121">类型</span><span class="sxs-lookup"><span data-stu-id="bb43d-121">Type</span></span> | <span data-ttu-id="bb43d-122">说明</span><span class="sxs-lookup"><span data-stu-id="bb43d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb43d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb43d-123">Authorization</span></span>  | <span data-ttu-id="bb43d-124">string</span><span class="sxs-lookup"><span data-stu-id="bb43d-124">string</span></span>  | <span data-ttu-id="bb43d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb43d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb43d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb43d-127">Request body</span></span>
<span data-ttu-id="bb43d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb43d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bb43d-129">响应</span><span class="sxs-lookup"><span data-stu-id="bb43d-129">Response</span></span>
<span data-ttu-id="bb43d-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bb43d-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb43d-131">示例</span><span class="sxs-lookup"><span data-stu-id="bb43d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb43d-132">请求</span><span class="sxs-lookup"><span data-stu-id="bb43d-132">Request</span></span>
<span data-ttu-id="bb43d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb43d-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bb43d-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bb43d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb43d-135">C#</span><span class="sxs-lookup"><span data-stu-id="bb43d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb43d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb43d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb43d-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="bb43d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb43d-138">响应</span><span class="sxs-lookup"><span data-stu-id="bb43d-138">Response</span></span>
<span data-ttu-id="bb43d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb43d-139">The following is an example of the response.</span></span> 

><span data-ttu-id="bb43d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bb43d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
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
