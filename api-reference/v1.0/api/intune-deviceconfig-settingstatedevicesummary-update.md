---
title: 更新 settingStateDeviceSummary
description: 更新 settingStateDeviceSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2419f6e743448c91ea3927d1bc9f7ca71ebc686d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258679"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="fe854-103">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="fe854-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="fe854-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe854-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe854-105">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fe854-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe854-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe854-106">Prerequisites</span></span>
<span data-ttu-id="fe854-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fe854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe854-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe854-109">Permission type</span></span>|<span data-ttu-id="fe854-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe854-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe854-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe854-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe854-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe854-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe854-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe854-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe854-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe854-114">Not supported.</span></span>|
|<span data-ttu-id="fe854-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe854-115">Application</span></span>|<span data-ttu-id="fe854-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe854-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe854-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe854-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="fe854-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe854-118">Request headers</span></span>
|<span data-ttu-id="fe854-119">标头</span><span class="sxs-lookup"><span data-stu-id="fe854-119">Header</span></span>|<span data-ttu-id="fe854-120">值</span><span class="sxs-lookup"><span data-stu-id="fe854-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe854-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe854-121">Authorization</span></span>|<span data-ttu-id="fe854-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe854-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe854-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fe854-123">Accept</span></span>|<span data-ttu-id="fe854-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fe854-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe854-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe854-125">Request body</span></span>
<span data-ttu-id="fe854-126">在请求正文中，提供 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe854-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="fe854-127">下表显示了创建 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe854-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="fe854-128">属性</span><span class="sxs-lookup"><span data-stu-id="fe854-128">Property</span></span>|<span data-ttu-id="fe854-129">类型</span><span class="sxs-lookup"><span data-stu-id="fe854-129">Type</span></span>|<span data-ttu-id="fe854-130">说明</span><span class="sxs-lookup"><span data-stu-id="fe854-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe854-131">id</span><span class="sxs-lookup"><span data-stu-id="fe854-131">id</span></span>|<span data-ttu-id="fe854-132">字符串</span><span class="sxs-lookup"><span data-stu-id="fe854-132">String</span></span>|<span data-ttu-id="fe854-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fe854-133">Key of the entity.</span></span>|
|<span data-ttu-id="fe854-134">settingName</span><span class="sxs-lookup"><span data-stu-id="fe854-134">settingName</span></span>|<span data-ttu-id="fe854-135">String</span><span class="sxs-lookup"><span data-stu-id="fe854-135">String</span></span>|<span data-ttu-id="fe854-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="fe854-136">Name of the setting</span></span>|
|<span data-ttu-id="fe854-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="fe854-137">instancePath</span></span>|<span data-ttu-id="fe854-138">String</span><span class="sxs-lookup"><span data-stu-id="fe854-138">String</span></span>|<span data-ttu-id="fe854-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="fe854-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="fe854-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fe854-140">unknownDeviceCount</span></span>|<span data-ttu-id="fe854-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fe854-141">Int32</span></span>|<span data-ttu-id="fe854-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="fe854-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="fe854-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fe854-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="fe854-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fe854-144">Int32</span></span>|<span data-ttu-id="fe854-145">设置的设备不适用计数</span><span class="sxs-lookup"><span data-stu-id="fe854-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="fe854-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fe854-146">compliantDeviceCount</span></span>|<span data-ttu-id="fe854-147">Int32</span><span class="sxs-lookup"><span data-stu-id="fe854-147">Int32</span></span>|<span data-ttu-id="fe854-148">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="fe854-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="fe854-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fe854-149">remediatedDeviceCount</span></span>|<span data-ttu-id="fe854-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fe854-150">Int32</span></span>|<span data-ttu-id="fe854-151">设置的设备合规计数</span><span class="sxs-lookup"><span data-stu-id="fe854-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="fe854-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fe854-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="fe854-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fe854-153">Int32</span></span>|<span data-ttu-id="fe854-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="fe854-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="fe854-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fe854-155">errorDeviceCount</span></span>|<span data-ttu-id="fe854-156">Int32</span><span class="sxs-lookup"><span data-stu-id="fe854-156">Int32</span></span>|<span data-ttu-id="fe854-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="fe854-157">Device error count for the setting</span></span>|
|<span data-ttu-id="fe854-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fe854-158">conflictDeviceCount</span></span>|<span data-ttu-id="fe854-159">Int32</span><span class="sxs-lookup"><span data-stu-id="fe854-159">Int32</span></span>|<span data-ttu-id="fe854-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="fe854-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="fe854-161">响应</span><span class="sxs-lookup"><span data-stu-id="fe854-161">Response</span></span>
<span data-ttu-id="fe854-162">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe854-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe854-163">示例</span><span class="sxs-lookup"><span data-stu-id="fe854-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe854-164">请求</span><span class="sxs-lookup"><span data-stu-id="fe854-164">Request</span></span>
<span data-ttu-id="fe854-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe854-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe854-166">响应</span><span class="sxs-lookup"><span data-stu-id="fe854-166">Response</span></span>
<span data-ttu-id="fe854-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe854-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



