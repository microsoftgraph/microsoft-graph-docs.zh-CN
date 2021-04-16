---
title: 创建 userExperienceAnalyticsWorkFromAnywhereDevice
description: 创建新的 userExperienceAnalyticsWorkFromAnywhereDevice 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cd4db22f691935d53b85eded268650ab0bc12b4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868467"
---
# <a name="create-userexperienceanalyticsworkfromanywheredevice"></a><span data-ttu-id="9f9f7-103">创建 userExperienceAnalyticsWorkFromAnywhereDevice</span><span class="sxs-lookup"><span data-stu-id="9f9f7-103">Create userExperienceAnalyticsWorkFromAnywhereDevice</span></span>

<span data-ttu-id="9f9f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f9f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f9f7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f9f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f9f7-107">创建新的 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-107">Create a new [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f9f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f9f7-108">Prerequisites</span></span>
<span data-ttu-id="9f9f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f9f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f9f7-111">Permission type</span></span>|<span data-ttu-id="9f9f7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f9f7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f9f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f9f7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f9f7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9f9f7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f9f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f9f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-116">Not supported.</span></span>|
|<span data-ttu-id="9f9f7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f9f7-117">Application</span></span>|<span data-ttu-id="9f9f7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f9f7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f9f7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f9f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a><span data-ttu-id="9f9f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f9f7-120">Request headers</span></span>
|<span data-ttu-id="9f9f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="9f9f7-121">Header</span></span>|<span data-ttu-id="9f9f7-122">值</span><span class="sxs-lookup"><span data-stu-id="9f9f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f9f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f9f7-123">Authorization</span></span>|<span data-ttu-id="9f9f7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f9f7-125">接受</span><span class="sxs-lookup"><span data-stu-id="9f9f7-125">Accept</span></span>|<span data-ttu-id="9f9f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f9f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f9f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f9f7-127">Request body</span></span>
<span data-ttu-id="9f9f7-128">在请求正文中，提供 userExperienceAnalyticsWorkFromAnywhereDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-128">In the request body, supply a JSON representation for the userExperienceAnalyticsWorkFromAnywhereDevice object.</span></span>

<span data-ttu-id="9f9f7-129">下表显示创建 userExperienceAnalyticsWorkFromAnywhereDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-129">The following table shows the properties that are required when you create the userExperienceAnalyticsWorkFromAnywhereDevice.</span></span>

|<span data-ttu-id="9f9f7-130">属性</span><span class="sxs-lookup"><span data-stu-id="9f9f7-130">Property</span></span>|<span data-ttu-id="9f9f7-131">类型</span><span class="sxs-lookup"><span data-stu-id="9f9f7-131">Type</span></span>|<span data-ttu-id="9f9f7-132">说明</span><span class="sxs-lookup"><span data-stu-id="9f9f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f9f7-133">id</span><span class="sxs-lookup"><span data-stu-id="9f9f7-133">id</span></span>|<span data-ttu-id="9f9f7-134">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-134">String</span></span>|<span data-ttu-id="9f9f7-135">用户体验分析的唯一标识符从任何设备工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-135">The unique identifier of the user experience analytics work from anywhere device.</span></span>|
|<span data-ttu-id="9f9f7-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="9f9f7-136">deviceName</span></span>|<span data-ttu-id="9f9f7-137">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-137">String</span></span>|<span data-ttu-id="9f9f7-138">来自任何设备名称的工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-138">The work from anywhere device's name.</span></span>|
|<span data-ttu-id="9f9f7-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9f9f7-139">serialNumber</span></span>|<span data-ttu-id="9f9f7-140">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-140">String</span></span>|<span data-ttu-id="9f9f7-141">用户体验随设备序列号随处工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-141">The user experience work from anywhere device's serial number.</span></span>|
|<span data-ttu-id="9f9f7-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9f9f7-142">manufacturer</span></span>|<span data-ttu-id="9f9f7-143">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-143">String</span></span>|<span data-ttu-id="9f9f7-144">用户体验从任何设备制造商处工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-144">The user experience work from anywhere device's manufacturer.</span></span>|
|<span data-ttu-id="9f9f7-145">model</span><span class="sxs-lookup"><span data-stu-id="9f9f7-145">model</span></span>|<span data-ttu-id="9f9f7-146">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-146">String</span></span>|<span data-ttu-id="9f9f7-147">用户体验从任何设备型号开始工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-147">The user experience work from anywhere device's model.</span></span>|
|<span data-ttu-id="9f9f7-148">ownership</span><span class="sxs-lookup"><span data-stu-id="9f9f7-148">ownership</span></span>|<span data-ttu-id="9f9f7-149">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-149">String</span></span>|<span data-ttu-id="9f9f7-150">用户体验从任何设备所有权开始工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-150">The user experience work from anywhere device's ownership.</span></span>|
|<span data-ttu-id="9f9f7-151">managedBy</span><span class="sxs-lookup"><span data-stu-id="9f9f7-151">managedBy</span></span>|<span data-ttu-id="9f9f7-152">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-152">String</span></span>|<span data-ttu-id="9f9f7-153">用户体验从设备的任何管理代理工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-153">The user experience work from anywhere management agent of the device.</span></span>|
|<span data-ttu-id="9f9f7-154">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="9f9f7-154">autoPilotRegistered</span></span>|<span data-ttu-id="9f9f7-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f9f7-155">Boolean</span></span>|<span data-ttu-id="9f9f7-156">用户体验从 intune 设备的 autopilotRegistered 的任何位置工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-156">The user experience work from anywhere intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="9f9f7-157">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="9f9f7-157">autoPilotProfileAssigned</span></span>|<span data-ttu-id="9f9f7-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f9f7-158">Boolean</span></span>|<span data-ttu-id="9f9f7-159">用户体验分析从 intune 设备的 autopilotProfileAssigned 的任何位置工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-159">The user experience analytics work from anywhere intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="9f9f7-160">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="9f9f7-160">azureAdRegistered</span></span>|<span data-ttu-id="9f9f7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f9f7-161">Boolean</span></span>|<span data-ttu-id="9f9f7-162">用户体验从任何设备的 azureAdRegistered 工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-162">The user experience work from anywhere device's azureAdRegistered.</span></span>|
|<span data-ttu-id="9f9f7-163">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="9f9f7-163">azureAdDeviceId</span></span>|<span data-ttu-id="9f9f7-164">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-164">String</span></span>|<span data-ttu-id="9f9f7-165">用户体验从 Azure Ad 设备 ID 的任何位置工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-165">The user experience work from anywhere azure Ad device Id.</span></span>|
|<span data-ttu-id="9f9f7-166">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="9f9f7-166">azureAdJoinType</span></span>|<span data-ttu-id="9f9f7-167">String</span><span class="sxs-lookup"><span data-stu-id="9f9f7-167">String</span></span>|<span data-ttu-id="9f9f7-168">用户体验从任何设备的 azure Ad joinType 工作。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-168">The user experience work from anywhere device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="9f9f7-169">响应</span><span class="sxs-lookup"><span data-stu-id="9f9f7-169">Response</span></span>
<span data-ttu-id="9f9f7-170">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-170">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f9f7-171">示例</span><span class="sxs-lookup"><span data-stu-id="9f9f7-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f9f7-172">请求</span><span class="sxs-lookup"><span data-stu-id="9f9f7-172">Request</span></span>
<span data-ttu-id="9f9f7-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
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

### <a name="response"></a><span data-ttu-id="9f9f7-174">响应</span><span class="sxs-lookup"><span data-stu-id="9f9f7-174">Response</span></span>
<span data-ttu-id="9f9f7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f9f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




