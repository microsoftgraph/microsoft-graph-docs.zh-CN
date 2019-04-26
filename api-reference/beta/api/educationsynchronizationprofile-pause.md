---
title: 暂停 educationSynchronizationProfile 上的同步
description: 暂停租户中特定学校数据同步配置文件的同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e903ff08c6bb2e3a3bd56a20ca526a0b1ff42909
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324378"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="eecac-103">暂停 educationSynchronizationProfile 上的同步</span><span class="sxs-lookup"><span data-stu-id="eecac-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eecac-104">暂停租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的同步。</span><span class="sxs-lookup"><span data-stu-id="eecac-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="eecac-105">权限</span><span class="sxs-lookup"><span data-stu-id="eecac-105">Permissions</span></span>
<span data-ttu-id="eecac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eecac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eecac-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="eecac-108">Permission type</span></span> | <span data-ttu-id="eecac-109">权限</span><span class="sxs-lookup"><span data-stu-id="eecac-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="eecac-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eecac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eecac-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eecac-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="eecac-112">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="eecac-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eecac-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="eecac-113">Not supported.</span></span>|
|<span data-ttu-id="eecac-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="eecac-114">Application</span></span>|<span data-ttu-id="eecac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eecac-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eecac-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eecac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="eecac-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="eecac-117">Request headers</span></span>
| <span data-ttu-id="eecac-118">名称</span><span class="sxs-lookup"><span data-stu-id="eecac-118">Name</span></span>       | <span data-ttu-id="eecac-119">类型</span><span class="sxs-lookup"><span data-stu-id="eecac-119">Type</span></span> | <span data-ttu-id="eecac-120">说明</span><span class="sxs-lookup"><span data-stu-id="eecac-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eecac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eecac-121">Authorization</span></span>  | <span data-ttu-id="eecac-122">string</span><span class="sxs-lookup"><span data-stu-id="eecac-122">string</span></span>  | <span data-ttu-id="eecac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eecac-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eecac-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eecac-125">Request body</span></span>
<span data-ttu-id="eecac-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eecac-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eecac-127">响应</span><span class="sxs-lookup"><span data-stu-id="eecac-127">Response</span></span>
<span data-ttu-id="eecac-128">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eecac-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eecac-129">示例</span><span class="sxs-lookup"><span data-stu-id="eecac-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eecac-130">请求</span><span class="sxs-lookup"><span data-stu-id="eecac-130">Request</span></span>
<span data-ttu-id="eecac-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eecac-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="eecac-132">响应</span><span class="sxs-lookup"><span data-stu-id="eecac-132">Response</span></span>

<span data-ttu-id="eecac-133">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="eecac-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```
