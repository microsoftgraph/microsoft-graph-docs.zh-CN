---
title: 获取 educationSynchronizationProfile 的状态
description: 获取租户中特定学校数据同步配置文件的状态。 响应将指示同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a2d3dffd715d78bb96794808da39255db0164b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457459"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="9af4c-104">获取 educationSynchronizationProfile 的状态</span><span class="sxs-lookup"><span data-stu-id="9af4c-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9af4c-105">获取租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="9af4c-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="9af4c-106">响应将指示同步的状态。</span><span class="sxs-lookup"><span data-stu-id="9af4c-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="9af4c-107">权限</span><span class="sxs-lookup"><span data-stu-id="9af4c-107">Permissions</span></span>
<span data-ttu-id="9af4c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9af4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9af4c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9af4c-110">Permission type</span></span> | <span data-ttu-id="9af4c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9af4c-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9af4c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9af4c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9af4c-113">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="9af4c-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="9af4c-114">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="9af4c-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9af4c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9af4c-115">Not supported.</span></span>|
|<span data-ttu-id="9af4c-116">Application</span><span class="sxs-lookup"><span data-stu-id="9af4c-116">Application</span></span>| <span data-ttu-id="9af4c-117">EduAdministration、EduAdministration 和所有</span><span class="sxs-lookup"><span data-stu-id="9af4c-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9af4c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9af4c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="9af4c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9af4c-119">Request headers</span></span>
| <span data-ttu-id="9af4c-120">名称</span><span class="sxs-lookup"><span data-stu-id="9af4c-120">Name</span></span>       | <span data-ttu-id="9af4c-121">类型</span><span class="sxs-lookup"><span data-stu-id="9af4c-121">Type</span></span> | <span data-ttu-id="9af4c-122">说明</span><span class="sxs-lookup"><span data-stu-id="9af4c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9af4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9af4c-123">Authorization</span></span>  | <span data-ttu-id="9af4c-124">string</span><span class="sxs-lookup"><span data-stu-id="9af4c-124">string</span></span>  | <span data-ttu-id="9af4c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9af4c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9af4c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9af4c-127">Request body</span></span>
<span data-ttu-id="9af4c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9af4c-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9af4c-129">响应</span><span class="sxs-lookup"><span data-stu-id="9af4c-129">Response</span></span>
<span data-ttu-id="9af4c-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9af4c-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9af4c-131">示例</span><span class="sxs-lookup"><span data-stu-id="9af4c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9af4c-132">请求</span><span class="sxs-lookup"><span data-stu-id="9af4c-132">Request</span></span>
<span data-ttu-id="9af4c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9af4c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="9af4c-134">响应</span><span class="sxs-lookup"><span data-stu-id="9af4c-134">Response</span></span>
<span data-ttu-id="9af4c-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9af4c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9af4c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9af4c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
