---
title: 更新 settingStateDeviceSummary
description: 更新 settingStateDeviceSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81331f767403b40ebe07ad0676a568f82a844384
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089159"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="55fe7-103">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="55fe7-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="55fe7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55fe7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55fe7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55fe7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55fe7-106">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="55fe7-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55fe7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="55fe7-107">Prerequisites</span></span>
<span data-ttu-id="55fe7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55fe7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="55fe7-110">Permission type</span></span>|<span data-ttu-id="55fe7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="55fe7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55fe7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55fe7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55fe7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55fe7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55fe7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55fe7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55fe7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="55fe7-115">Not supported.</span></span>|
|<span data-ttu-id="55fe7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="55fe7-116">Application</span></span>|<span data-ttu-id="55fe7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="55fe7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55fe7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55fe7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="55fe7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="55fe7-119">Request headers</span></span>
|<span data-ttu-id="55fe7-120">标头</span><span class="sxs-lookup"><span data-stu-id="55fe7-120">Header</span></span>|<span data-ttu-id="55fe7-121">值</span><span class="sxs-lookup"><span data-stu-id="55fe7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55fe7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55fe7-122">Authorization</span></span>|<span data-ttu-id="55fe7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55fe7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55fe7-124">接受</span><span class="sxs-lookup"><span data-stu-id="55fe7-124">Accept</span></span>|<span data-ttu-id="55fe7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55fe7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55fe7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="55fe7-126">Request body</span></span>
<span data-ttu-id="55fe7-127">在请求正文中，提供 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55fe7-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="55fe7-128">下表显示了创建 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="55fe7-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="55fe7-129">属性</span><span class="sxs-lookup"><span data-stu-id="55fe7-129">Property</span></span>|<span data-ttu-id="55fe7-130">类型</span><span class="sxs-lookup"><span data-stu-id="55fe7-130">Type</span></span>|<span data-ttu-id="55fe7-131">说明</span><span class="sxs-lookup"><span data-stu-id="55fe7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55fe7-132">id</span><span class="sxs-lookup"><span data-stu-id="55fe7-132">id</span></span>|<span data-ttu-id="55fe7-133">String</span><span class="sxs-lookup"><span data-stu-id="55fe7-133">String</span></span>|<span data-ttu-id="55fe7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="55fe7-134">Key of the entity.</span></span>|
|<span data-ttu-id="55fe7-135">settingName</span><span class="sxs-lookup"><span data-stu-id="55fe7-135">settingName</span></span>|<span data-ttu-id="55fe7-136">String</span><span class="sxs-lookup"><span data-stu-id="55fe7-136">String</span></span>|<span data-ttu-id="55fe7-137">设置的名称</span><span class="sxs-lookup"><span data-stu-id="55fe7-137">Name of the setting</span></span>|
|<span data-ttu-id="55fe7-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="55fe7-138">instancePath</span></span>|<span data-ttu-id="55fe7-139">String</span><span class="sxs-lookup"><span data-stu-id="55fe7-139">String</span></span>|<span data-ttu-id="55fe7-140">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="55fe7-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="55fe7-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55fe7-141">unknownDeviceCount</span></span>|<span data-ttu-id="55fe7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="55fe7-142">Int32</span></span>|<span data-ttu-id="55fe7-143">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="55fe7-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="55fe7-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55fe7-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="55fe7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="55fe7-145">Int32</span></span>|<span data-ttu-id="55fe7-146">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="55fe7-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="55fe7-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55fe7-147">compliantDeviceCount</span></span>|<span data-ttu-id="55fe7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="55fe7-148">Int32</span></span>|<span data-ttu-id="55fe7-149">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="55fe7-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="55fe7-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55fe7-150">remediatedDeviceCount</span></span>|<span data-ttu-id="55fe7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="55fe7-151">Int32</span></span>|<span data-ttu-id="55fe7-152">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="55fe7-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="55fe7-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55fe7-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="55fe7-154">Int32</span><span class="sxs-lookup"><span data-stu-id="55fe7-154">Int32</span></span>|<span data-ttu-id="55fe7-155">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="55fe7-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="55fe7-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55fe7-156">errorDeviceCount</span></span>|<span data-ttu-id="55fe7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="55fe7-157">Int32</span></span>|<span data-ttu-id="55fe7-158">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="55fe7-158">Device error count for the setting</span></span>|
|<span data-ttu-id="55fe7-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55fe7-159">conflictDeviceCount</span></span>|<span data-ttu-id="55fe7-160">Int32</span><span class="sxs-lookup"><span data-stu-id="55fe7-160">Int32</span></span>|<span data-ttu-id="55fe7-161">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="55fe7-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="55fe7-162">响应</span><span class="sxs-lookup"><span data-stu-id="55fe7-162">Response</span></span>
<span data-ttu-id="55fe7-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55fe7-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55fe7-164">示例</span><span class="sxs-lookup"><span data-stu-id="55fe7-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="55fe7-165">请求</span><span class="sxs-lookup"><span data-stu-id="55fe7-165">Request</span></span>
<span data-ttu-id="55fe7-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55fe7-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55fe7-167">响应</span><span class="sxs-lookup"><span data-stu-id="55fe7-167">Response</span></span>
<span data-ttu-id="55fe7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55fe7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









