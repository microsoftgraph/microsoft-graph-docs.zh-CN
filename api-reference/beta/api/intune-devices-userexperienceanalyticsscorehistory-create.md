---
title: 创建 userExperienceAnalyticsScoreHistory
description: 创建新的 userExperienceAnalyticsScoreHistory 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1a6d5275a8214f5698a41a711c1b82b1e48b960
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792658"
---
# <a name="create-userexperienceanalyticsscorehistory"></a><span data-ttu-id="e2653-103">创建 userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="e2653-103">Create userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="e2653-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2653-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2653-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2653-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2653-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2653-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2653-107">创建新的 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2653-107">Create a new [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2653-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2653-108">Prerequisites</span></span>
<span data-ttu-id="e2653-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2653-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2653-111">Permission type</span></span>|<span data-ttu-id="e2653-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e2653-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2653-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2653-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2653-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2653-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e2653-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2653-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2653-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2653-116">Not supported.</span></span>|
|<span data-ttu-id="e2653-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2653-117">Application</span></span>|<span data-ttu-id="e2653-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2653-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2653-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2653-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="e2653-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2653-120">Request headers</span></span>
|<span data-ttu-id="e2653-121">标头</span><span class="sxs-lookup"><span data-stu-id="e2653-121">Header</span></span>|<span data-ttu-id="e2653-122">值</span><span class="sxs-lookup"><span data-stu-id="e2653-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2653-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2653-123">Authorization</span></span>|<span data-ttu-id="e2653-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2653-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2653-125">接受</span><span class="sxs-lookup"><span data-stu-id="e2653-125">Accept</span></span>|<span data-ttu-id="e2653-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2653-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2653-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2653-127">Request body</span></span>
<span data-ttu-id="e2653-128">在请求正文中，提供 userExperienceAnalyticsScoreHistory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2653-128">In the request body, supply a JSON representation for the userExperienceAnalyticsScoreHistory object.</span></span>

<span data-ttu-id="e2653-129">下表显示创建 userExperienceAnalyticsScoreHistory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e2653-129">The following table shows the properties that are required when you create the userExperienceAnalyticsScoreHistory.</span></span>

|<span data-ttu-id="e2653-130">属性</span><span class="sxs-lookup"><span data-stu-id="e2653-130">Property</span></span>|<span data-ttu-id="e2653-131">类型</span><span class="sxs-lookup"><span data-stu-id="e2653-131">Type</span></span>|<span data-ttu-id="e2653-132">说明</span><span class="sxs-lookup"><span data-stu-id="e2653-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2653-133">id</span><span class="sxs-lookup"><span data-stu-id="e2653-133">id</span></span>|<span data-ttu-id="e2653-134">String</span><span class="sxs-lookup"><span data-stu-id="e2653-134">String</span></span>|<span data-ttu-id="e2653-135">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e2653-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="e2653-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="e2653-136">startupDateTime</span></span>|<span data-ttu-id="e2653-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2653-137">DateTimeOffset</span></span>|<span data-ttu-id="e2653-138">User experience analytics 设备启动日期时间。</span><span class="sxs-lookup"><span data-stu-id="e2653-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="e2653-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="e2653-139">startupScore</span></span>|<span data-ttu-id="e2653-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e2653-140">Int32</span></span>|<span data-ttu-id="e2653-141">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-141">User experience analytics device startup score.</span></span> <span data-ttu-id="e2653-142">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-142">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e2653-143">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="e2653-143">coreBootScore</span></span>|<span data-ttu-id="e2653-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e2653-144">Int32</span></span>|<span data-ttu-id="e2653-145">用户体验分析设备核心启动分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-145">The user experience analytics device core boot score.</span></span> <span data-ttu-id="e2653-146">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-146">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e2653-147">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="e2653-147">coreSigninScore</span></span>|<span data-ttu-id="e2653-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e2653-148">Int32</span></span>|<span data-ttu-id="e2653-149">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-149">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="e2653-150">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-150">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e2653-151">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="e2653-151">recommendedSoftwareScore</span></span>|<span data-ttu-id="e2653-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e2653-152">Int32</span></span>|<span data-ttu-id="e2653-153">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-153">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="e2653-154">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-154">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="e2653-155">restartScore</span><span class="sxs-lookup"><span data-stu-id="e2653-155">restartScore</span></span>|<span data-ttu-id="e2653-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e2653-156">Int32</span></span>|<span data-ttu-id="e2653-157">重启分数。</span><span class="sxs-lookup"><span data-stu-id="e2653-157">Restart score.</span></span> <span data-ttu-id="e2653-158">分数将在范围0-100，100为理想分数，0表示重新启动过多。</span><span class="sxs-lookup"><span data-stu-id="e2653-158">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="e2653-159">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="e2653-159">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="e2653-160">响应</span><span class="sxs-lookup"><span data-stu-id="e2653-160">Response</span></span>
<span data-ttu-id="e2653-161">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2653-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2653-162">示例</span><span class="sxs-lookup"><span data-stu-id="e2653-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2653-163">请求</span><span class="sxs-lookup"><span data-stu-id="e2653-163">Request</span></span>
<span data-ttu-id="e2653-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2653-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```

### <a name="response"></a><span data-ttu-id="e2653-165">响应</span><span class="sxs-lookup"><span data-stu-id="e2653-165">Response</span></span>
<span data-ttu-id="e2653-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2653-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```



