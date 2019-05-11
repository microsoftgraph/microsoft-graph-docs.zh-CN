---
title: 更新 deviceCompliancePolicySettingStateSummary
description: 更新 deviceCompliancePolicySettingStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d5b85775a0b3562af129b2e020872da086131e8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927816"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="0f96e-103">更新 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="0f96e-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="0f96e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f96e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f96e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f96e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f96e-106">更新 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0f96e-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f96e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f96e-107">Prerequisites</span></span>
<span data-ttu-id="0f96e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f96e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f96e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f96e-110">Permission type</span></span>|<span data-ttu-id="0f96e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f96e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f96e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f96e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f96e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f96e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f96e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f96e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f96e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f96e-115">Not supported.</span></span>|
|<span data-ttu-id="0f96e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f96e-116">Application</span></span>|<span data-ttu-id="0f96e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f96e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f96e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f96e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="0f96e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f96e-119">Request headers</span></span>
|<span data-ttu-id="0f96e-120">标头</span><span class="sxs-lookup"><span data-stu-id="0f96e-120">Header</span></span>|<span data-ttu-id="0f96e-121">值</span><span class="sxs-lookup"><span data-stu-id="0f96e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f96e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f96e-122">Authorization</span></span>|<span data-ttu-id="0f96e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f96e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f96e-124">接受</span><span class="sxs-lookup"><span data-stu-id="0f96e-124">Accept</span></span>|<span data-ttu-id="0f96e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f96e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f96e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f96e-126">Request body</span></span>
<span data-ttu-id="0f96e-127">在请求正文中，提供 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f96e-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="0f96e-128">下表显示创建 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0f96e-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="0f96e-129">属性</span><span class="sxs-lookup"><span data-stu-id="0f96e-129">Property</span></span>|<span data-ttu-id="0f96e-130">类型</span><span class="sxs-lookup"><span data-stu-id="0f96e-130">Type</span></span>|<span data-ttu-id="0f96e-131">说明</span><span class="sxs-lookup"><span data-stu-id="0f96e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f96e-132">id</span><span class="sxs-lookup"><span data-stu-id="0f96e-132">id</span></span>|<span data-ttu-id="0f96e-133">String</span><span class="sxs-lookup"><span data-stu-id="0f96e-133">String</span></span>|<span data-ttu-id="0f96e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f96e-134">Key of the entity.</span></span>|
|<span data-ttu-id="0f96e-135">setting</span><span class="sxs-lookup"><span data-stu-id="0f96e-135">setting</span></span>|<span data-ttu-id="0f96e-136">String</span><span class="sxs-lookup"><span data-stu-id="0f96e-136">String</span></span>|<span data-ttu-id="0f96e-137">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="0f96e-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="0f96e-138">settingName</span><span class="sxs-lookup"><span data-stu-id="0f96e-138">settingName</span></span>|<span data-ttu-id="0f96e-139">String</span><span class="sxs-lookup"><span data-stu-id="0f96e-139">String</span></span>|<span data-ttu-id="0f96e-140">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="0f96e-140">Name of the setting.</span></span>|
|<span data-ttu-id="0f96e-141">platformType</span><span class="sxs-lookup"><span data-stu-id="0f96e-141">platformType</span></span>|[<span data-ttu-id="0f96e-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0f96e-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="0f96e-143">设置平台。</span><span class="sxs-lookup"><span data-stu-id="0f96e-143">Setting platform.</span></span> <span data-ttu-id="0f96e-144">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="0f96e-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="0f96e-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f96e-145">unknownDeviceCount</span></span>|<span data-ttu-id="0f96e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0f96e-146">Int32</span></span>|<span data-ttu-id="0f96e-147">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="0f96e-147">Number of unknown devices</span></span>|
|<span data-ttu-id="0f96e-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f96e-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="0f96e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0f96e-149">Int32</span></span>|<span data-ttu-id="0f96e-150">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="0f96e-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="0f96e-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f96e-151">compliantDeviceCount</span></span>|<span data-ttu-id="0f96e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0f96e-152">Int32</span></span>|<span data-ttu-id="0f96e-153">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="0f96e-153">Number of compliant devices</span></span>|
|<span data-ttu-id="0f96e-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f96e-154">remediatedDeviceCount</span></span>|<span data-ttu-id="0f96e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="0f96e-155">Int32</span></span>|<span data-ttu-id="0f96e-156">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="0f96e-156">Number of remediated devices</span></span>|
|<span data-ttu-id="0f96e-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f96e-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0f96e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0f96e-158">Int32</span></span>|<span data-ttu-id="0f96e-159">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="0f96e-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="0f96e-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f96e-160">errorDeviceCount</span></span>|<span data-ttu-id="0f96e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0f96e-161">Int32</span></span>|<span data-ttu-id="0f96e-162">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="0f96e-162">Number of error devices</span></span>|
|<span data-ttu-id="0f96e-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f96e-163">conflictDeviceCount</span></span>|<span data-ttu-id="0f96e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0f96e-164">Int32</span></span>|<span data-ttu-id="0f96e-165">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="0f96e-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="0f96e-166">响应</span><span class="sxs-lookup"><span data-stu-id="0f96e-166">Response</span></span>
<span data-ttu-id="0f96e-167">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0f96e-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f96e-168">示例</span><span class="sxs-lookup"><span data-stu-id="0f96e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f96e-169">请求</span><span class="sxs-lookup"><span data-stu-id="0f96e-169">Request</span></span>
<span data-ttu-id="0f96e-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f96e-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="0f96e-171">响应</span><span class="sxs-lookup"><span data-stu-id="0f96e-171">Response</span></span>
<span data-ttu-id="0f96e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f96e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




