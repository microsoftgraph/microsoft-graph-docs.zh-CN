---
title: 在 educationSynchronizationProfile 暂停同步
description: 暂停租户中的特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c9ba7d2ab3f67880105d45d9d98506b8e8caaac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510930"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="b6aef-103">在 educationSynchronizationProfile 暂停同步</span><span class="sxs-lookup"><span data-stu-id="b6aef-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6aef-104">暂停的租户特定的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="b6aef-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6aef-105">权限</span><span class="sxs-lookup"><span data-stu-id="b6aef-105">Permissions</span></span>
<span data-ttu-id="b6aef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6aef-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6aef-108">Permission type</span></span> | <span data-ttu-id="b6aef-109">权限</span><span class="sxs-lookup"><span data-stu-id="b6aef-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="b6aef-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6aef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6aef-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6aef-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="b6aef-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6aef-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b6aef-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6aef-113">Not supported.</span></span>|
|<span data-ttu-id="b6aef-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6aef-114">Application</span></span>|<span data-ttu-id="b6aef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6aef-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6aef-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6aef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="b6aef-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6aef-117">Request headers</span></span>
| <span data-ttu-id="b6aef-118">名称</span><span class="sxs-lookup"><span data-stu-id="b6aef-118">Name</span></span>       | <span data-ttu-id="b6aef-119">类型</span><span class="sxs-lookup"><span data-stu-id="b6aef-119">Type</span></span> | <span data-ttu-id="b6aef-120">说明</span><span class="sxs-lookup"><span data-stu-id="b6aef-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b6aef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6aef-121">Authorization</span></span>  | <span data-ttu-id="b6aef-122">string</span><span class="sxs-lookup"><span data-stu-id="b6aef-122">string</span></span>  | <span data-ttu-id="b6aef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6aef-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b6aef-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6aef-125">Request body</span></span>
<span data-ttu-id="b6aef-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6aef-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b6aef-127">响应</span><span class="sxs-lookup"><span data-stu-id="b6aef-127">Response</span></span>
<span data-ttu-id="b6aef-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b6aef-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6aef-129">示例</span><span class="sxs-lookup"><span data-stu-id="b6aef-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6aef-130">请求</span><span class="sxs-lookup"><span data-stu-id="b6aef-130">Request</span></span>
<span data-ttu-id="b6aef-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b6aef-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="b6aef-132">响应</span><span class="sxs-lookup"><span data-stu-id="b6aef-132">Response</span></span>

<span data-ttu-id="b6aef-133">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="b6aef-133">There is no response body.</span></span>

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
