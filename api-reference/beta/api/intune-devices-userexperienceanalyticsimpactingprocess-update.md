---
title: 更新 userExperienceAnalyticsImpactingProcess
description: 更新 userExperienceAnalyticsImpactingProcess 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18be2d4556c454d387418a0ba434aa51bc0ea7e3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445957"
---
# <a name="update-userexperienceanalyticsimpactingprocess"></a><span data-ttu-id="4bc04-103">更新 userExperienceAnalyticsImpactingProcess</span><span class="sxs-lookup"><span data-stu-id="4bc04-103">Update userExperienceAnalyticsImpactingProcess</span></span>

<span data-ttu-id="4bc04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bc04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bc04-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bc04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bc04-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bc04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bc04-107">更新 [userExperienceAnalyticsImpactingProcess 对象](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4bc04-107">Update the properties of a [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bc04-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4bc04-108">Prerequisites</span></span>
<span data-ttu-id="4bc04-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bc04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bc04-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bc04-111">Permission type</span></span>|<span data-ttu-id="4bc04-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4bc04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bc04-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bc04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bc04-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bc04-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4bc04-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bc04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bc04-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bc04-116">Not supported.</span></span>|
|<span data-ttu-id="4bc04-117">Application</span><span class="sxs-lookup"><span data-stu-id="4bc04-117">Application</span></span>|<span data-ttu-id="4bc04-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bc04-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bc04-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bc04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="4bc04-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bc04-120">Request headers</span></span>
|<span data-ttu-id="4bc04-121">标头</span><span class="sxs-lookup"><span data-stu-id="4bc04-121">Header</span></span>|<span data-ttu-id="4bc04-122">值</span><span class="sxs-lookup"><span data-stu-id="4bc04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bc04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bc04-123">Authorization</span></span>|<span data-ttu-id="4bc04-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4bc04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bc04-125">接受</span><span class="sxs-lookup"><span data-stu-id="4bc04-125">Accept</span></span>|<span data-ttu-id="4bc04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bc04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bc04-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bc04-127">Request body</span></span>
<span data-ttu-id="4bc04-128">在请求正文中，提供 [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bc04-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

<span data-ttu-id="4bc04-129">下表显示创建 [userExperienceAnalyticsImpactingProcess 时所需的属性](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)。</span><span class="sxs-lookup"><span data-stu-id="4bc04-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).</span></span>

|<span data-ttu-id="4bc04-130">属性</span><span class="sxs-lookup"><span data-stu-id="4bc04-130">Property</span></span>|<span data-ttu-id="4bc04-131">类型</span><span class="sxs-lookup"><span data-stu-id="4bc04-131">Type</span></span>|<span data-ttu-id="4bc04-132">说明</span><span class="sxs-lookup"><span data-stu-id="4bc04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bc04-133">id</span><span class="sxs-lookup"><span data-stu-id="4bc04-133">id</span></span>|<span data-ttu-id="4bc04-134">String</span><span class="sxs-lookup"><span data-stu-id="4bc04-134">String</span></span>|<span data-ttu-id="4bc04-135">用户体验分析影响最重的进程实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4bc04-135">The unique identifier of the user experience analytics top impacting process entity.</span></span>|
|<span data-ttu-id="4bc04-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="4bc04-136">deviceId</span></span>|<span data-ttu-id="4bc04-137">String</span><span class="sxs-lookup"><span data-stu-id="4bc04-137">String</span></span>|<span data-ttu-id="4bc04-138">受影响设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4bc04-138">The unique identifier of the impacted device.</span></span>|
|<span data-ttu-id="4bc04-139">“类别”</span><span class="sxs-lookup"><span data-stu-id="4bc04-139">category</span></span>|<span data-ttu-id="4bc04-140">String</span><span class="sxs-lookup"><span data-stu-id="4bc04-140">String</span></span>|<span data-ttu-id="4bc04-141">影响过程的类别。</span><span class="sxs-lookup"><span data-stu-id="4bc04-141">The category of impacting process.</span></span>|
|<span data-ttu-id="4bc04-142">processName</span><span class="sxs-lookup"><span data-stu-id="4bc04-142">processName</span></span>|<span data-ttu-id="4bc04-143">String</span><span class="sxs-lookup"><span data-stu-id="4bc04-143">String</span></span>|<span data-ttu-id="4bc04-144">进程名称。</span><span class="sxs-lookup"><span data-stu-id="4bc04-144">The process name.</span></span>|
|<span data-ttu-id="4bc04-145">说明</span><span class="sxs-lookup"><span data-stu-id="4bc04-145">description</span></span>|<span data-ttu-id="4bc04-146">String</span><span class="sxs-lookup"><span data-stu-id="4bc04-146">String</span></span>|<span data-ttu-id="4bc04-147">过程说明。</span><span class="sxs-lookup"><span data-stu-id="4bc04-147">The description of process.</span></span>|
|<span data-ttu-id="4bc04-148">发布者</span><span class="sxs-lookup"><span data-stu-id="4bc04-148">publisher</span></span>|<span data-ttu-id="4bc04-149">String</span><span class="sxs-lookup"><span data-stu-id="4bc04-149">String</span></span>|<span data-ttu-id="4bc04-150">进程的发布者。</span><span class="sxs-lookup"><span data-stu-id="4bc04-150">The publisher of the process.</span></span>|
|<span data-ttu-id="4bc04-151">impactValue</span><span class="sxs-lookup"><span data-stu-id="4bc04-151">impactValue</span></span>|<span data-ttu-id="4bc04-152">双精度</span><span class="sxs-lookup"><span data-stu-id="4bc04-152">Double</span></span>|<span data-ttu-id="4bc04-153">进程的影响值。</span><span class="sxs-lookup"><span data-stu-id="4bc04-153">The impact value of the process.</span></span> <span data-ttu-id="4bc04-154">有效值 0 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="4bc04-154">Valid values 0 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="4bc04-155">响应</span><span class="sxs-lookup"><span data-stu-id="4bc04-155">Response</span></span>
<span data-ttu-id="4bc04-156">如果成功，此方法在响应正文中返回响应代码和更新的用户 `200 OK` [ExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4bc04-156">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc04-157">示例</span><span class="sxs-lookup"><span data-stu-id="4bc04-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bc04-158">请求</span><span class="sxs-lookup"><span data-stu-id="4bc04-158">Request</span></span>
<span data-ttu-id="4bc04-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bc04-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```

### <a name="response"></a><span data-ttu-id="4bc04-160">响应</span><span class="sxs-lookup"><span data-stu-id="4bc04-160">Response</span></span>
<span data-ttu-id="4bc04-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4bc04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "faefd665-d665-faef-65d6-effa65d6effa",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```




