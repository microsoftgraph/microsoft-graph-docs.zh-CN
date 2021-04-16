---
title: 更新 userExperienceAnalyticsWorkFromAnywhereDevice
description: 更新 userExperienceAnalyticsWorkFromAnywhereDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec8a6c16550eb28770af9ce895f3941f3461b00a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868484"
---
# <a name="update-userexperienceanalyticsworkfromanywheredevice"></a><span data-ttu-id="e0394-103">更新 userExperienceAnalyticsWorkFromAnywhereDevice</span><span class="sxs-lookup"><span data-stu-id="e0394-103">Update userExperienceAnalyticsWorkFromAnywhereDevice</span></span>

<span data-ttu-id="e0394-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0394-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0394-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0394-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0394-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0394-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0394-107">更新 [userExperienceAnalyticsWorkFromAnywhereDevice 对象](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e0394-107">Update the properties of a [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0394-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0394-108">Prerequisites</span></span>
<span data-ttu-id="e0394-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0394-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0394-111">Permission type</span></span>|<span data-ttu-id="e0394-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0394-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0394-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0394-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0394-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0394-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e0394-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0394-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0394-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0394-116">Not supported.</span></span>|
|<span data-ttu-id="e0394-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0394-117">Application</span></span>|<span data-ttu-id="e0394-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0394-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0394-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0394-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="e0394-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0394-120">Request headers</span></span>
|<span data-ttu-id="e0394-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0394-121">Header</span></span>|<span data-ttu-id="e0394-122">值</span><span class="sxs-lookup"><span data-stu-id="e0394-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0394-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0394-123">Authorization</span></span>|<span data-ttu-id="e0394-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0394-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0394-125">接受</span><span class="sxs-lookup"><span data-stu-id="e0394-125">Accept</span></span>|<span data-ttu-id="e0394-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0394-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0394-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0394-127">Request body</span></span>
<span data-ttu-id="e0394-128">在请求正文中，提供 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0394-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

<span data-ttu-id="e0394-129">下表显示创建 [userExperienceAnalyticsWorkFromAnywhereDevice 时所需的属性](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)。</span><span class="sxs-lookup"><span data-stu-id="e0394-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md).</span></span>

|<span data-ttu-id="e0394-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0394-130">Property</span></span>|<span data-ttu-id="e0394-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0394-131">Type</span></span>|<span data-ttu-id="e0394-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0394-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0394-133">id</span><span class="sxs-lookup"><span data-stu-id="e0394-133">id</span></span>|<span data-ttu-id="e0394-134">String</span><span class="sxs-lookup"><span data-stu-id="e0394-134">String</span></span>|<span data-ttu-id="e0394-135">用户体验分析的唯一标识符从任何设备工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-135">The unique identifier of the user experience analytics work from anywhere device.</span></span>|
|<span data-ttu-id="e0394-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="e0394-136">deviceName</span></span>|<span data-ttu-id="e0394-137">String</span><span class="sxs-lookup"><span data-stu-id="e0394-137">String</span></span>|<span data-ttu-id="e0394-138">来自任何设备名称的工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-138">The work from anywhere device's name.</span></span>|
|<span data-ttu-id="e0394-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e0394-139">serialNumber</span></span>|<span data-ttu-id="e0394-140">String</span><span class="sxs-lookup"><span data-stu-id="e0394-140">String</span></span>|<span data-ttu-id="e0394-141">用户体验随设备序列号随处工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-141">The user experience work from anywhere device's serial number.</span></span>|
|<span data-ttu-id="e0394-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="e0394-142">manufacturer</span></span>|<span data-ttu-id="e0394-143">String</span><span class="sxs-lookup"><span data-stu-id="e0394-143">String</span></span>|<span data-ttu-id="e0394-144">用户体验从任何设备制造商处工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-144">The user experience work from anywhere device's manufacturer.</span></span>|
|<span data-ttu-id="e0394-145">model</span><span class="sxs-lookup"><span data-stu-id="e0394-145">model</span></span>|<span data-ttu-id="e0394-146">String</span><span class="sxs-lookup"><span data-stu-id="e0394-146">String</span></span>|<span data-ttu-id="e0394-147">用户体验从任何设备型号开始工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-147">The user experience work from anywhere device's model.</span></span>|
|<span data-ttu-id="e0394-148">ownership</span><span class="sxs-lookup"><span data-stu-id="e0394-148">ownership</span></span>|<span data-ttu-id="e0394-149">String</span><span class="sxs-lookup"><span data-stu-id="e0394-149">String</span></span>|<span data-ttu-id="e0394-150">用户体验从任何设备所有权开始工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-150">The user experience work from anywhere device's ownership.</span></span>|
|<span data-ttu-id="e0394-151">managedBy</span><span class="sxs-lookup"><span data-stu-id="e0394-151">managedBy</span></span>|<span data-ttu-id="e0394-152">String</span><span class="sxs-lookup"><span data-stu-id="e0394-152">String</span></span>|<span data-ttu-id="e0394-153">用户体验从设备的任何管理代理工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-153">The user experience work from anywhere management agent of the device.</span></span>|
|<span data-ttu-id="e0394-154">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="e0394-154">autoPilotRegistered</span></span>|<span data-ttu-id="e0394-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0394-155">Boolean</span></span>|<span data-ttu-id="e0394-156">用户体验从 intune 设备的 autopilotRegistered 的任何位置工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-156">The user experience work from anywhere intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="e0394-157">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="e0394-157">autoPilotProfileAssigned</span></span>|<span data-ttu-id="e0394-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0394-158">Boolean</span></span>|<span data-ttu-id="e0394-159">用户体验分析从 intune 设备的 autopilotProfileAssigned 的任何位置工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-159">The user experience analytics work from anywhere intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="e0394-160">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="e0394-160">azureAdRegistered</span></span>|<span data-ttu-id="e0394-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0394-161">Boolean</span></span>|<span data-ttu-id="e0394-162">用户体验从任何设备的 azureAdRegistered 工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-162">The user experience work from anywhere device's azureAdRegistered.</span></span>|
|<span data-ttu-id="e0394-163">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="e0394-163">azureAdDeviceId</span></span>|<span data-ttu-id="e0394-164">String</span><span class="sxs-lookup"><span data-stu-id="e0394-164">String</span></span>|<span data-ttu-id="e0394-165">用户体验从 Azure Ad 设备 ID 的任何位置工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-165">The user experience work from anywhere azure Ad device Id.</span></span>|
|<span data-ttu-id="e0394-166">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="e0394-166">azureAdJoinType</span></span>|<span data-ttu-id="e0394-167">String</span><span class="sxs-lookup"><span data-stu-id="e0394-167">String</span></span>|<span data-ttu-id="e0394-168">用户体验从任何设备的 azure Ad joinType 工作。</span><span class="sxs-lookup"><span data-stu-id="e0394-168">The user experience work from anywhere device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="e0394-169">响应</span><span class="sxs-lookup"><span data-stu-id="e0394-169">Response</span></span>
<span data-ttu-id="e0394-170">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0394-170">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0394-171">示例</span><span class="sxs-lookup"><span data-stu-id="e0394-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0394-172">请求</span><span class="sxs-lookup"><span data-stu-id="e0394-172">Request</span></span>
<span data-ttu-id="e0394-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0394-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="e0394-174">响应</span><span class="sxs-lookup"><span data-stu-id="e0394-174">Response</span></span>
<span data-ttu-id="e0394-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0394-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 554

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




