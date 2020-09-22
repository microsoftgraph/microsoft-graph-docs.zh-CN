---
title: 创建 deviceCompliancePolicySettingStateSummary
description: 创建新的 deviceCompliancePolicySettingStateSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 86a9c93c07ec2d8f180e146e18b96a32895f92be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083468"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="ea2c0-103">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="ea2c0-103">Create deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="ea2c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea2c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea2c0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea2c0-106">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea2c0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea2c0-107">Prerequisites</span></span>
<span data-ttu-id="ea2c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea2c0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea2c0-110">Permission type</span></span>|<span data-ttu-id="ea2c0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea2c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea2c0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea2c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea2c0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea2c0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea2c0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea2c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea2c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-115">Not supported.</span></span>|
|<span data-ttu-id="ea2c0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea2c0-116">Application</span></span>|<span data-ttu-id="ea2c0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea2c0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea2c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ea2c0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea2c0-119">Request headers</span></span>
|<span data-ttu-id="ea2c0-120">标头</span><span class="sxs-lookup"><span data-stu-id="ea2c0-120">Header</span></span>|<span data-ttu-id="ea2c0-121">值</span><span class="sxs-lookup"><span data-stu-id="ea2c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea2c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea2c0-122">Authorization</span></span>|<span data-ttu-id="ea2c0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea2c0-124">接受</span><span class="sxs-lookup"><span data-stu-id="ea2c0-124">Accept</span></span>|<span data-ttu-id="ea2c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea2c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea2c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea2c0-126">Request body</span></span>
<span data-ttu-id="ea2c0-127">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="ea2c0-128">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="ea2c0-129">属性</span><span class="sxs-lookup"><span data-stu-id="ea2c0-129">Property</span></span>|<span data-ttu-id="ea2c0-130">类型</span><span class="sxs-lookup"><span data-stu-id="ea2c0-130">Type</span></span>|<span data-ttu-id="ea2c0-131">说明</span><span class="sxs-lookup"><span data-stu-id="ea2c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea2c0-132">id</span><span class="sxs-lookup"><span data-stu-id="ea2c0-132">id</span></span>|<span data-ttu-id="ea2c0-133">String</span><span class="sxs-lookup"><span data-stu-id="ea2c0-133">String</span></span>|<span data-ttu-id="ea2c0-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-134">Key of the entity.</span></span>|
|<span data-ttu-id="ea2c0-135">setting</span><span class="sxs-lookup"><span data-stu-id="ea2c0-135">setting</span></span>|<span data-ttu-id="ea2c0-136">String</span><span class="sxs-lookup"><span data-stu-id="ea2c0-136">String</span></span>|<span data-ttu-id="ea2c0-137">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="ea2c0-138">settingName</span><span class="sxs-lookup"><span data-stu-id="ea2c0-138">settingName</span></span>|<span data-ttu-id="ea2c0-139">String</span><span class="sxs-lookup"><span data-stu-id="ea2c0-139">String</span></span>|<span data-ttu-id="ea2c0-140">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-140">Name of the setting.</span></span>|
|<span data-ttu-id="ea2c0-141">platformType</span><span class="sxs-lookup"><span data-stu-id="ea2c0-141">platformType</span></span>|[<span data-ttu-id="ea2c0-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="ea2c0-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="ea2c0-143">设置平台。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-143">Setting platform.</span></span> <span data-ttu-id="ea2c0-144">可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-144">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="ea2c0-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea2c0-145">unknownDeviceCount</span></span>|<span data-ttu-id="ea2c0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ea2c0-146">Int32</span></span>|<span data-ttu-id="ea2c0-147">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="ea2c0-147">Number of unknown devices</span></span>|
|<span data-ttu-id="ea2c0-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea2c0-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="ea2c0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ea2c0-149">Int32</span></span>|<span data-ttu-id="ea2c0-150">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="ea2c0-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="ea2c0-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea2c0-151">compliantDeviceCount</span></span>|<span data-ttu-id="ea2c0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ea2c0-152">Int32</span></span>|<span data-ttu-id="ea2c0-153">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="ea2c0-153">Number of compliant devices</span></span>|
|<span data-ttu-id="ea2c0-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea2c0-154">remediatedDeviceCount</span></span>|<span data-ttu-id="ea2c0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ea2c0-155">Int32</span></span>|<span data-ttu-id="ea2c0-156">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="ea2c0-156">Number of remediated devices</span></span>|
|<span data-ttu-id="ea2c0-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea2c0-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ea2c0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ea2c0-158">Int32</span></span>|<span data-ttu-id="ea2c0-159">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="ea2c0-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ea2c0-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea2c0-160">errorDeviceCount</span></span>|<span data-ttu-id="ea2c0-161">Int32</span><span class="sxs-lookup"><span data-stu-id="ea2c0-161">Int32</span></span>|<span data-ttu-id="ea2c0-162">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="ea2c0-162">Number of error devices</span></span>|
|<span data-ttu-id="ea2c0-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ea2c0-163">conflictDeviceCount</span></span>|<span data-ttu-id="ea2c0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ea2c0-164">Int32</span></span>|<span data-ttu-id="ea2c0-165">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="ea2c0-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="ea2c0-166">响应</span><span class="sxs-lookup"><span data-stu-id="ea2c0-166">Response</span></span>
<span data-ttu-id="ea2c0-167">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea2c0-168">示例</span><span class="sxs-lookup"><span data-stu-id="ea2c0-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea2c0-169">请求</span><span class="sxs-lookup"><span data-stu-id="ea2c0-169">Request</span></span>
<span data-ttu-id="ea2c0-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="ea2c0-171">响应</span><span class="sxs-lookup"><span data-stu-id="ea2c0-171">Response</span></span>
<span data-ttu-id="ea2c0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea2c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```









