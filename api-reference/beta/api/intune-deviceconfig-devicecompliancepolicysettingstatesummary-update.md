---
title: 更新 deviceCompliancePolicySettingStateSummary
description: 更新 deviceCompliancePolicySettingStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10f269b7db39d15eb008fa5a26dd513f8fdc2de5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443179"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="b8628-103">更新 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="b8628-103">Update deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="b8628-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b8628-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8628-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8628-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8628-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8628-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8628-107">更新 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8628-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8628-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8628-108">Prerequisites</span></span>
<span data-ttu-id="b8628-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8628-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8628-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8628-111">Permission type</span></span>|<span data-ttu-id="b8628-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8628-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8628-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8628-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8628-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8628-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8628-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8628-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8628-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8628-116">Not supported.</span></span>|
|<span data-ttu-id="b8628-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8628-117">Application</span></span>|<span data-ttu-id="b8628-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8628-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8628-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8628-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b8628-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8628-120">Request headers</span></span>
|<span data-ttu-id="b8628-121">标头</span><span class="sxs-lookup"><span data-stu-id="b8628-121">Header</span></span>|<span data-ttu-id="b8628-122">值</span><span class="sxs-lookup"><span data-stu-id="b8628-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8628-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8628-123">Authorization</span></span>|<span data-ttu-id="b8628-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8628-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8628-125">接受</span><span class="sxs-lookup"><span data-stu-id="b8628-125">Accept</span></span>|<span data-ttu-id="b8628-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8628-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8628-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8628-127">Request body</span></span>
<span data-ttu-id="b8628-128">在请求正文中，提供 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8628-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="b8628-129">下表显示创建 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8628-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="b8628-130">属性</span><span class="sxs-lookup"><span data-stu-id="b8628-130">Property</span></span>|<span data-ttu-id="b8628-131">类型</span><span class="sxs-lookup"><span data-stu-id="b8628-131">Type</span></span>|<span data-ttu-id="b8628-132">说明</span><span class="sxs-lookup"><span data-stu-id="b8628-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8628-133">id</span><span class="sxs-lookup"><span data-stu-id="b8628-133">id</span></span>|<span data-ttu-id="b8628-134">String</span><span class="sxs-lookup"><span data-stu-id="b8628-134">String</span></span>|<span data-ttu-id="b8628-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8628-135">Key of the entity.</span></span>|
|<span data-ttu-id="b8628-136">setting</span><span class="sxs-lookup"><span data-stu-id="b8628-136">setting</span></span>|<span data-ttu-id="b8628-137">String</span><span class="sxs-lookup"><span data-stu-id="b8628-137">String</span></span>|<span data-ttu-id="b8628-138">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="b8628-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="b8628-139">settingName</span><span class="sxs-lookup"><span data-stu-id="b8628-139">settingName</span></span>|<span data-ttu-id="b8628-140">String</span><span class="sxs-lookup"><span data-stu-id="b8628-140">String</span></span>|<span data-ttu-id="b8628-141">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="b8628-141">Name of the setting.</span></span>|
|<span data-ttu-id="b8628-142">platformType</span><span class="sxs-lookup"><span data-stu-id="b8628-142">platformType</span></span>|[<span data-ttu-id="b8628-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="b8628-143">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="b8628-144">设置平台。</span><span class="sxs-lookup"><span data-stu-id="b8628-144">Setting platform.</span></span> <span data-ttu-id="b8628-145">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="b8628-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="b8628-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8628-146">unknownDeviceCount</span></span>|<span data-ttu-id="b8628-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b8628-147">Int32</span></span>|<span data-ttu-id="b8628-148">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="b8628-148">Number of unknown devices</span></span>|
|<span data-ttu-id="b8628-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8628-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="b8628-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b8628-150">Int32</span></span>|<span data-ttu-id="b8628-151">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="b8628-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="b8628-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8628-152">compliantDeviceCount</span></span>|<span data-ttu-id="b8628-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b8628-153">Int32</span></span>|<span data-ttu-id="b8628-154">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="b8628-154">Number of compliant devices</span></span>|
|<span data-ttu-id="b8628-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8628-155">remediatedDeviceCount</span></span>|<span data-ttu-id="b8628-156">Int32</span><span class="sxs-lookup"><span data-stu-id="b8628-156">Int32</span></span>|<span data-ttu-id="b8628-157">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="b8628-157">Number of remediated devices</span></span>|
|<span data-ttu-id="b8628-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8628-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b8628-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b8628-159">Int32</span></span>|<span data-ttu-id="b8628-160">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="b8628-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="b8628-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8628-161">errorDeviceCount</span></span>|<span data-ttu-id="b8628-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b8628-162">Int32</span></span>|<span data-ttu-id="b8628-163">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="b8628-163">Number of error devices</span></span>|
|<span data-ttu-id="b8628-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b8628-164">conflictDeviceCount</span></span>|<span data-ttu-id="b8628-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b8628-165">Int32</span></span>|<span data-ttu-id="b8628-166">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="b8628-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="b8628-167">响应</span><span class="sxs-lookup"><span data-stu-id="b8628-167">Response</span></span>
<span data-ttu-id="b8628-168">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8628-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8628-169">示例</span><span class="sxs-lookup"><span data-stu-id="b8628-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8628-170">请求</span><span class="sxs-lookup"><span data-stu-id="b8628-170">Request</span></span>
<span data-ttu-id="b8628-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8628-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8628-172">响应</span><span class="sxs-lookup"><span data-stu-id="b8628-172">Response</span></span>
<span data-ttu-id="b8628-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8628-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





