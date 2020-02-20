---
title: 更新 userExperienceAnalyticsStartupScoreHistory
description: 更新 userExperienceAnalyticsStartupScoreHistory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b3c49164ef636ad7822ca4c82bd81802ea37431
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160932"
---
# <a name="update-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="a2881-103">更新 userExperienceAnalyticsStartupScoreHistory</span><span class="sxs-lookup"><span data-stu-id="a2881-103">Update userExperienceAnalyticsStartupScoreHistory</span></span>

> <span data-ttu-id="a2881-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2881-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2881-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2881-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2881-106">更新[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2881-106">Update the properties of a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2881-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2881-107">Prerequisites</span></span>
<span data-ttu-id="a2881-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2881-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2881-110">Permission type</span></span>|<span data-ttu-id="a2881-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2881-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2881-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2881-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2881-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2881-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2881-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2881-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2881-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2881-115">Not supported.</span></span>|
|<span data-ttu-id="a2881-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2881-116">Application</span></span>|<span data-ttu-id="a2881-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2881-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2881-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2881-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a2881-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2881-119">Request headers</span></span>
|<span data-ttu-id="a2881-120">标头</span><span class="sxs-lookup"><span data-stu-id="a2881-120">Header</span></span>|<span data-ttu-id="a2881-121">值</span><span class="sxs-lookup"><span data-stu-id="a2881-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2881-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2881-122">Authorization</span></span>|<span data-ttu-id="a2881-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2881-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2881-124">接受</span><span class="sxs-lookup"><span data-stu-id="a2881-124">Accept</span></span>|<span data-ttu-id="a2881-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2881-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2881-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2881-126">Request body</span></span>
<span data-ttu-id="a2881-127">在请求正文中，提供[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2881-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

<span data-ttu-id="a2881-128">下表显示创建[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2881-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).</span></span>

|<span data-ttu-id="a2881-129">属性</span><span class="sxs-lookup"><span data-stu-id="a2881-129">Property</span></span>|<span data-ttu-id="a2881-130">类型</span><span class="sxs-lookup"><span data-stu-id="a2881-130">Type</span></span>|<span data-ttu-id="a2881-131">说明</span><span class="sxs-lookup"><span data-stu-id="a2881-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2881-132">id</span><span class="sxs-lookup"><span data-stu-id="a2881-132">id</span></span>|<span data-ttu-id="a2881-133">String</span><span class="sxs-lookup"><span data-stu-id="a2881-133">String</span></span>|<span data-ttu-id="a2881-134">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a2881-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="a2881-135">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="a2881-135">startupDateTime</span></span>|<span data-ttu-id="a2881-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2881-136">DateTimeOffset</span></span>|<span data-ttu-id="a2881-137">User experience analytics 设备启动日期时间。</span><span class="sxs-lookup"><span data-stu-id="a2881-137">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="a2881-138">startupScore</span><span class="sxs-lookup"><span data-stu-id="a2881-138">startupScore</span></span>|<span data-ttu-id="a2881-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a2881-139">Int32</span></span>|<span data-ttu-id="a2881-140">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="a2881-140">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="a2881-141">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="a2881-141">coreBootScore</span></span>|<span data-ttu-id="a2881-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a2881-142">Int32</span></span>|<span data-ttu-id="a2881-143">用户体验分析设备核心启动分数。</span><span class="sxs-lookup"><span data-stu-id="a2881-143">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="a2881-144">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="a2881-144">coreSigninScore</span></span>|<span data-ttu-id="a2881-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a2881-145">Int32</span></span>|<span data-ttu-id="a2881-146">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="a2881-146">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="a2881-147">响应</span><span class="sxs-lookup"><span data-stu-id="a2881-147">Response</span></span>
<span data-ttu-id="a2881-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2881-148">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2881-149">示例</span><span class="sxs-lookup"><span data-stu-id="a2881-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2881-150">请求</span><span class="sxs-lookup"><span data-stu-id="a2881-150">Request</span></span>
<span data-ttu-id="a2881-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2881-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2881-152">响应</span><span class="sxs-lookup"><span data-stu-id="a2881-152">Response</span></span>
<span data-ttu-id="a2881-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2881-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





