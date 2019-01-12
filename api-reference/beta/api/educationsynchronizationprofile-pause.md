---
title: 在 educationSynchronizationProfile 暂停同步
description: 暂停租户中的特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4979ed19c9a01d6a7ff2d43f7f3755d03b4b070c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950681"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="e709f-103">在 educationSynchronizationProfile 暂停同步</span><span class="sxs-lookup"><span data-stu-id="e709f-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="e709f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e709f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e709f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e709f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e709f-106">暂停的租户特定的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="e709f-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e709f-107">权限</span><span class="sxs-lookup"><span data-stu-id="e709f-107">Permissions</span></span>
<span data-ttu-id="e709f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e709f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e709f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e709f-110">Permission type</span></span> | <span data-ttu-id="e709f-111">权限</span><span class="sxs-lookup"><span data-stu-id="e709f-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e709f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e709f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e709f-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e709f-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e709f-114">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e709f-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e709f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e709f-115">Not supported.</span></span>|
|<span data-ttu-id="e709f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e709f-116">Application</span></span>|<span data-ttu-id="e709f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e709f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e709f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e709f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="e709f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e709f-119">Request headers</span></span>
| <span data-ttu-id="e709f-120">名称</span><span class="sxs-lookup"><span data-stu-id="e709f-120">Name</span></span>       | <span data-ttu-id="e709f-121">类型</span><span class="sxs-lookup"><span data-stu-id="e709f-121">Type</span></span> | <span data-ttu-id="e709f-122">说明</span><span class="sxs-lookup"><span data-stu-id="e709f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e709f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e709f-123">Authorization</span></span>  | <span data-ttu-id="e709f-124">string</span><span class="sxs-lookup"><span data-stu-id="e709f-124">string</span></span>  | <span data-ttu-id="e709f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e709f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e709f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e709f-127">Request body</span></span>
<span data-ttu-id="e709f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e709f-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e709f-129">响应</span><span class="sxs-lookup"><span data-stu-id="e709f-129">Response</span></span>
<span data-ttu-id="e709f-130">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e709f-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e709f-131">示例</span><span class="sxs-lookup"><span data-stu-id="e709f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e709f-132">请求</span><span class="sxs-lookup"><span data-stu-id="e709f-132">Request</span></span>
<span data-ttu-id="e709f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e709f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="e709f-134">响应</span><span class="sxs-lookup"><span data-stu-id="e709f-134">Response</span></span>

<span data-ttu-id="e709f-135">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="e709f-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
