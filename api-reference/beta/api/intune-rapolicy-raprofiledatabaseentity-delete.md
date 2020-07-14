---
title: 删除 raProfileDatabaseEntity
description: 删除 raProfileDatabaseEntity。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 822f2e39642425e4de153757c0c3545dbcb10ebf
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124245"
---
# <a name="delete-raprofiledatabaseentity"></a><span data-ttu-id="7b3a2-103">删除 raProfileDatabaseEntity</span><span class="sxs-lookup"><span data-stu-id="7b3a2-103">Delete raProfileDatabaseEntity</span></span>

<span data-ttu-id="7b3a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b3a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b3a2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b3a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b3a2-107">删除[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-107">Deletes a [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b3a2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b3a2-108">Prerequisites</span></span>
<span data-ttu-id="7b3a2-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7b3a2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7b3a2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b3a2-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b3a2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b3a2-111">Permission type</span></span>|<span data-ttu-id="7b3a2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b3a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b3a2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b3a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b3a2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b3a2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7b3a2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b3a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b3a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-116">Not supported.</span></span>|
|<span data-ttu-id="7b3a2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b3a2-117">Application</span></span>|<span data-ttu-id="7b3a2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b3a2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b3a2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b3a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

## <a name="request-headers"></a><span data-ttu-id="7b3a2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b3a2-120">Request headers</span></span>
|<span data-ttu-id="7b3a2-121">标头</span><span class="sxs-lookup"><span data-stu-id="7b3a2-121">Header</span></span>|<span data-ttu-id="7b3a2-122">值</span><span class="sxs-lookup"><span data-stu-id="7b3a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b3a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b3a2-123">Authorization</span></span>|<span data-ttu-id="7b3a2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b3a2-125">接受</span><span class="sxs-lookup"><span data-stu-id="7b3a2-125">Accept</span></span>|<span data-ttu-id="7b3a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b3a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b3a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b3a2-127">Request body</span></span>
<span data-ttu-id="7b3a2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b3a2-129">响应</span><span class="sxs-lookup"><span data-stu-id="7b3a2-129">Response</span></span>
<span data-ttu-id="7b3a2-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7b3a2-131">示例</span><span class="sxs-lookup"><span data-stu-id="7b3a2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b3a2-132">请求</span><span class="sxs-lookup"><span data-stu-id="7b3a2-132">Request</span></span>
<span data-ttu-id="7b3a2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b3a2-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

### <a name="response"></a><span data-ttu-id="7b3a2-134">响应</span><span class="sxs-lookup"><span data-stu-id="7b3a2-134">Response</span></span>
<span data-ttu-id="7b3a2-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7b3a2-135">Here is an example of the response.</span></span> <span data-ttu-id="7b3a2-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7b3a2-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7b3a2-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7b3a2-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



