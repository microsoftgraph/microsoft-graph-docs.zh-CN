---
title: 创建 deviceCompliancePolicySettingStateSummary
description: 创建新的 deviceCompliancePolicySettingStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ccd9ce498af34ec2f0f3640572a336cb5f82c874
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017782"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="4eb76-103">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="4eb76-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="4eb76-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4eb76-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eb76-105">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4eb76-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eb76-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4eb76-106">Prerequisites</span></span>
<span data-ttu-id="4eb76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4eb76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb76-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4eb76-109">Permission type</span></span>|<span data-ttu-id="4eb76-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4eb76-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eb76-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4eb76-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4eb76-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb76-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4eb76-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4eb76-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eb76-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4eb76-114">Not supported.</span></span>|
|<span data-ttu-id="4eb76-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4eb76-115">Application</span></span>|<span data-ttu-id="4eb76-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4eb76-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eb76-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4eb76-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4eb76-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4eb76-118">Request headers</span></span>
|<span data-ttu-id="4eb76-119">标头</span><span class="sxs-lookup"><span data-stu-id="4eb76-119">Header</span></span>|<span data-ttu-id="4eb76-120">值</span><span class="sxs-lookup"><span data-stu-id="4eb76-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eb76-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eb76-121">Authorization</span></span>|<span data-ttu-id="4eb76-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4eb76-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eb76-123">接受</span><span class="sxs-lookup"><span data-stu-id="4eb76-123">Accept</span></span>|<span data-ttu-id="4eb76-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4eb76-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eb76-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4eb76-125">Request body</span></span>
<span data-ttu-id="4eb76-126">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eb76-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="4eb76-127">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4eb76-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="4eb76-128">属性</span><span class="sxs-lookup"><span data-stu-id="4eb76-128">Property</span></span>|<span data-ttu-id="4eb76-129">类型</span><span class="sxs-lookup"><span data-stu-id="4eb76-129">Type</span></span>|<span data-ttu-id="4eb76-130">说明</span><span class="sxs-lookup"><span data-stu-id="4eb76-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb76-131">id</span><span class="sxs-lookup"><span data-stu-id="4eb76-131">id</span></span>|<span data-ttu-id="4eb76-132">String</span><span class="sxs-lookup"><span data-stu-id="4eb76-132">String</span></span>|<span data-ttu-id="4eb76-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4eb76-133">Key of the entity.</span></span>|
|<span data-ttu-id="4eb76-134">setting</span><span class="sxs-lookup"><span data-stu-id="4eb76-134">setting</span></span>|<span data-ttu-id="4eb76-135">String</span><span class="sxs-lookup"><span data-stu-id="4eb76-135">String</span></span>|<span data-ttu-id="4eb76-136">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="4eb76-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="4eb76-137">settingName</span><span class="sxs-lookup"><span data-stu-id="4eb76-137">settingName</span></span>|<span data-ttu-id="4eb76-138">String</span><span class="sxs-lookup"><span data-stu-id="4eb76-138">String</span></span>|<span data-ttu-id="4eb76-139">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="4eb76-139">Name of the setting.</span></span>|
|<span data-ttu-id="4eb76-140">platformType</span><span class="sxs-lookup"><span data-stu-id="4eb76-140">platformType</span></span>|[<span data-ttu-id="4eb76-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="4eb76-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="4eb76-142">设置平台。</span><span class="sxs-lookup"><span data-stu-id="4eb76-142">Setting platform.</span></span> <span data-ttu-id="4eb76-143">可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="4eb76-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="4eb76-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eb76-144">unknownDeviceCount</span></span>|<span data-ttu-id="4eb76-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb76-145">Int32</span></span>|<span data-ttu-id="4eb76-146">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="4eb76-146">Number of unknown devices</span></span>|
|<span data-ttu-id="4eb76-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eb76-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="4eb76-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb76-148">Int32</span></span>|<span data-ttu-id="4eb76-149">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="4eb76-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="4eb76-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eb76-150">compliantDeviceCount</span></span>|<span data-ttu-id="4eb76-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb76-151">Int32</span></span>|<span data-ttu-id="4eb76-152">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="4eb76-152">Number of compliant devices</span></span>|
|<span data-ttu-id="4eb76-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eb76-153">remediatedDeviceCount</span></span>|<span data-ttu-id="4eb76-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb76-154">Int32</span></span>|<span data-ttu-id="4eb76-155">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="4eb76-155">Number of remediated devices</span></span>|
|<span data-ttu-id="4eb76-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eb76-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4eb76-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb76-157">Int32</span></span>|<span data-ttu-id="4eb76-158">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="4eb76-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="4eb76-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eb76-159">errorDeviceCount</span></span>|<span data-ttu-id="4eb76-160">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb76-160">Int32</span></span>|<span data-ttu-id="4eb76-161">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="4eb76-161">Number of error devices</span></span>|
|<span data-ttu-id="4eb76-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4eb76-162">conflictDeviceCount</span></span>|<span data-ttu-id="4eb76-163">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb76-163">Int32</span></span>|<span data-ttu-id="4eb76-164">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="4eb76-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="4eb76-165">响应</span><span class="sxs-lookup"><span data-stu-id="4eb76-165">Response</span></span>
<span data-ttu-id="4eb76-166">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4eb76-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eb76-167">示例</span><span class="sxs-lookup"><span data-stu-id="4eb76-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eb76-168">请求</span><span class="sxs-lookup"><span data-stu-id="4eb76-168">Request</span></span>
<span data-ttu-id="4eb76-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4eb76-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4eb76-170">响应</span><span class="sxs-lookup"><span data-stu-id="4eb76-170">Response</span></span>
<span data-ttu-id="4eb76-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4eb76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



