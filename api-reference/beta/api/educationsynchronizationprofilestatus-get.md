---
title: 获取 educationSynchronizationProfile 的状态
description: 为租户中获取特定学校数据同步配置文件的状态。 响应将指示的同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 394bb03760e33b4581f5d29e90a4c8fd875c26d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418132"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="5cc99-104">获取 educationSynchronizationProfile 的状态</span><span class="sxs-lookup"><span data-stu-id="5cc99-104">Get the status of an educationSynchronizationProfile</span></span>

> <span data-ttu-id="5cc99-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5cc99-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cc99-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5cc99-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5cc99-107">获取租户中的特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="5cc99-107">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="5cc99-108">响应将指示的同步的状态。</span><span class="sxs-lookup"><span data-stu-id="5cc99-108">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cc99-109">权限</span><span class="sxs-lookup"><span data-stu-id="5cc99-109">Permissions</span></span>
<span data-ttu-id="5cc99-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cc99-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5cc99-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cc99-112">Permission type</span></span> | <span data-ttu-id="5cc99-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cc99-113">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5cc99-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cc99-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5cc99-115">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cc99-115">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5cc99-116">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5cc99-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5cc99-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cc99-117">Not supported.</span></span>|
|<span data-ttu-id="5cc99-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cc99-118">Application</span></span>| <span data-ttu-id="5cc99-119">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cc99-119">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cc99-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cc99-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="5cc99-121">请求头</span><span class="sxs-lookup"><span data-stu-id="5cc99-121">Request headers</span></span>
| <span data-ttu-id="5cc99-122">名称</span><span class="sxs-lookup"><span data-stu-id="5cc99-122">Name</span></span>       | <span data-ttu-id="5cc99-123">类型</span><span class="sxs-lookup"><span data-stu-id="5cc99-123">Type</span></span> | <span data-ttu-id="5cc99-124">说明</span><span class="sxs-lookup"><span data-stu-id="5cc99-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5cc99-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cc99-125">Authorization</span></span>  | <span data-ttu-id="5cc99-126">string</span><span class="sxs-lookup"><span data-stu-id="5cc99-126">string</span></span>  | <span data-ttu-id="5cc99-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5cc99-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cc99-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cc99-129">Request body</span></span>
<span data-ttu-id="5cc99-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5cc99-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5cc99-131">响应</span><span class="sxs-lookup"><span data-stu-id="5cc99-131">Response</span></span>
<span data-ttu-id="5cc99-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5cc99-132">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc99-133">示例</span><span class="sxs-lookup"><span data-stu-id="5cc99-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cc99-134">请求</span><span class="sxs-lookup"><span data-stu-id="5cc99-134">Request</span></span>
<span data-ttu-id="5cc99-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5cc99-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="5cc99-136">响应</span><span class="sxs-lookup"><span data-stu-id="5cc99-136">Response</span></span>
<span data-ttu-id="5cc99-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5cc99-137">The following is an example of the response.</span></span> 

><span data-ttu-id="5cc99-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5cc99-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
