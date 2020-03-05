---
title: 创建 userExperienceAnalyticsStartupScoreHistory
description: 创建新的 userExperienceAnalyticsStartupScoreHistory 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd2dfad7eecfd373c6fa92c8b1023200b08a61d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468045"
---
# <a name="create-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="20233-103">创建 userExperienceAnalyticsStartupScoreHistory</span><span class="sxs-lookup"><span data-stu-id="20233-103">Create userExperienceAnalyticsStartupScoreHistory</span></span>

<span data-ttu-id="20233-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="20233-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20233-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="20233-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20233-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20233-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20233-107">创建新的[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20233-107">Create a new [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20233-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="20233-108">Prerequisites</span></span>
<span data-ttu-id="20233-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20233-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="20233-111">Permission type</span></span>|<span data-ttu-id="20233-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="20233-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20233-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20233-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20233-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20233-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="20233-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20233-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20233-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20233-116">Not supported.</span></span>|
|<span data-ttu-id="20233-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="20233-117">Application</span></span>|<span data-ttu-id="20233-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20233-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20233-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20233-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="20233-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="20233-120">Request headers</span></span>
|<span data-ttu-id="20233-121">标头</span><span class="sxs-lookup"><span data-stu-id="20233-121">Header</span></span>|<span data-ttu-id="20233-122">值</span><span class="sxs-lookup"><span data-stu-id="20233-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20233-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20233-123">Authorization</span></span>|<span data-ttu-id="20233-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20233-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20233-125">接受</span><span class="sxs-lookup"><span data-stu-id="20233-125">Accept</span></span>|<span data-ttu-id="20233-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20233-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20233-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="20233-127">Request body</span></span>
<span data-ttu-id="20233-128">在请求正文中，提供 userExperienceAnalyticsStartupScoreHistory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20233-128">In the request body, supply a JSON representation for the userExperienceAnalyticsStartupScoreHistory object.</span></span>

<span data-ttu-id="20233-129">下表显示创建 userExperienceAnalyticsStartupScoreHistory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20233-129">The following table shows the properties that are required when you create the userExperienceAnalyticsStartupScoreHistory.</span></span>

|<span data-ttu-id="20233-130">属性</span><span class="sxs-lookup"><span data-stu-id="20233-130">Property</span></span>|<span data-ttu-id="20233-131">类型</span><span class="sxs-lookup"><span data-stu-id="20233-131">Type</span></span>|<span data-ttu-id="20233-132">说明</span><span class="sxs-lookup"><span data-stu-id="20233-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20233-133">id</span><span class="sxs-lookup"><span data-stu-id="20233-133">id</span></span>|<span data-ttu-id="20233-134">String</span><span class="sxs-lookup"><span data-stu-id="20233-134">String</span></span>|<span data-ttu-id="20233-135">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="20233-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="20233-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="20233-136">startupDateTime</span></span>|<span data-ttu-id="20233-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20233-137">DateTimeOffset</span></span>|<span data-ttu-id="20233-138">User experience analytics 设备启动日期时间。</span><span class="sxs-lookup"><span data-stu-id="20233-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="20233-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="20233-139">startupScore</span></span>|<span data-ttu-id="20233-140">Int32</span><span class="sxs-lookup"><span data-stu-id="20233-140">Int32</span></span>|<span data-ttu-id="20233-141">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="20233-141">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="20233-142">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="20233-142">coreBootScore</span></span>|<span data-ttu-id="20233-143">Int32</span><span class="sxs-lookup"><span data-stu-id="20233-143">Int32</span></span>|<span data-ttu-id="20233-144">用户体验分析设备核心启动分数。</span><span class="sxs-lookup"><span data-stu-id="20233-144">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="20233-145">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="20233-145">coreSigninScore</span></span>|<span data-ttu-id="20233-146">Int32</span><span class="sxs-lookup"><span data-stu-id="20233-146">Int32</span></span>|<span data-ttu-id="20233-147">用户体验分析设备核心登录分数。</span><span class="sxs-lookup"><span data-stu-id="20233-147">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="20233-148">响应</span><span class="sxs-lookup"><span data-stu-id="20233-148">Response</span></span>
<span data-ttu-id="20233-149">如果成功，此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20233-149">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20233-150">示例</span><span class="sxs-lookup"><span data-stu-id="20233-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="20233-151">请求</span><span class="sxs-lookup"><span data-stu-id="20233-151">Request</span></span>
<span data-ttu-id="20233-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20233-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory
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

### <a name="response"></a><span data-ttu-id="20233-153">响应</span><span class="sxs-lookup"><span data-stu-id="20233-153">Response</span></span>
<span data-ttu-id="20233-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20233-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





