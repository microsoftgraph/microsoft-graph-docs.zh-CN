---
title: 重置 sync educationSynchronizationProfile 上
description: 重置为租户中的特定学校数据同步配置文件同步。
author: mmast-msft
ms.openlocfilehash: 29d21318737ceba3bd380eaf20a9500a6a711857
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362438"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="65e88-103">重置 sync educationSynchronizationProfile 上</span><span class="sxs-lookup"><span data-stu-id="65e88-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="65e88-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="65e88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65e88-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="65e88-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65e88-106">重置为租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="65e88-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="65e88-107">**注意：** 此操作将导致同步重新启动。</span><span class="sxs-lookup"><span data-stu-id="65e88-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="65e88-108">遇到的任何错误都将被删除。</span><span class="sxs-lookup"><span data-stu-id="65e88-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="65e88-109">将从 Azure Active Directory (Azure AD) 中不删除任何数据。</span><span class="sxs-lookup"><span data-stu-id="65e88-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="65e88-110">权限</span><span class="sxs-lookup"><span data-stu-id="65e88-110">Permissions</span></span>
<span data-ttu-id="65e88-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65e88-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65e88-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="65e88-113">Permission type</span></span> | <span data-ttu-id="65e88-114">权限</span><span class="sxs-lookup"><span data-stu-id="65e88-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="65e88-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65e88-115">Delegated (work or school account)</span></span> | <span data-ttu-id="65e88-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65e88-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="65e88-117">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="65e88-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="65e88-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="65e88-118">Not supported.</span></span>|
|<span data-ttu-id="65e88-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="65e88-119">Application</span></span>|<span data-ttu-id="65e88-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="65e88-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e88-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65e88-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="65e88-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="65e88-122">Request headers</span></span>
| <span data-ttu-id="65e88-123">Name</span><span class="sxs-lookup"><span data-stu-id="65e88-123">Name</span></span>       | <span data-ttu-id="65e88-124">类型</span><span class="sxs-lookup"><span data-stu-id="65e88-124">Type</span></span> | <span data-ttu-id="65e88-125">说明</span><span class="sxs-lookup"><span data-stu-id="65e88-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65e88-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e88-126">Authorization</span></span>  | <span data-ttu-id="65e88-127">string</span><span class="sxs-lookup"><span data-stu-id="65e88-127">string</span></span>  | <span data-ttu-id="65e88-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65e88-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65e88-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="65e88-130">Request body</span></span>
<span data-ttu-id="65e88-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65e88-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="65e88-132">响应</span><span class="sxs-lookup"><span data-stu-id="65e88-132">Response</span></span>
<span data-ttu-id="65e88-133">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="65e88-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65e88-134">示例</span><span class="sxs-lookup"><span data-stu-id="65e88-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65e88-135">请求</span><span class="sxs-lookup"><span data-stu-id="65e88-135">Request</span></span>
<span data-ttu-id="65e88-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="65e88-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="65e88-137">响应</span><span class="sxs-lookup"><span data-stu-id="65e88-137">Response</span></span>

<span data-ttu-id="65e88-138">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="65e88-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```