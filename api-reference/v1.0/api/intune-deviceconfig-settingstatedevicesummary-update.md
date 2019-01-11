---
title: 更新 settingStateDeviceSummary
description: 更新 settingStateDeviceSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3927f039164c8b8e5be4092615cd213f505d7e76
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845834"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="144d4-103">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="144d4-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="144d4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="144d4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="144d4-105">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="144d4-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="144d4-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="144d4-106">Prerequisites</span></span>
<span data-ttu-id="144d4-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="144d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="144d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="144d4-109">Permission type</span></span>|<span data-ttu-id="144d4-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="144d4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="144d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="144d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="144d4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="144d4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="144d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="144d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="144d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="144d4-114">Not supported.</span></span>|
|<span data-ttu-id="144d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="144d4-115">Application</span></span>|<span data-ttu-id="144d4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="144d4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="144d4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="144d4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="144d4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="144d4-118">Request headers</span></span>
|<span data-ttu-id="144d4-119">标头</span><span class="sxs-lookup"><span data-stu-id="144d4-119">Header</span></span>|<span data-ttu-id="144d4-120">值</span><span class="sxs-lookup"><span data-stu-id="144d4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="144d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="144d4-121">Authorization</span></span>|<span data-ttu-id="144d4-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="144d4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="144d4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="144d4-123">Accept</span></span>|<span data-ttu-id="144d4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="144d4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="144d4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="144d4-125">Request body</span></span>
<span data-ttu-id="144d4-126">在请求正文中，提供 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="144d4-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="144d4-127">下表显示了创建 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="144d4-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="144d4-128">属性</span><span class="sxs-lookup"><span data-stu-id="144d4-128">Property</span></span>|<span data-ttu-id="144d4-129">类型</span><span class="sxs-lookup"><span data-stu-id="144d4-129">Type</span></span>|<span data-ttu-id="144d4-130">说明</span><span class="sxs-lookup"><span data-stu-id="144d4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="144d4-131">id</span><span class="sxs-lookup"><span data-stu-id="144d4-131">id</span></span>|<span data-ttu-id="144d4-132">String</span><span class="sxs-lookup"><span data-stu-id="144d4-132">String</span></span>|<span data-ttu-id="144d4-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="144d4-133">Key of the entity.</span></span>|
|<span data-ttu-id="144d4-134">settingName</span><span class="sxs-lookup"><span data-stu-id="144d4-134">settingName</span></span>|<span data-ttu-id="144d4-135">String</span><span class="sxs-lookup"><span data-stu-id="144d4-135">String</span></span>|<span data-ttu-id="144d4-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="144d4-136">Name of the setting</span></span>|
|<span data-ttu-id="144d4-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="144d4-137">instancePath</span></span>|<span data-ttu-id="144d4-138">String</span><span class="sxs-lookup"><span data-stu-id="144d4-138">String</span></span>|<span data-ttu-id="144d4-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="144d4-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="144d4-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="144d4-140">unknownDeviceCount</span></span>|<span data-ttu-id="144d4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="144d4-141">Int32</span></span>|<span data-ttu-id="144d4-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="144d4-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="144d4-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="144d4-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="144d4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="144d4-144">Int32</span></span>|<span data-ttu-id="144d4-145">设置的设备不适用计数</span><span class="sxs-lookup"><span data-stu-id="144d4-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="144d4-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="144d4-146">compliantDeviceCount</span></span>|<span data-ttu-id="144d4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="144d4-147">Int32</span></span>|<span data-ttu-id="144d4-148">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="144d4-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="144d4-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="144d4-149">remediatedDeviceCount</span></span>|<span data-ttu-id="144d4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="144d4-150">Int32</span></span>|<span data-ttu-id="144d4-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="144d4-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="144d4-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="144d4-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="144d4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="144d4-153">Int32</span></span>|<span data-ttu-id="144d4-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="144d4-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="144d4-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="144d4-155">errorDeviceCount</span></span>|<span data-ttu-id="144d4-156">Int32</span><span class="sxs-lookup"><span data-stu-id="144d4-156">Int32</span></span>|<span data-ttu-id="144d4-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="144d4-157">Device error count for the setting</span></span>|
|<span data-ttu-id="144d4-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="144d4-158">conflictDeviceCount</span></span>|<span data-ttu-id="144d4-159">Int32</span><span class="sxs-lookup"><span data-stu-id="144d4-159">Int32</span></span>|<span data-ttu-id="144d4-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="144d4-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="144d4-161">响应</span><span class="sxs-lookup"><span data-stu-id="144d4-161">Response</span></span>
<span data-ttu-id="144d4-162">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="144d4-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="144d4-163">示例</span><span class="sxs-lookup"><span data-stu-id="144d4-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="144d4-164">请求</span><span class="sxs-lookup"><span data-stu-id="144d4-164">Request</span></span>
<span data-ttu-id="144d4-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="144d4-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="144d4-166">响应</span><span class="sxs-lookup"><span data-stu-id="144d4-166">Response</span></span>
<span data-ttu-id="144d4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="144d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



