---
title: 更新 userExperienceAnalyticsScoreHistory
description: 更新 userExperienceAnalyticsScoreHistory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62f6243b6241901ee330ceb855bd3886db8cdc27
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49263699"
---
# <a name="update-userexperienceanalyticsscorehistory"></a><span data-ttu-id="8c258-103">更新 userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="8c258-103">Update userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="8c258-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c258-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c258-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c258-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c258-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c258-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c258-107">更新 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c258-107">Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c258-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c258-108">Prerequisites</span></span>
<span data-ttu-id="8c258-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c258-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c258-111">Permission type</span></span>|<span data-ttu-id="8c258-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c258-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c258-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c258-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c258-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c258-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8c258-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c258-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c258-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c258-116">Not supported.</span></span>|
|<span data-ttu-id="8c258-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c258-117">Application</span></span>|<span data-ttu-id="8c258-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c258-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c258-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c258-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="8c258-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c258-120">Request headers</span></span>
|<span data-ttu-id="8c258-121">标头</span><span class="sxs-lookup"><span data-stu-id="8c258-121">Header</span></span>|<span data-ttu-id="8c258-122">值</span><span class="sxs-lookup"><span data-stu-id="8c258-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c258-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c258-123">Authorization</span></span>|<span data-ttu-id="8c258-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c258-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c258-125">接受</span><span class="sxs-lookup"><span data-stu-id="8c258-125">Accept</span></span>|<span data-ttu-id="8c258-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c258-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c258-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c258-127">Request body</span></span>
<span data-ttu-id="8c258-128">在请求正文中，提供 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c258-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

<span data-ttu-id="8c258-129">下表显示创建 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c258-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span></span>

|<span data-ttu-id="8c258-130">属性</span><span class="sxs-lookup"><span data-stu-id="8c258-130">Property</span></span>|<span data-ttu-id="8c258-131">类型</span><span class="sxs-lookup"><span data-stu-id="8c258-131">Type</span></span>|<span data-ttu-id="8c258-132">说明</span><span class="sxs-lookup"><span data-stu-id="8c258-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c258-133">id</span><span class="sxs-lookup"><span data-stu-id="8c258-133">id</span></span>|<span data-ttu-id="8c258-134">String</span><span class="sxs-lookup"><span data-stu-id="8c258-134">String</span></span>|<span data-ttu-id="8c258-135">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8c258-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="8c258-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="8c258-136">startupDateTime</span></span>|<span data-ttu-id="8c258-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c258-137">DateTimeOffset</span></span>|<span data-ttu-id="8c258-138">User experience analytics 设备启动日期时间。</span><span class="sxs-lookup"><span data-stu-id="8c258-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="8c258-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="8c258-139">startupScore</span></span>|<span data-ttu-id="8c258-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8c258-140">Int32</span></span>|<span data-ttu-id="8c258-141">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-141">User experience analytics device startup score.</span></span> <span data-ttu-id="8c258-142">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-142">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8c258-143">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="8c258-143">coreBootScore</span></span>|<span data-ttu-id="8c258-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8c258-144">Int32</span></span>|<span data-ttu-id="8c258-145">用户体验分析设备核心启动分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-145">The user experience analytics device core boot score.</span></span> <span data-ttu-id="8c258-146">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-146">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8c258-147">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="8c258-147">coreSigninScore</span></span>|<span data-ttu-id="8c258-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8c258-148">Int32</span></span>|<span data-ttu-id="8c258-149">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-149">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="8c258-150">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-150">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8c258-151">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="8c258-151">recommendedSoftwareScore</span></span>|<span data-ttu-id="8c258-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8c258-152">Int32</span></span>|<span data-ttu-id="8c258-153">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-153">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="8c258-154">分数将在范围0-100，100是理想的分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-154">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8c258-155">restartScore</span><span class="sxs-lookup"><span data-stu-id="8c258-155">restartScore</span></span>|<span data-ttu-id="8c258-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8c258-156">Int32</span></span>|<span data-ttu-id="8c258-157">重启分数。</span><span class="sxs-lookup"><span data-stu-id="8c258-157">Restart score.</span></span> <span data-ttu-id="8c258-158">分数将在范围0-100，100为理想分数，0表示重新启动过多。</span><span class="sxs-lookup"><span data-stu-id="8c258-158">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="8c258-159">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="8c258-159">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="8c258-160">响应</span><span class="sxs-lookup"><span data-stu-id="8c258-160">Response</span></span>
<span data-ttu-id="8c258-161">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c258-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c258-162">示例</span><span class="sxs-lookup"><span data-stu-id="8c258-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c258-163">请求</span><span class="sxs-lookup"><span data-stu-id="8c258-163">Request</span></span>
<span data-ttu-id="8c258-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c258-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
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

### <a name="response"></a><span data-ttu-id="8c258-165">响应</span><span class="sxs-lookup"><span data-stu-id="8c258-165">Response</span></span>
<span data-ttu-id="8c258-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c258-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




