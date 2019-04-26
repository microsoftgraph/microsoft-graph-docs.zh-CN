---
title: 在 educationSynchronizationProfile 上重置同步
description: 在租户中重置特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ccf257a2fc479f87d1e0b6d2b6414d0e3431fcb6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322296"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="e8b2e-103">在 educationSynchronizationProfile 上重置同步</span><span class="sxs-lookup"><span data-stu-id="e8b2e-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8b2e-104">在租户中重置特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="e8b2e-105">**注意:** 此操作将导致重新启动同步。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="e8b2e-106">遇到的任何错误都将被删除。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="e8b2e-107">将不会从 azure Active Directory (azure AD) 中删除任何数据。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e8b2e-108">权限</span><span class="sxs-lookup"><span data-stu-id="e8b2e-108">Permissions</span></span>
<span data-ttu-id="e8b2e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8b2e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8b2e-111">Permission type</span></span> | <span data-ttu-id="e8b2e-112">权限</span><span class="sxs-lookup"><span data-stu-id="e8b2e-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e8b2e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8b2e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e8b2e-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8b2e-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e8b2e-115">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e8b2e-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e8b2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-116">Not supported.</span></span>|
|<span data-ttu-id="e8b2e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8b2e-117">Application</span></span>|<span data-ttu-id="e8b2e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8b2e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8b2e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="e8b2e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8b2e-120">Request headers</span></span>
| <span data-ttu-id="e8b2e-121">名称</span><span class="sxs-lookup"><span data-stu-id="e8b2e-121">Name</span></span>       | <span data-ttu-id="e8b2e-122">类型</span><span class="sxs-lookup"><span data-stu-id="e8b2e-122">Type</span></span> | <span data-ttu-id="e8b2e-123">说明</span><span class="sxs-lookup"><span data-stu-id="e8b2e-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8b2e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8b2e-124">Authorization</span></span>  | <span data-ttu-id="e8b2e-125">string</span><span class="sxs-lookup"><span data-stu-id="e8b2e-125">string</span></span>  | <span data-ttu-id="e8b2e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8b2e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8b2e-128">Request body</span></span>
<span data-ttu-id="e8b2e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e8b2e-130">响应</span><span class="sxs-lookup"><span data-stu-id="e8b2e-130">Response</span></span>
<span data-ttu-id="e8b2e-131">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8b2e-132">示例</span><span class="sxs-lookup"><span data-stu-id="e8b2e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8b2e-133">请求</span><span class="sxs-lookup"><span data-stu-id="e8b2e-133">Request</span></span>
<span data-ttu-id="e8b2e-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="e8b2e-135">响应</span><span class="sxs-lookup"><span data-stu-id="e8b2e-135">Response</span></span>

<span data-ttu-id="e8b2e-136">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="e8b2e-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
