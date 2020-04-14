---
title: 更新 userExperienceAnalyticsScoreHistory
description: 更新 userExperienceAnalyticsScoreHistory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b44ee2dcbade774c704a7c5d1df1ae31e9423c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378824"
---
# <a name="update-userexperienceanalyticsscorehistory"></a><span data-ttu-id="ffb08-103">更新 userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="ffb08-103">Update userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="ffb08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffb08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffb08-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ffb08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffb08-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ffb08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffb08-107">更新[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ffb08-107">Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffb08-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ffb08-108">Prerequisites</span></span>
<span data-ttu-id="ffb08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffb08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffb08-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffb08-111">Permission type</span></span>|<span data-ttu-id="ffb08-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ffb08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffb08-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffb08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffb08-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb08-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ffb08-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffb08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffb08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffb08-116">Not supported.</span></span>|
|<span data-ttu-id="ffb08-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffb08-117">Application</span></span>|<span data-ttu-id="ffb08-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb08-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffb08-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffb08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="ffb08-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffb08-120">Request headers</span></span>
|<span data-ttu-id="ffb08-121">标头</span><span class="sxs-lookup"><span data-stu-id="ffb08-121">Header</span></span>|<span data-ttu-id="ffb08-122">值</span><span class="sxs-lookup"><span data-stu-id="ffb08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffb08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffb08-123">Authorization</span></span>|<span data-ttu-id="ffb08-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ffb08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffb08-125">接受</span><span class="sxs-lookup"><span data-stu-id="ffb08-125">Accept</span></span>|<span data-ttu-id="ffb08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb08-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffb08-127">Request body</span></span>
<span data-ttu-id="ffb08-128">在请求正文中，提供[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffb08-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

<span data-ttu-id="ffb08-129">下表显示创建[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ffb08-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span></span>

|<span data-ttu-id="ffb08-130">属性</span><span class="sxs-lookup"><span data-stu-id="ffb08-130">Property</span></span>|<span data-ttu-id="ffb08-131">类型</span><span class="sxs-lookup"><span data-stu-id="ffb08-131">Type</span></span>|<span data-ttu-id="ffb08-132">说明</span><span class="sxs-lookup"><span data-stu-id="ffb08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffb08-133">id</span><span class="sxs-lookup"><span data-stu-id="ffb08-133">id</span></span>|<span data-ttu-id="ffb08-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ffb08-134">String</span></span>|<span data-ttu-id="ffb08-135">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ffb08-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="ffb08-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb08-136">startupDateTime</span></span>|<span data-ttu-id="ffb08-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb08-137">DateTimeOffset</span></span>|<span data-ttu-id="ffb08-138">User experience analytics 设备启动日期时间。</span><span class="sxs-lookup"><span data-stu-id="ffb08-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="ffb08-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="ffb08-139">startupScore</span></span>|<span data-ttu-id="ffb08-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ffb08-140">Int32</span></span>|<span data-ttu-id="ffb08-141">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="ffb08-141">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="ffb08-142">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="ffb08-142">coreBootScore</span></span>|<span data-ttu-id="ffb08-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ffb08-143">Int32</span></span>|<span data-ttu-id="ffb08-144">用户体验分析设备核心启动分数。</span><span class="sxs-lookup"><span data-stu-id="ffb08-144">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="ffb08-145">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="ffb08-145">coreSigninScore</span></span>|<span data-ttu-id="ffb08-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ffb08-146">Int32</span></span>|<span data-ttu-id="ffb08-147">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="ffb08-147">The User experience analytics device core sign-in score.</span></span>|
|<span data-ttu-id="ffb08-148">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="ffb08-148">recommendedSoftwareScore</span></span>|<span data-ttu-id="ffb08-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ffb08-149">Int32</span></span>|<span data-ttu-id="ffb08-150">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="ffb08-150">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="ffb08-151">响应</span><span class="sxs-lookup"><span data-stu-id="ffb08-151">Response</span></span>
<span data-ttu-id="ffb08-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffb08-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb08-153">示例</span><span class="sxs-lookup"><span data-stu-id="ffb08-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffb08-154">请求</span><span class="sxs-lookup"><span data-stu-id="ffb08-154">Request</span></span>
<span data-ttu-id="ffb08-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffb08-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 243

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8
}
```

### <a name="response"></a><span data-ttu-id="ffb08-156">响应</span><span class="sxs-lookup"><span data-stu-id="ffb08-156">Response</span></span>
<span data-ttu-id="ffb08-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffb08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8
}
```



