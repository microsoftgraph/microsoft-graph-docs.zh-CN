---
title: 获取 educationSynchronizationProfile 的状态
description: 获取租户中特定学校数据同步配置文件的状态。 响应将指示同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1b9d8a1b8faf09ce9f70b4744dc116513b12c640
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954744"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="e8c7b-104">获取 educationSynchronizationProfile 的状态</span><span class="sxs-lookup"><span data-stu-id="e8c7b-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8c7b-105">获取租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="e8c7b-106">响应将指示同步的状态。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8c7b-107">权限</span><span class="sxs-lookup"><span data-stu-id="e8c7b-107">Permissions</span></span>
<span data-ttu-id="e8c7b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8c7b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8c7b-110">Permission type</span></span> | <span data-ttu-id="e8c7b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8c7b-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e8c7b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8c7b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8c7b-113">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="e8c7b-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e8c7b-114">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e8c7b-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e8c7b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-115">Not supported.</span></span>|
|<span data-ttu-id="e8c7b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8c7b-116">Application</span></span>| <span data-ttu-id="e8c7b-117">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="e8c7b-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8c7b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8c7b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="e8c7b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8c7b-119">Request headers</span></span>
| <span data-ttu-id="e8c7b-120">名称</span><span class="sxs-lookup"><span data-stu-id="e8c7b-120">Name</span></span>       | <span data-ttu-id="e8c7b-121">类型</span><span class="sxs-lookup"><span data-stu-id="e8c7b-121">Type</span></span> | <span data-ttu-id="e8c7b-122">说明</span><span class="sxs-lookup"><span data-stu-id="e8c7b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8c7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8c7b-123">Authorization</span></span>  | <span data-ttu-id="e8c7b-124">string</span><span class="sxs-lookup"><span data-stu-id="e8c7b-124">string</span></span>  | <span data-ttu-id="e8c7b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8c7b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8c7b-127">Request body</span></span>
<span data-ttu-id="e8c7b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e8c7b-129">响应</span><span class="sxs-lookup"><span data-stu-id="e8c7b-129">Response</span></span>
<span data-ttu-id="e8c7b-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8c7b-131">示例</span><span class="sxs-lookup"><span data-stu-id="e8c7b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8c7b-132">请求</span><span class="sxs-lookup"><span data-stu-id="e8c7b-132">Request</span></span>
<span data-ttu-id="e8c7b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8c7b-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e8c7b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8c7b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e8c7b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8c7b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8c7b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8c7b-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="e8c7b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8c7b-138">Java</span><span class="sxs-lookup"><span data-stu-id="e8c7b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-status-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e8c7b-139">响应</span><span class="sxs-lookup"><span data-stu-id="e8c7b-139">Response</span></span>
<span data-ttu-id="e8c7b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="e8c7b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e8c7b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
