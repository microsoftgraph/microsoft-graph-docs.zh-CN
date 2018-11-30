---
title: 重置 sync educationSynchronizationProfile 上
description: 重置为租户中的特定学校数据同步配置文件同步。
ms.openlocfilehash: 4be91b7d6229148c51dc8fb1279a9078fb5cad7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046047"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="acc0f-103">重置 sync educationSynchronizationProfile 上</span><span class="sxs-lookup"><span data-stu-id="acc0f-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="acc0f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="acc0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acc0f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="acc0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acc0f-106">重置为租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="acc0f-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="acc0f-107">**注意：** 此操作将导致同步重新启动。</span><span class="sxs-lookup"><span data-stu-id="acc0f-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="acc0f-108">遇到的任何错误都将被删除。</span><span class="sxs-lookup"><span data-stu-id="acc0f-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="acc0f-109">将从 Azure Active Directory (Azure AD) 中不删除任何数据。</span><span class="sxs-lookup"><span data-stu-id="acc0f-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="acc0f-110">权限</span><span class="sxs-lookup"><span data-stu-id="acc0f-110">Permissions</span></span>
<span data-ttu-id="acc0f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acc0f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="acc0f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="acc0f-113">Permission type</span></span> | <span data-ttu-id="acc0f-114">Permissions</span><span class="sxs-lookup"><span data-stu-id="acc0f-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="acc0f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acc0f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="acc0f-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acc0f-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="acc0f-117">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="acc0f-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="acc0f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="acc0f-118">Not supported.</span></span>|
|<span data-ttu-id="acc0f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="acc0f-119">Application</span></span>|<span data-ttu-id="acc0f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="acc0f-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acc0f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acc0f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="acc0f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="acc0f-122">Request headers</span></span>
| <span data-ttu-id="acc0f-123">名称</span><span class="sxs-lookup"><span data-stu-id="acc0f-123">Name</span></span>       | <span data-ttu-id="acc0f-124">类型</span><span class="sxs-lookup"><span data-stu-id="acc0f-124">Type</span></span> | <span data-ttu-id="acc0f-125">说明</span><span class="sxs-lookup"><span data-stu-id="acc0f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="acc0f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="acc0f-126">Authorization</span></span>  | <span data-ttu-id="acc0f-127">string</span><span class="sxs-lookup"><span data-stu-id="acc0f-127">string</span></span>  | <span data-ttu-id="acc0f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="acc0f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="acc0f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="acc0f-130">Request body</span></span>
<span data-ttu-id="acc0f-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="acc0f-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="acc0f-132">响应</span><span class="sxs-lookup"><span data-stu-id="acc0f-132">Response</span></span>
<span data-ttu-id="acc0f-133">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="acc0f-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="acc0f-134">示例</span><span class="sxs-lookup"><span data-stu-id="acc0f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acc0f-135">请求</span><span class="sxs-lookup"><span data-stu-id="acc0f-135">Request</span></span>
<span data-ttu-id="acc0f-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="acc0f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="acc0f-137">响应</span><span class="sxs-lookup"><span data-stu-id="acc0f-137">Response</span></span>

<span data-ttu-id="acc0f-138">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="acc0f-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```