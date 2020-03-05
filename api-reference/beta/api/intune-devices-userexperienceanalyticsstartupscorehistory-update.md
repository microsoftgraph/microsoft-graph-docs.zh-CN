---
title: 更新 userExperienceAnalyticsStartupScoreHistory
description: 更新 userExperienceAnalyticsStartupScoreHistory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4645c627a54f0476c0928bb5bfd2267a04741fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467954"
---
# <a name="update-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="6d95b-103">更新 userExperienceAnalyticsStartupScoreHistory</span><span class="sxs-lookup"><span data-stu-id="6d95b-103">Update userExperienceAnalyticsStartupScoreHistory</span></span>

<span data-ttu-id="6d95b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6d95b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d95b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d95b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d95b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d95b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d95b-107">更新[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6d95b-107">Update the properties of a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d95b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d95b-108">Prerequisites</span></span>
<span data-ttu-id="6d95b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d95b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d95b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d95b-111">Permission type</span></span>|<span data-ttu-id="6d95b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6d95b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d95b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d95b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d95b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d95b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6d95b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d95b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d95b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d95b-116">Not supported.</span></span>|
|<span data-ttu-id="6d95b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d95b-117">Application</span></span>|<span data-ttu-id="6d95b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d95b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d95b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d95b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="6d95b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d95b-120">Request headers</span></span>
|<span data-ttu-id="6d95b-121">标头</span><span class="sxs-lookup"><span data-stu-id="6d95b-121">Header</span></span>|<span data-ttu-id="6d95b-122">值</span><span class="sxs-lookup"><span data-stu-id="6d95b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d95b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d95b-123">Authorization</span></span>|<span data-ttu-id="6d95b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6d95b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d95b-125">接受</span><span class="sxs-lookup"><span data-stu-id="6d95b-125">Accept</span></span>|<span data-ttu-id="6d95b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d95b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d95b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d95b-127">Request body</span></span>
<span data-ttu-id="6d95b-128">在请求正文中，提供[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d95b-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

<span data-ttu-id="6d95b-129">下表显示创建[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6d95b-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).</span></span>

|<span data-ttu-id="6d95b-130">属性</span><span class="sxs-lookup"><span data-stu-id="6d95b-130">Property</span></span>|<span data-ttu-id="6d95b-131">类型</span><span class="sxs-lookup"><span data-stu-id="6d95b-131">Type</span></span>|<span data-ttu-id="6d95b-132">说明</span><span class="sxs-lookup"><span data-stu-id="6d95b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d95b-133">id</span><span class="sxs-lookup"><span data-stu-id="6d95b-133">id</span></span>|<span data-ttu-id="6d95b-134">String</span><span class="sxs-lookup"><span data-stu-id="6d95b-134">String</span></span>|<span data-ttu-id="6d95b-135">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6d95b-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="6d95b-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="6d95b-136">startupDateTime</span></span>|<span data-ttu-id="6d95b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d95b-137">DateTimeOffset</span></span>|<span data-ttu-id="6d95b-138">User experience analytics 设备启动日期时间。</span><span class="sxs-lookup"><span data-stu-id="6d95b-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="6d95b-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="6d95b-139">startupScore</span></span>|<span data-ttu-id="6d95b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6d95b-140">Int32</span></span>|<span data-ttu-id="6d95b-141">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="6d95b-141">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="6d95b-142">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="6d95b-142">coreBootScore</span></span>|<span data-ttu-id="6d95b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6d95b-143">Int32</span></span>|<span data-ttu-id="6d95b-144">用户体验分析设备核心启动分数。</span><span class="sxs-lookup"><span data-stu-id="6d95b-144">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="6d95b-145">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="6d95b-145">coreSigninScore</span></span>|<span data-ttu-id="6d95b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6d95b-146">Int32</span></span>|<span data-ttu-id="6d95b-147">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="6d95b-147">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="6d95b-148">响应</span><span class="sxs-lookup"><span data-stu-id="6d95b-148">Response</span></span>
<span data-ttu-id="6d95b-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6d95b-149">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d95b-150">示例</span><span class="sxs-lookup"><span data-stu-id="6d95b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d95b-151">请求</span><span class="sxs-lookup"><span data-stu-id="6d95b-151">Request</span></span>
<span data-ttu-id="6d95b-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d95b-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15
}
```

### <a name="response"></a><span data-ttu-id="6d95b-153">响应</span><span class="sxs-lookup"><span data-stu-id="6d95b-153">Response</span></span>
<span data-ttu-id="6d95b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d95b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "52efee0b-ee0b-52ef-0bee-ef520beeef52",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15
}
```





