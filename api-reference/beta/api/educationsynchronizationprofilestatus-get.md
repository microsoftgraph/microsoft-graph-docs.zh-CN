---
title: 获取 educationSynchronizationProfile 的状态
description: 获取租户中特定学校数据同步配置文件的状态。 响应将指示同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f33c53e850babed98536fba74de6d6162e9045
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587526"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="5fd58-104">获取 educationSynchronizationProfile 的状态</span><span class="sxs-lookup"><span data-stu-id="5fd58-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fd58-105">获取租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="5fd58-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="5fd58-106">响应将指示同步的状态。</span><span class="sxs-lookup"><span data-stu-id="5fd58-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fd58-107">权限</span><span class="sxs-lookup"><span data-stu-id="5fd58-107">Permissions</span></span>
<span data-ttu-id="5fd58-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5fd58-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fd58-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fd58-110">Permission type</span></span> | <span data-ttu-id="5fd58-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5fd58-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5fd58-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fd58-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5fd58-113">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="5fd58-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5fd58-114">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5fd58-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5fd58-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fd58-115">Not supported.</span></span>|
|<span data-ttu-id="5fd58-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fd58-116">Application</span></span>| <span data-ttu-id="5fd58-117">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="5fd58-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fd58-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fd58-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="5fd58-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fd58-119">Request headers</span></span>
| <span data-ttu-id="5fd58-120">名称</span><span class="sxs-lookup"><span data-stu-id="5fd58-120">Name</span></span>       | <span data-ttu-id="5fd58-121">类型</span><span class="sxs-lookup"><span data-stu-id="5fd58-121">Type</span></span> | <span data-ttu-id="5fd58-122">说明</span><span class="sxs-lookup"><span data-stu-id="5fd58-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5fd58-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fd58-123">Authorization</span></span>  | <span data-ttu-id="5fd58-124">string</span><span class="sxs-lookup"><span data-stu-id="5fd58-124">string</span></span>  | <span data-ttu-id="5fd58-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5fd58-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5fd58-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fd58-127">Request body</span></span>
<span data-ttu-id="5fd58-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5fd58-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5fd58-129">响应</span><span class="sxs-lookup"><span data-stu-id="5fd58-129">Response</span></span>
<span data-ttu-id="5fd58-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5fd58-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fd58-131">示例</span><span class="sxs-lookup"><span data-stu-id="5fd58-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fd58-132">请求</span><span class="sxs-lookup"><span data-stu-id="5fd58-132">Request</span></span>
<span data-ttu-id="5fd58-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5fd58-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="5fd58-134">响应</span><span class="sxs-lookup"><span data-stu-id="5fd58-134">Response</span></span>
<span data-ttu-id="5fd58-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5fd58-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5fd58-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5fd58-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5fd58-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5fd58-138">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="5fd58-139">语言</span><span class="sxs-lookup"><span data-stu-id="5fd58-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_status-Cs-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
