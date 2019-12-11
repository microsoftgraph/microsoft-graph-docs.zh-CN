---
title: 更新 deviceCompliancePolicySettingStateSummary
description: 更新 deviceCompliancePolicySettingStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebad7ddb10eeaa4b897c126f3ae86389727d0e30
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949621"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="d772b-103">更新 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="d772b-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="d772b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d772b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d772b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d772b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d772b-106">更新 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d772b-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d772b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d772b-107">Prerequisites</span></span>
<span data-ttu-id="d772b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d772b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d772b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d772b-110">Permission type</span></span>|<span data-ttu-id="d772b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d772b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d772b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d772b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d772b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d772b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d772b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d772b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d772b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d772b-115">Not supported.</span></span>|
|<span data-ttu-id="d772b-116">Application</span><span class="sxs-lookup"><span data-stu-id="d772b-116">Application</span></span>|<span data-ttu-id="d772b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d772b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d772b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d772b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d772b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d772b-119">Request headers</span></span>
|<span data-ttu-id="d772b-120">标头</span><span class="sxs-lookup"><span data-stu-id="d772b-120">Header</span></span>|<span data-ttu-id="d772b-121">值</span><span class="sxs-lookup"><span data-stu-id="d772b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d772b-122">授权</span><span class="sxs-lookup"><span data-stu-id="d772b-122">Authorization</span></span>|<span data-ttu-id="d772b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d772b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d772b-124">接受</span><span class="sxs-lookup"><span data-stu-id="d772b-124">Accept</span></span>|<span data-ttu-id="d772b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d772b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d772b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d772b-126">Request body</span></span>
<span data-ttu-id="d772b-127">在请求正文中，提供 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d772b-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="d772b-128">下表显示创建 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d772b-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="d772b-129">属性</span><span class="sxs-lookup"><span data-stu-id="d772b-129">Property</span></span>|<span data-ttu-id="d772b-130">类型</span><span class="sxs-lookup"><span data-stu-id="d772b-130">Type</span></span>|<span data-ttu-id="d772b-131">说明</span><span class="sxs-lookup"><span data-stu-id="d772b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d772b-132">id</span><span class="sxs-lookup"><span data-stu-id="d772b-132">id</span></span>|<span data-ttu-id="d772b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d772b-133">String</span></span>|<span data-ttu-id="d772b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d772b-134">Key of the entity.</span></span>|
|<span data-ttu-id="d772b-135">setting</span><span class="sxs-lookup"><span data-stu-id="d772b-135">setting</span></span>|<span data-ttu-id="d772b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="d772b-136">String</span></span>|<span data-ttu-id="d772b-137">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="d772b-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="d772b-138">settingName</span><span class="sxs-lookup"><span data-stu-id="d772b-138">settingName</span></span>|<span data-ttu-id="d772b-139">String</span><span class="sxs-lookup"><span data-stu-id="d772b-139">String</span></span>|<span data-ttu-id="d772b-140">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="d772b-140">Name of the setting.</span></span>|
|<span data-ttu-id="d772b-141">platformType</span><span class="sxs-lookup"><span data-stu-id="d772b-141">platformType</span></span>|[<span data-ttu-id="d772b-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="d772b-142">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="d772b-143">设置平台。</span><span class="sxs-lookup"><span data-stu-id="d772b-143">Setting platform.</span></span> <span data-ttu-id="d772b-144">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="d772b-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="d772b-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d772b-145">unknownDeviceCount</span></span>|<span data-ttu-id="d772b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d772b-146">Int32</span></span>|<span data-ttu-id="d772b-147">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="d772b-147">Number of unknown devices</span></span>|
|<span data-ttu-id="d772b-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d772b-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="d772b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d772b-149">Int32</span></span>|<span data-ttu-id="d772b-150">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="d772b-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="d772b-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d772b-151">compliantDeviceCount</span></span>|<span data-ttu-id="d772b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d772b-152">Int32</span></span>|<span data-ttu-id="d772b-153">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="d772b-153">Number of compliant devices</span></span>|
|<span data-ttu-id="d772b-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d772b-154">remediatedDeviceCount</span></span>|<span data-ttu-id="d772b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d772b-155">Int32</span></span>|<span data-ttu-id="d772b-156">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="d772b-156">Number of remediated devices</span></span>|
|<span data-ttu-id="d772b-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d772b-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d772b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d772b-158">Int32</span></span>|<span data-ttu-id="d772b-159">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="d772b-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d772b-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d772b-160">errorDeviceCount</span></span>|<span data-ttu-id="d772b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d772b-161">Int32</span></span>|<span data-ttu-id="d772b-162">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="d772b-162">Number of error devices</span></span>|
|<span data-ttu-id="d772b-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d772b-163">conflictDeviceCount</span></span>|<span data-ttu-id="d772b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d772b-164">Int32</span></span>|<span data-ttu-id="d772b-165">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="d772b-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="d772b-166">响应</span><span class="sxs-lookup"><span data-stu-id="d772b-166">Response</span></span>
<span data-ttu-id="d772b-167">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d772b-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d772b-168">示例</span><span class="sxs-lookup"><span data-stu-id="d772b-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d772b-169">请求</span><span class="sxs-lookup"><span data-stu-id="d772b-169">Request</span></span>
<span data-ttu-id="d772b-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d772b-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d772b-171">响应</span><span class="sxs-lookup"><span data-stu-id="d772b-171">Response</span></span>
<span data-ttu-id="d772b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d772b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





