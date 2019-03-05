---
title: 创建 deviceCompliancePolicySettingStateSummary
description: 创建新的 deviceCompliancePolicySettingStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 110b3853c7e36280cf530f6d5d18a197cfd33230
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170922"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="578e0-103">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="578e0-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="578e0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="578e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="578e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="578e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="578e0-106">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="578e0-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="578e0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="578e0-107">Prerequisites</span></span>
<span data-ttu-id="578e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="578e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="578e0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="578e0-110">Permission type</span></span>|<span data-ttu-id="578e0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="578e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="578e0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="578e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="578e0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="578e0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="578e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="578e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="578e0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="578e0-115">Not supported.</span></span>|
|<span data-ttu-id="578e0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="578e0-116">Application</span></span>|<span data-ttu-id="578e0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="578e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="578e0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="578e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="578e0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="578e0-119">Request headers</span></span>
|<span data-ttu-id="578e0-120">标头</span><span class="sxs-lookup"><span data-stu-id="578e0-120">Header</span></span>|<span data-ttu-id="578e0-121">值</span><span class="sxs-lookup"><span data-stu-id="578e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="578e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="578e0-122">Authorization</span></span>|<span data-ttu-id="578e0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="578e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="578e0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="578e0-124">Accept</span></span>|<span data-ttu-id="578e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="578e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="578e0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="578e0-126">Request body</span></span>
<span data-ttu-id="578e0-127">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="578e0-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="578e0-128">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="578e0-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="578e0-129">属性</span><span class="sxs-lookup"><span data-stu-id="578e0-129">Property</span></span>|<span data-ttu-id="578e0-130">类型</span><span class="sxs-lookup"><span data-stu-id="578e0-130">Type</span></span>|<span data-ttu-id="578e0-131">说明</span><span class="sxs-lookup"><span data-stu-id="578e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="578e0-132">id</span><span class="sxs-lookup"><span data-stu-id="578e0-132">id</span></span>|<span data-ttu-id="578e0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="578e0-133">String</span></span>|<span data-ttu-id="578e0-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="578e0-134">Key of the entity.</span></span>|
|<span data-ttu-id="578e0-135">setting</span><span class="sxs-lookup"><span data-stu-id="578e0-135">setting</span></span>|<span data-ttu-id="578e0-136">String</span><span class="sxs-lookup"><span data-stu-id="578e0-136">String</span></span>|<span data-ttu-id="578e0-137">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="578e0-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="578e0-138">settingName</span><span class="sxs-lookup"><span data-stu-id="578e0-138">settingName</span></span>|<span data-ttu-id="578e0-139">String</span><span class="sxs-lookup"><span data-stu-id="578e0-139">String</span></span>|<span data-ttu-id="578e0-140">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="578e0-140">Name of the setting.</span></span>|
|<span data-ttu-id="578e0-141">platformType</span><span class="sxs-lookup"><span data-stu-id="578e0-141">platformType</span></span>|[<span data-ttu-id="578e0-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="578e0-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="578e0-143">设置平台。</span><span class="sxs-lookup"><span data-stu-id="578e0-143">Setting platform.</span></span> <span data-ttu-id="578e0-144">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="578e0-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="578e0-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="578e0-145">unknownDeviceCount</span></span>|<span data-ttu-id="578e0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="578e0-146">Int32</span></span>|<span data-ttu-id="578e0-147">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="578e0-147">Number of unknown devices</span></span>|
|<span data-ttu-id="578e0-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="578e0-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="578e0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="578e0-149">Int32</span></span>|<span data-ttu-id="578e0-150">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="578e0-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="578e0-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="578e0-151">compliantDeviceCount</span></span>|<span data-ttu-id="578e0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="578e0-152">Int32</span></span>|<span data-ttu-id="578e0-153">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="578e0-153">Number of compliant devices</span></span>|
|<span data-ttu-id="578e0-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="578e0-154">remediatedDeviceCount</span></span>|<span data-ttu-id="578e0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="578e0-155">Int32</span></span>|<span data-ttu-id="578e0-156">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="578e0-156">Number of remediated devices</span></span>|
|<span data-ttu-id="578e0-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="578e0-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="578e0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="578e0-158">Int32</span></span>|<span data-ttu-id="578e0-159">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="578e0-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="578e0-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="578e0-160">errorDeviceCount</span></span>|<span data-ttu-id="578e0-161">Int32</span><span class="sxs-lookup"><span data-stu-id="578e0-161">Int32</span></span>|<span data-ttu-id="578e0-162">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="578e0-162">Number of error devices</span></span>|
|<span data-ttu-id="578e0-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="578e0-163">conflictDeviceCount</span></span>|<span data-ttu-id="578e0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="578e0-164">Int32</span></span>|<span data-ttu-id="578e0-165">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="578e0-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="578e0-166">响应</span><span class="sxs-lookup"><span data-stu-id="578e0-166">Response</span></span>
<span data-ttu-id="578e0-167">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="578e0-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="578e0-168">示例</span><span class="sxs-lookup"><span data-stu-id="578e0-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="578e0-169">请求</span><span class="sxs-lookup"><span data-stu-id="578e0-169">Request</span></span>
<span data-ttu-id="578e0-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="578e0-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="578e0-171">响应</span><span class="sxs-lookup"><span data-stu-id="578e0-171">Response</span></span>
<span data-ttu-id="578e0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="578e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




