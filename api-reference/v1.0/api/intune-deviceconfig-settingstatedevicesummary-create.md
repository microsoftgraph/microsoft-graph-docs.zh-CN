---
title: 创建 settingStateDeviceSummary
description: 创建新的 settingStateDeviceSummary 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a535f6a83be088b1798ee2baf3b8031cd69ddb9c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365843"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="a455f-103">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a455f-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="a455f-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a455f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a455f-105">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a455f-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a455f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a455f-106">Prerequisites</span></span>
<span data-ttu-id="a455f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a455f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a455f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a455f-109">Permission type</span></span>|<span data-ttu-id="a455f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a455f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a455f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a455f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a455f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a455f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a455f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a455f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a455f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a455f-114">Not supported.</span></span>|
|<span data-ttu-id="a455f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a455f-115">Application</span></span>|<span data-ttu-id="a455f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a455f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a455f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a455f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a455f-118">请求头</span><span class="sxs-lookup"><span data-stu-id="a455f-118">Request headers</span></span>
|<span data-ttu-id="a455f-119">标头</span><span class="sxs-lookup"><span data-stu-id="a455f-119">Header</span></span>|<span data-ttu-id="a455f-120">值</span><span class="sxs-lookup"><span data-stu-id="a455f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a455f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a455f-121">Authorization</span></span>|<span data-ttu-id="a455f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a455f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a455f-123">接受</span><span class="sxs-lookup"><span data-stu-id="a455f-123">Accept</span></span>|<span data-ttu-id="a455f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a455f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a455f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a455f-125">Request body</span></span>
<span data-ttu-id="a455f-126">在请求正文中，提供 settingStateDeviceSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a455f-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="a455f-127">下表显示了创建 settingStateDeviceSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a455f-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="a455f-128">属性</span><span class="sxs-lookup"><span data-stu-id="a455f-128">Property</span></span>|<span data-ttu-id="a455f-129">类型</span><span class="sxs-lookup"><span data-stu-id="a455f-129">Type</span></span>|<span data-ttu-id="a455f-130">说明</span><span class="sxs-lookup"><span data-stu-id="a455f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a455f-131">id</span><span class="sxs-lookup"><span data-stu-id="a455f-131">id</span></span>|<span data-ttu-id="a455f-132">String</span><span class="sxs-lookup"><span data-stu-id="a455f-132">String</span></span>|<span data-ttu-id="a455f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a455f-133">Key of the entity.</span></span>|
|<span data-ttu-id="a455f-134">settingName</span><span class="sxs-lookup"><span data-stu-id="a455f-134">settingName</span></span>|<span data-ttu-id="a455f-135">String</span><span class="sxs-lookup"><span data-stu-id="a455f-135">String</span></span>|<span data-ttu-id="a455f-136">设置的名称</span><span class="sxs-lookup"><span data-stu-id="a455f-136">Name of the setting</span></span>|
|<span data-ttu-id="a455f-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="a455f-137">instancePath</span></span>|<span data-ttu-id="a455f-138">String</span><span class="sxs-lookup"><span data-stu-id="a455f-138">String</span></span>|<span data-ttu-id="a455f-139">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="a455f-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="a455f-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a455f-140">unknownDeviceCount</span></span>|<span data-ttu-id="a455f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a455f-141">Int32</span></span>|<span data-ttu-id="a455f-142">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="a455f-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="a455f-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a455f-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="a455f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a455f-144">Int32</span></span>|<span data-ttu-id="a455f-145">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="a455f-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="a455f-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a455f-146">compliantDeviceCount</span></span>|<span data-ttu-id="a455f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a455f-147">Int32</span></span>|<span data-ttu-id="a455f-148">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="a455f-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a455f-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a455f-149">remediatedDeviceCount</span></span>|<span data-ttu-id="a455f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a455f-150">Int32</span></span>|<span data-ttu-id="a455f-151">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="a455f-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a455f-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a455f-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a455f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a455f-153">Int32</span></span>|<span data-ttu-id="a455f-154">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="a455f-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="a455f-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a455f-155">errorDeviceCount</span></span>|<span data-ttu-id="a455f-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a455f-156">Int32</span></span>|<span data-ttu-id="a455f-157">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="a455f-157">Device error count for the setting</span></span>|
|<span data-ttu-id="a455f-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a455f-158">conflictDeviceCount</span></span>|<span data-ttu-id="a455f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a455f-159">Int32</span></span>|<span data-ttu-id="a455f-160">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="a455f-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="a455f-161">响应</span><span class="sxs-lookup"><span data-stu-id="a455f-161">Response</span></span>
<span data-ttu-id="a455f-162">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a455f-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a455f-163">示例</span><span class="sxs-lookup"><span data-stu-id="a455f-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a455f-164">请求</span><span class="sxs-lookup"><span data-stu-id="a455f-164">Request</span></span>
<span data-ttu-id="a455f-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a455f-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a455f-166">响应</span><span class="sxs-lookup"><span data-stu-id="a455f-166">Response</span></span>
<span data-ttu-id="a455f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a455f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




