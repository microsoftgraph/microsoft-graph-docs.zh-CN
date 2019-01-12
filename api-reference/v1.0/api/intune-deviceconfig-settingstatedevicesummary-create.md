---
title: 创建 settingStateDeviceSummary
description: 创建新的 settingStateDeviceSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 512d36e348a675534c3c1306045fd8570dc22ef5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912265"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="53b6b-103">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="53b6b-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="53b6b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="53b6b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53b6b-105">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53b6b-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53b6b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="53b6b-106">Prerequisites</span></span>
<span data-ttu-id="53b6b-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="53b6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b6b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53b6b-109">Permission type</span></span>|<span data-ttu-id="53b6b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53b6b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b6b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53b6b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53b6b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b6b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53b6b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53b6b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b6b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53b6b-114">Not supported.</span></span>|
|<span data-ttu-id="53b6b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53b6b-115">Application</span></span>|<span data-ttu-id="53b6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53b6b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b6b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53b6b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="53b6b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="53b6b-118">Request headers</span></span>
|<span data-ttu-id="53b6b-119">标头</span><span class="sxs-lookup"><span data-stu-id="53b6b-119">Header</span></span>|<span data-ttu-id="53b6b-120">值</span><span class="sxs-lookup"><span data-stu-id="53b6b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53b6b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53b6b-121">Authorization</span></span>|<span data-ttu-id="53b6b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53b6b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53b6b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="53b6b-123">Accept</span></span>|<span data-ttu-id="53b6b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53b6b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b6b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53b6b-125">Request body</span></span>
<span data-ttu-id="53b6b-126">在请求正文中，提供 settingStateDeviceSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53b6b-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="53b6b-127">下表显示了创建 settingStateDeviceSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53b6b-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="53b6b-128">属性</span><span class="sxs-lookup"><span data-stu-id="53b6b-128">Property</span></span>|<span data-ttu-id="53b6b-129">类型</span><span class="sxs-lookup"><span data-stu-id="53b6b-129">Type</span></span>|<span data-ttu-id="53b6b-130">说明</span><span class="sxs-lookup"><span data-stu-id="53b6b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b6b-131">id</span><span class="sxs-lookup"><span data-stu-id="53b6b-131">id</span></span>|<span data-ttu-id="53b6b-132">String</span><span class="sxs-lookup"><span data-stu-id="53b6b-132">String</span></span>|<span data-ttu-id="53b6b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="53b6b-133">Key of the entity.</span></span>|
|<span data-ttu-id="53b6b-134">settingName</span><span class="sxs-lookup"><span data-stu-id="53b6b-134">settingName</span></span>|<span data-ttu-id="53b6b-135">String</span><span class="sxs-lookup"><span data-stu-id="53b6b-135">String</span></span>|<span data-ttu-id="53b6b-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="53b6b-136">Name of the setting</span></span>|
|<span data-ttu-id="53b6b-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="53b6b-137">instancePath</span></span>|<span data-ttu-id="53b6b-138">String</span><span class="sxs-lookup"><span data-stu-id="53b6b-138">String</span></span>|<span data-ttu-id="53b6b-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="53b6b-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="53b6b-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53b6b-140">unknownDeviceCount</span></span>|<span data-ttu-id="53b6b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="53b6b-141">Int32</span></span>|<span data-ttu-id="53b6b-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="53b6b-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="53b6b-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53b6b-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="53b6b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="53b6b-144">Int32</span></span>|<span data-ttu-id="53b6b-145">设置的设备不适用计数</span><span class="sxs-lookup"><span data-stu-id="53b6b-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="53b6b-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53b6b-146">compliantDeviceCount</span></span>|<span data-ttu-id="53b6b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="53b6b-147">Int32</span></span>|<span data-ttu-id="53b6b-148">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="53b6b-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="53b6b-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53b6b-149">remediatedDeviceCount</span></span>|<span data-ttu-id="53b6b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="53b6b-150">Int32</span></span>|<span data-ttu-id="53b6b-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="53b6b-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="53b6b-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53b6b-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="53b6b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="53b6b-153">Int32</span></span>|<span data-ttu-id="53b6b-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="53b6b-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="53b6b-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53b6b-155">errorDeviceCount</span></span>|<span data-ttu-id="53b6b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="53b6b-156">Int32</span></span>|<span data-ttu-id="53b6b-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="53b6b-157">Device error count for the setting</span></span>|
|<span data-ttu-id="53b6b-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53b6b-158">conflictDeviceCount</span></span>|<span data-ttu-id="53b6b-159">Int32</span><span class="sxs-lookup"><span data-stu-id="53b6b-159">Int32</span></span>|<span data-ttu-id="53b6b-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="53b6b-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="53b6b-161">响应</span><span class="sxs-lookup"><span data-stu-id="53b6b-161">Response</span></span>
<span data-ttu-id="53b6b-162">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53b6b-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b6b-163">示例</span><span class="sxs-lookup"><span data-stu-id="53b6b-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="53b6b-164">请求</span><span class="sxs-lookup"><span data-stu-id="53b6b-164">Request</span></span>
<span data-ttu-id="53b6b-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53b6b-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="53b6b-166">响应</span><span class="sxs-lookup"><span data-stu-id="53b6b-166">Response</span></span>
<span data-ttu-id="53b6b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53b6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



