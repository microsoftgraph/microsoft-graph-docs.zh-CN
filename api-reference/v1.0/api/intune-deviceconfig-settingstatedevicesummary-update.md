---
title: 更新 settingStateDeviceSummary
description: 更新 settingStateDeviceSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61810538addfc22f371077214e9960bda2014e9e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458288"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="26f66-103">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="26f66-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="26f66-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26f66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26f66-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26f66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26f66-106">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26f66-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26f66-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="26f66-107">Prerequisites</span></span>
<span data-ttu-id="26f66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26f66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f66-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26f66-110">Permission type</span></span>|<span data-ttu-id="26f66-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26f66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26f66-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26f66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26f66-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26f66-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26f66-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26f66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26f66-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26f66-115">Not supported.</span></span>|
|<span data-ttu-id="26f66-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="26f66-116">Application</span></span>|<span data-ttu-id="26f66-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="26f66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26f66-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26f66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="26f66-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26f66-119">Request headers</span></span>
|<span data-ttu-id="26f66-120">标头</span><span class="sxs-lookup"><span data-stu-id="26f66-120">Header</span></span>|<span data-ttu-id="26f66-121">值</span><span class="sxs-lookup"><span data-stu-id="26f66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26f66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26f66-122">Authorization</span></span>|<span data-ttu-id="26f66-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26f66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26f66-124">接受</span><span class="sxs-lookup"><span data-stu-id="26f66-124">Accept</span></span>|<span data-ttu-id="26f66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26f66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26f66-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26f66-126">Request body</span></span>
<span data-ttu-id="26f66-127">在请求正文中，提供 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26f66-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="26f66-128">下表显示了创建 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="26f66-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="26f66-129">属性</span><span class="sxs-lookup"><span data-stu-id="26f66-129">Property</span></span>|<span data-ttu-id="26f66-130">类型</span><span class="sxs-lookup"><span data-stu-id="26f66-130">Type</span></span>|<span data-ttu-id="26f66-131">说明</span><span class="sxs-lookup"><span data-stu-id="26f66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26f66-132">id</span><span class="sxs-lookup"><span data-stu-id="26f66-132">id</span></span>|<span data-ttu-id="26f66-133">String</span><span class="sxs-lookup"><span data-stu-id="26f66-133">String</span></span>|<span data-ttu-id="26f66-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="26f66-134">Key of the entity.</span></span>|
|<span data-ttu-id="26f66-135">settingName</span><span class="sxs-lookup"><span data-stu-id="26f66-135">settingName</span></span>|<span data-ttu-id="26f66-136">String</span><span class="sxs-lookup"><span data-stu-id="26f66-136">String</span></span>|<span data-ttu-id="26f66-137">设置的名称</span><span class="sxs-lookup"><span data-stu-id="26f66-137">Name of the setting</span></span>|
|<span data-ttu-id="26f66-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="26f66-138">instancePath</span></span>|<span data-ttu-id="26f66-139">String</span><span class="sxs-lookup"><span data-stu-id="26f66-139">String</span></span>|<span data-ttu-id="26f66-140">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="26f66-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="26f66-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f66-141">unknownDeviceCount</span></span>|<span data-ttu-id="26f66-142">Int32</span><span class="sxs-lookup"><span data-stu-id="26f66-142">Int32</span></span>|<span data-ttu-id="26f66-143">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="26f66-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="26f66-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f66-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="26f66-145">Int32</span><span class="sxs-lookup"><span data-stu-id="26f66-145">Int32</span></span>|<span data-ttu-id="26f66-146">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="26f66-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="26f66-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f66-147">compliantDeviceCount</span></span>|<span data-ttu-id="26f66-148">Int32</span><span class="sxs-lookup"><span data-stu-id="26f66-148">Int32</span></span>|<span data-ttu-id="26f66-149">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="26f66-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="26f66-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f66-150">remediatedDeviceCount</span></span>|<span data-ttu-id="26f66-151">Int32</span><span class="sxs-lookup"><span data-stu-id="26f66-151">Int32</span></span>|<span data-ttu-id="26f66-152">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="26f66-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="26f66-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f66-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="26f66-154">Int32</span><span class="sxs-lookup"><span data-stu-id="26f66-154">Int32</span></span>|<span data-ttu-id="26f66-155">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="26f66-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="26f66-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f66-156">errorDeviceCount</span></span>|<span data-ttu-id="26f66-157">Int32</span><span class="sxs-lookup"><span data-stu-id="26f66-157">Int32</span></span>|<span data-ttu-id="26f66-158">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="26f66-158">Device error count for the setting</span></span>|
|<span data-ttu-id="26f66-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f66-159">conflictDeviceCount</span></span>|<span data-ttu-id="26f66-160">Int32</span><span class="sxs-lookup"><span data-stu-id="26f66-160">Int32</span></span>|<span data-ttu-id="26f66-161">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="26f66-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="26f66-162">响应</span><span class="sxs-lookup"><span data-stu-id="26f66-162">Response</span></span>
<span data-ttu-id="26f66-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="26f66-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26f66-164">示例</span><span class="sxs-lookup"><span data-stu-id="26f66-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="26f66-165">请求</span><span class="sxs-lookup"><span data-stu-id="26f66-165">Request</span></span>
<span data-ttu-id="26f66-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26f66-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="26f66-167">响应</span><span class="sxs-lookup"><span data-stu-id="26f66-167">Response</span></span>
<span data-ttu-id="26f66-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26f66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```






