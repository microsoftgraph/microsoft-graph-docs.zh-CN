---
title: 获取 educationSynchronizationProfile 的状态
description: 获取租户中特定学校数据同步配置文件的状态。 响应将指示同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b9683a7f97ca2610efd8fd91a762dffd26a3e3b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424104"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="ab184-104">获取 educationSynchronizationProfile 的状态</span><span class="sxs-lookup"><span data-stu-id="ab184-104">Get the status of an educationSynchronizationProfile</span></span>

<span data-ttu-id="ab184-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ab184-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab184-106">获取租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="ab184-106">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="ab184-107">响应将指示同步的状态。</span><span class="sxs-lookup"><span data-stu-id="ab184-107">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab184-108">权限</span><span class="sxs-lookup"><span data-stu-id="ab184-108">Permissions</span></span>
<span data-ttu-id="ab184-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab184-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab184-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab184-111">Permission type</span></span> | <span data-ttu-id="ab184-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab184-112">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ab184-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab184-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ab184-114">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="ab184-114">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ab184-115">委派（个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="ab184-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ab184-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab184-116">Not supported.</span></span>|
|<span data-ttu-id="ab184-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab184-117">Application</span></span>| <span data-ttu-id="ab184-118">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="ab184-118">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab184-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab184-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="ab184-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab184-120">Request headers</span></span>
| <span data-ttu-id="ab184-121">名称</span><span class="sxs-lookup"><span data-stu-id="ab184-121">Name</span></span>       | <span data-ttu-id="ab184-122">类型</span><span class="sxs-lookup"><span data-stu-id="ab184-122">Type</span></span> | <span data-ttu-id="ab184-123">说明</span><span class="sxs-lookup"><span data-stu-id="ab184-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ab184-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab184-124">Authorization</span></span>  | <span data-ttu-id="ab184-125">string</span><span class="sxs-lookup"><span data-stu-id="ab184-125">string</span></span>  | <span data-ttu-id="ab184-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab184-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab184-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab184-128">Request body</span></span>
<span data-ttu-id="ab184-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab184-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ab184-130">响应</span><span class="sxs-lookup"><span data-stu-id="ab184-130">Response</span></span>
<span data-ttu-id="ab184-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab184-131">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab184-132">示例</span><span class="sxs-lookup"><span data-stu-id="ab184-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab184-133">请求</span><span class="sxs-lookup"><span data-stu-id="ab184-133">Request</span></span>
<span data-ttu-id="ab184-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab184-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab184-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab184-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="c"></a>[<span data-ttu-id="ab184-136">C#</span><span class="sxs-lookup"><span data-stu-id="ab184-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab184-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab184-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab184-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab184-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ab184-139">响应</span><span class="sxs-lookup"><span data-stu-id="ab184-139">Response</span></span>
<span data-ttu-id="ab184-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab184-140">The following is an example of the response.</span></span> 

><span data-ttu-id="ab184-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ab184-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
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
