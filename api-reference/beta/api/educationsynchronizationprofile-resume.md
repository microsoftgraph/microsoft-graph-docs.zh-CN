---
title: 恢复 educationSynchronizationProfile 上同步
description: 继续为租户中的特定学校数据同步配置文件同步。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c68fb6d042d92fd0f1334dc498b175c27cbc4ced
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894206"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="6cba3-103">恢复 educationSynchronizationProfile 上同步</span><span class="sxs-lookup"><span data-stu-id="6cba3-103">Resume sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="6cba3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6cba3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cba3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6cba3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cba3-106">继续为租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步。</span><span class="sxs-lookup"><span data-stu-id="6cba3-106">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cba3-107">权限</span><span class="sxs-lookup"><span data-stu-id="6cba3-107">Permissions</span></span>
<span data-ttu-id="6cba3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cba3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cba3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cba3-110">Permission type</span></span> | <span data-ttu-id="6cba3-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="6cba3-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="6cba3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cba3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6cba3-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cba3-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="6cba3-114">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="6cba3-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6cba3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cba3-115">Not supported.</span></span>|
|<span data-ttu-id="6cba3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cba3-116">Application</span></span>|<span data-ttu-id="6cba3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cba3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cba3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cba3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="6cba3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cba3-119">Request headers</span></span>
| <span data-ttu-id="6cba3-120">名称</span><span class="sxs-lookup"><span data-stu-id="6cba3-120">Name</span></span>       | <span data-ttu-id="6cba3-121">类型</span><span class="sxs-lookup"><span data-stu-id="6cba3-121">Type</span></span> | <span data-ttu-id="6cba3-122">说明</span><span class="sxs-lookup"><span data-stu-id="6cba3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6cba3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cba3-123">Authorization</span></span>  | <span data-ttu-id="6cba3-124">string</span><span class="sxs-lookup"><span data-stu-id="6cba3-124">string</span></span>  | <span data-ttu-id="6cba3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cba3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cba3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cba3-127">Request body</span></span>
<span data-ttu-id="6cba3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cba3-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6cba3-129">响应</span><span class="sxs-lookup"><span data-stu-id="6cba3-129">Response</span></span>
<span data-ttu-id="6cba3-130">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6cba3-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6cba3-131">示例</span><span class="sxs-lookup"><span data-stu-id="6cba3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cba3-132">请求</span><span class="sxs-lookup"><span data-stu-id="6cba3-132">Request</span></span>
<span data-ttu-id="6cba3-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6cba3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="6cba3-134">响应</span><span class="sxs-lookup"><span data-stu-id="6cba3-134">Response</span></span>

<span data-ttu-id="6cba3-135">没有响应正文。</span><span class="sxs-lookup"><span data-stu-id="6cba3-135">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
