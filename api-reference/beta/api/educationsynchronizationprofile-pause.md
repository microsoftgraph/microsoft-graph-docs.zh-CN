---
title: 暂停 educationSynchronizationProfile 上的同步
description: 暂停租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c9ba7d2ab3f67880105d45d9d98506b8e8caaac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464689"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="c366d-103">暂停 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="c366d-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c366d-104">暂停租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="c366d-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c366d-105">权限</span><span class="sxs-lookup"><span data-stu-id="c366d-105">Permissions</span></span>
<span data-ttu-id="c366d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c366d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c366d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c366d-108">Permission type</span></span> | <span data-ttu-id="c366d-109">权限</span><span class="sxs-lookup"><span data-stu-id="c366d-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c366d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c366d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c366d-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c366d-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c366d-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="c366d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c366d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c366d-113">Not supported.</span></span>|
|<span data-ttu-id="c366d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c366d-114">Application</span></span>|<span data-ttu-id="c366d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c366d-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c366d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c366d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="c366d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c366d-117">Request headers</span></span>
| <span data-ttu-id="c366d-118">名称</span><span class="sxs-lookup"><span data-stu-id="c366d-118">Name</span></span>       | <span data-ttu-id="c366d-119">类型</span><span class="sxs-lookup"><span data-stu-id="c366d-119">Type</span></span> | <span data-ttu-id="c366d-120">说明</span><span class="sxs-lookup"><span data-stu-id="c366d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c366d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c366d-121">Authorization</span></span>  | <span data-ttu-id="c366d-122">string</span><span class="sxs-lookup"><span data-stu-id="c366d-122">string</span></span>  | <span data-ttu-id="c366d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c366d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c366d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c366d-125">Request body</span></span>
<span data-ttu-id="c366d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c366d-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c366d-127">响应</span><span class="sxs-lookup"><span data-stu-id="c366d-127">Response</span></span>
<span data-ttu-id="c366d-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c366d-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c366d-129">示例</span><span class="sxs-lookup"><span data-stu-id="c366d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c366d-130">请求</span><span class="sxs-lookup"><span data-stu-id="c366d-130">Request</span></span>
<span data-ttu-id="c366d-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c366d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="c366d-132">响应</span><span class="sxs-lookup"><span data-stu-id="c366d-132">Response</span></span>

<span data-ttu-id="c366d-133">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="c366d-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
