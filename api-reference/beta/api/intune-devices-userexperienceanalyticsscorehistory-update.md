---
title: 更新 userExperienceAnalyticsScoreHistory
description: 更新 userExperienceAnalyticsScoreHistory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af10809804f933b9a049ae37dad4aecfa2bf0c9e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666231"
---
# <a name="update-userexperienceanalyticsscorehistory"></a><span data-ttu-id="3857b-103">更新 userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="3857b-103">Update userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="3857b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3857b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3857b-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3857b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3857b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3857b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3857b-107">更新 [userExperienceAnalyticsScoreHistory 对象](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="3857b-107">Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3857b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3857b-108">Prerequisites</span></span>
<span data-ttu-id="3857b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3857b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3857b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3857b-111">Permission type</span></span>|<span data-ttu-id="3857b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3857b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3857b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3857b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3857b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3857b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3857b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3857b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3857b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3857b-116">Not supported.</span></span>|
|<span data-ttu-id="3857b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3857b-117">Application</span></span>|<span data-ttu-id="3857b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3857b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3857b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3857b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="3857b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3857b-120">Request headers</span></span>
|<span data-ttu-id="3857b-121">标头</span><span class="sxs-lookup"><span data-stu-id="3857b-121">Header</span></span>|<span data-ttu-id="3857b-122">值</span><span class="sxs-lookup"><span data-stu-id="3857b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3857b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3857b-123">Authorization</span></span>|<span data-ttu-id="3857b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3857b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3857b-125">接受</span><span class="sxs-lookup"><span data-stu-id="3857b-125">Accept</span></span>|<span data-ttu-id="3857b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3857b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3857b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3857b-127">Request body</span></span>
<span data-ttu-id="3857b-128">在请求正文中，提供 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3857b-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

<span data-ttu-id="3857b-129">下表显示创建 [userExperienceAnalyticsScoreHistory 时所需的属性](../resources/intune-devices-userexperienceanalyticsscorehistory.md)。</span><span class="sxs-lookup"><span data-stu-id="3857b-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span></span>

|<span data-ttu-id="3857b-130">属性</span><span class="sxs-lookup"><span data-stu-id="3857b-130">Property</span></span>|<span data-ttu-id="3857b-131">类型</span><span class="sxs-lookup"><span data-stu-id="3857b-131">Type</span></span>|<span data-ttu-id="3857b-132">说明</span><span class="sxs-lookup"><span data-stu-id="3857b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3857b-133">id</span><span class="sxs-lookup"><span data-stu-id="3857b-133">id</span></span>|<span data-ttu-id="3857b-134">String</span><span class="sxs-lookup"><span data-stu-id="3857b-134">String</span></span>|<span data-ttu-id="3857b-135">用户体验分析设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3857b-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="3857b-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="3857b-136">startupDateTime</span></span>|<span data-ttu-id="3857b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3857b-137">DateTimeOffset</span></span>|<span data-ttu-id="3857b-138">用户体验分析设备启动日期时间。</span><span class="sxs-lookup"><span data-stu-id="3857b-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="3857b-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="3857b-139">overallScore</span></span>|<span data-ttu-id="3857b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3857b-140">Int32</span></span>|<span data-ttu-id="3857b-141">用户体验分析总体分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-141">User experience analytics overall score.</span></span> <span data-ttu-id="3857b-142">分数范围为 0-100，100 是理想分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-142">Score will be in the range 0-100, 100 is the ideal score.</span></span> <span data-ttu-id="3857b-143">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="3857b-143">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3857b-144">startupScore</span><span class="sxs-lookup"><span data-stu-id="3857b-144">startupScore</span></span>|<span data-ttu-id="3857b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3857b-145">Int32</span></span>|<span data-ttu-id="3857b-146">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-146">User experience analytics device startup score.</span></span> <span data-ttu-id="3857b-147">分数范围为 0-100，100 是理想分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-147">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3857b-148">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="3857b-148">coreBootScore</span></span>|<span data-ttu-id="3857b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3857b-149">Int32</span></span>|<span data-ttu-id="3857b-150">用户体验分析设备核心启动分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-150">The user experience analytics device core boot score.</span></span> <span data-ttu-id="3857b-151">分数范围为 0-100，100 是理想分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-151">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3857b-152">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="3857b-152">coreSigninScore</span></span>|<span data-ttu-id="3857b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3857b-153">Int32</span></span>|<span data-ttu-id="3857b-154">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-154">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="3857b-155">分数范围为 0-100，100 是理想分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-155">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3857b-156">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="3857b-156">recommendedSoftwareScore</span></span>|<span data-ttu-id="3857b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3857b-157">Int32</span></span>|<span data-ttu-id="3857b-158">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-158">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="3857b-159">分数范围为 0-100，100 是理想分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-159">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="3857b-160">restartScore</span><span class="sxs-lookup"><span data-stu-id="3857b-160">restartScore</span></span>|<span data-ttu-id="3857b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3857b-161">Int32</span></span>|<span data-ttu-id="3857b-162">重启分数。</span><span class="sxs-lookup"><span data-stu-id="3857b-162">Restart score.</span></span> <span data-ttu-id="3857b-163">分数将在 0-100 之间，100 是理想分数，0 表示重启过多。</span><span class="sxs-lookup"><span data-stu-id="3857b-163">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="3857b-164">有效值为 0 到 9999999</span><span class="sxs-lookup"><span data-stu-id="3857b-164">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="3857b-165">响应</span><span class="sxs-lookup"><span data-stu-id="3857b-165">Response</span></span>
<span data-ttu-id="3857b-166">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3857b-166">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3857b-167">示例</span><span class="sxs-lookup"><span data-stu-id="3857b-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="3857b-168">请求</span><span class="sxs-lookup"><span data-stu-id="3857b-168">Request</span></span>
<span data-ttu-id="3857b-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3857b-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```

### <a name="response"></a><span data-ttu-id="3857b-170">响应</span><span class="sxs-lookup"><span data-stu-id="3857b-170">Response</span></span>
<span data-ttu-id="3857b-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3857b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```




