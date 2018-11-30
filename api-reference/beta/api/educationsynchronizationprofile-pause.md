---
title: 在 educationSynchronizationProfile 暂停同步
description: 暂停租户中的特定学校数据同步配置文件的同步。
ms.openlocfilehash: ee2ed2133619bbcded7a31afece55191a0cfd4e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041938"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="23010-103">在 educationSynchronizationProfile 暂停同步</span><span class="sxs-lookup"><span data-stu-id="23010-103">Pause sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="23010-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="23010-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23010-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23010-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23010-106">暂停的租户特定的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="23010-106">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="23010-107">权限</span><span class="sxs-lookup"><span data-stu-id="23010-107">Permissions</span></span>
<span data-ttu-id="23010-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23010-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23010-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="23010-110">Permission type</span></span> | <span data-ttu-id="23010-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="23010-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="23010-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23010-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23010-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23010-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="23010-114">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="23010-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="23010-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="23010-115">Not supported.</span></span>|
|<span data-ttu-id="23010-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="23010-116">Application</span></span>|<span data-ttu-id="23010-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="23010-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23010-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23010-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="23010-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="23010-119">Request headers</span></span>
| <span data-ttu-id="23010-120">名称</span><span class="sxs-lookup"><span data-stu-id="23010-120">Name</span></span>       | <span data-ttu-id="23010-121">类型</span><span class="sxs-lookup"><span data-stu-id="23010-121">Type</span></span> | <span data-ttu-id="23010-122">说明</span><span class="sxs-lookup"><span data-stu-id="23010-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23010-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23010-123">Authorization</span></span>  | <span data-ttu-id="23010-124">string</span><span class="sxs-lookup"><span data-stu-id="23010-124">string</span></span>  | <span data-ttu-id="23010-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23010-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23010-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="23010-127">Request body</span></span>
<span data-ttu-id="23010-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23010-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="23010-129">响应</span><span class="sxs-lookup"><span data-stu-id="23010-129">Response</span></span>
<span data-ttu-id="23010-130">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="23010-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="23010-131">示例</span><span class="sxs-lookup"><span data-stu-id="23010-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23010-132">请求</span><span class="sxs-lookup"><span data-stu-id="23010-132">Request</span></span>
<span data-ttu-id="23010-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="23010-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="23010-134">响应</span><span class="sxs-lookup"><span data-stu-id="23010-134">Response</span></span>

<span data-ttu-id="23010-135">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="23010-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```