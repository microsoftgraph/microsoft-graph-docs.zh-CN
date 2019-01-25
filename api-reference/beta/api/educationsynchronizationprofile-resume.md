---
title: 恢复 educationSynchronizationProfile 上同步
description: 继续为租户中的特定学校数据同步配置文件同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 50ffcb4ceab401a3041ecb69baa1de0409be94a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513254"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="5e0f2-103">恢复 educationSynchronizationProfile 上同步</span><span class="sxs-lookup"><span data-stu-id="5e0f2-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e0f2-104">继续为租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e0f2-105">权限</span><span class="sxs-lookup"><span data-stu-id="5e0f2-105">Permissions</span></span>
<span data-ttu-id="5e0f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e0f2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e0f2-108">Permission type</span></span> | <span data-ttu-id="5e0f2-109">权限</span><span class="sxs-lookup"><span data-stu-id="5e0f2-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5e0f2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e0f2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5e0f2-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e0f2-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5e0f2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e0f2-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5e0f2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-113">Not supported.</span></span>|
|<span data-ttu-id="5e0f2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e0f2-114">Application</span></span>|<span data-ttu-id="5e0f2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e0f2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e0f2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="5e0f2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e0f2-117">Request headers</span></span>
| <span data-ttu-id="5e0f2-118">名称</span><span class="sxs-lookup"><span data-stu-id="5e0f2-118">Name</span></span>       | <span data-ttu-id="5e0f2-119">类型</span><span class="sxs-lookup"><span data-stu-id="5e0f2-119">Type</span></span> | <span data-ttu-id="5e0f2-120">说明</span><span class="sxs-lookup"><span data-stu-id="5e0f2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5e0f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e0f2-121">Authorization</span></span>  | <span data-ttu-id="5e0f2-122">string</span><span class="sxs-lookup"><span data-stu-id="5e0f2-122">string</span></span>  | <span data-ttu-id="5e0f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e0f2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e0f2-125">Request body</span></span>
<span data-ttu-id="5e0f2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5e0f2-127">响应</span><span class="sxs-lookup"><span data-stu-id="5e0f2-127">Response</span></span>
<span data-ttu-id="5e0f2-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5e0f2-129">示例</span><span class="sxs-lookup"><span data-stu-id="5e0f2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e0f2-130">请求</span><span class="sxs-lookup"><span data-stu-id="5e0f2-130">Request</span></span>
<span data-ttu-id="5e0f2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="5e0f2-132">响应</span><span class="sxs-lookup"><span data-stu-id="5e0f2-132">Response</span></span>

<span data-ttu-id="5e0f2-133">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="5e0f2-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
