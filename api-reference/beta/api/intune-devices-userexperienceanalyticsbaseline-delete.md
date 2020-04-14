---
title: 删除 userExperienceAnalyticsBaseline
description: 删除 userExperienceAnalyticsBaseline。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1ac6be7e1646536c0ecbd0f38841965714292d6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43323219"
---
# <a name="delete-userexperienceanalyticsbaseline"></a><span data-ttu-id="05691-103">删除 userExperienceAnalyticsBaseline</span><span class="sxs-lookup"><span data-stu-id="05691-103">Delete userExperienceAnalyticsBaseline</span></span>

<span data-ttu-id="05691-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05691-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05691-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05691-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05691-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05691-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05691-107">删除[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)。</span><span class="sxs-lookup"><span data-stu-id="05691-107">Deletes a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05691-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="05691-108">Prerequisites</span></span>
<span data-ttu-id="05691-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05691-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="05691-111">Permission type</span></span>|<span data-ttu-id="05691-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05691-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05691-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05691-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05691-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05691-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="05691-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05691-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05691-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05691-116">Not supported.</span></span>|
|<span data-ttu-id="05691-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="05691-117">Application</span></span>|<span data-ttu-id="05691-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05691-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05691-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05691-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="05691-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05691-120">Request headers</span></span>
|<span data-ttu-id="05691-121">标头</span><span class="sxs-lookup"><span data-stu-id="05691-121">Header</span></span>|<span data-ttu-id="05691-122">值</span><span class="sxs-lookup"><span data-stu-id="05691-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05691-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05691-123">Authorization</span></span>|<span data-ttu-id="05691-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05691-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05691-125">接受</span><span class="sxs-lookup"><span data-stu-id="05691-125">Accept</span></span>|<span data-ttu-id="05691-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05691-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05691-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05691-127">Request body</span></span>
<span data-ttu-id="05691-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05691-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05691-129">响应</span><span class="sxs-lookup"><span data-stu-id="05691-129">Response</span></span>
<span data-ttu-id="05691-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="05691-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="05691-131">示例</span><span class="sxs-lookup"><span data-stu-id="05691-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="05691-132">请求</span><span class="sxs-lookup"><span data-stu-id="05691-132">Request</span></span>
<span data-ttu-id="05691-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05691-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

### <a name="response"></a><span data-ttu-id="05691-134">响应</span><span class="sxs-lookup"><span data-stu-id="05691-134">Response</span></span>
<span data-ttu-id="05691-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05691-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



