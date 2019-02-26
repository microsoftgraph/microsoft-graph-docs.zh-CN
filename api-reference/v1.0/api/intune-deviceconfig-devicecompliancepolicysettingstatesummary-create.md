---
title: 创建 deviceCompliancePolicySettingStateSummary
description: 创建新的 deviceCompliancePolicySettingStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f027d182222f496bab1a6ec3e74bf3bbd72935d1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256901"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="cc8e9-103">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="cc8e9-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="cc8e9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc8e9-105">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc8e9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cc8e9-106">Prerequisites</span></span>
<span data-ttu-id="cc8e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc8e9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc8e9-109">Permission type</span></span>|<span data-ttu-id="cc8e9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cc8e9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc8e9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc8e9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cc8e9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc8e9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc8e9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc8e9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc8e9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-114">Not supported.</span></span>|
|<span data-ttu-id="cc8e9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc8e9-115">Application</span></span>|<span data-ttu-id="cc8e9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc8e9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc8e9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="cc8e9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc8e9-118">Request headers</span></span>
|<span data-ttu-id="cc8e9-119">标头</span><span class="sxs-lookup"><span data-stu-id="cc8e9-119">Header</span></span>|<span data-ttu-id="cc8e9-120">值</span><span class="sxs-lookup"><span data-stu-id="cc8e9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc8e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc8e9-121">Authorization</span></span>|<span data-ttu-id="cc8e9-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc8e9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cc8e9-123">Accept</span></span>|<span data-ttu-id="cc8e9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cc8e9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc8e9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc8e9-125">Request body</span></span>
<span data-ttu-id="cc8e9-126">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="cc8e9-127">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="cc8e9-128">属性</span><span class="sxs-lookup"><span data-stu-id="cc8e9-128">Property</span></span>|<span data-ttu-id="cc8e9-129">类型</span><span class="sxs-lookup"><span data-stu-id="cc8e9-129">Type</span></span>|<span data-ttu-id="cc8e9-130">说明</span><span class="sxs-lookup"><span data-stu-id="cc8e9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc8e9-131">id</span><span class="sxs-lookup"><span data-stu-id="cc8e9-131">id</span></span>|<span data-ttu-id="cc8e9-132">字符串</span><span class="sxs-lookup"><span data-stu-id="cc8e9-132">String</span></span>|<span data-ttu-id="cc8e9-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-133">Key of the entity.</span></span>|
|<span data-ttu-id="cc8e9-134">setting</span><span class="sxs-lookup"><span data-stu-id="cc8e9-134">setting</span></span>|<span data-ttu-id="cc8e9-135">String</span><span class="sxs-lookup"><span data-stu-id="cc8e9-135">String</span></span>|<span data-ttu-id="cc8e9-136">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="cc8e9-137">settingName</span><span class="sxs-lookup"><span data-stu-id="cc8e9-137">settingName</span></span>|<span data-ttu-id="cc8e9-138">String</span><span class="sxs-lookup"><span data-stu-id="cc8e9-138">String</span></span>|<span data-ttu-id="cc8e9-139">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-139">Name of the setting.</span></span>|
|<span data-ttu-id="cc8e9-140">platformType</span><span class="sxs-lookup"><span data-stu-id="cc8e9-140">platformType</span></span>|[<span data-ttu-id="cc8e9-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="cc8e9-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="cc8e9-142">设置平台。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-142">Setting platform.</span></span> <span data-ttu-id="cc8e9-143">可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="cc8e9-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc8e9-144">unknownDeviceCount</span></span>|<span data-ttu-id="cc8e9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="cc8e9-145">Int32</span></span>|<span data-ttu-id="cc8e9-146">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="cc8e9-146">Number of unknown devices</span></span>|
|<span data-ttu-id="cc8e9-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc8e9-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="cc8e9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cc8e9-148">Int32</span></span>|<span data-ttu-id="cc8e9-149">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="cc8e9-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="cc8e9-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc8e9-150">compliantDeviceCount</span></span>|<span data-ttu-id="cc8e9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cc8e9-151">Int32</span></span>|<span data-ttu-id="cc8e9-152">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="cc8e9-152">Number of compliant devices</span></span>|
|<span data-ttu-id="cc8e9-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc8e9-153">remediatedDeviceCount</span></span>|<span data-ttu-id="cc8e9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cc8e9-154">Int32</span></span>|<span data-ttu-id="cc8e9-155">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="cc8e9-155">Number of remediated devices</span></span>|
|<span data-ttu-id="cc8e9-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc8e9-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="cc8e9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cc8e9-157">Int32</span></span>|<span data-ttu-id="cc8e9-158">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="cc8e9-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="cc8e9-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc8e9-159">errorDeviceCount</span></span>|<span data-ttu-id="cc8e9-160">Int32</span><span class="sxs-lookup"><span data-stu-id="cc8e9-160">Int32</span></span>|<span data-ttu-id="cc8e9-161">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="cc8e9-161">Number of error devices</span></span>|
|<span data-ttu-id="cc8e9-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cc8e9-162">conflictDeviceCount</span></span>|<span data-ttu-id="cc8e9-163">Int32</span><span class="sxs-lookup"><span data-stu-id="cc8e9-163">Int32</span></span>|<span data-ttu-id="cc8e9-164">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="cc8e9-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="cc8e9-165">响应</span><span class="sxs-lookup"><span data-stu-id="cc8e9-165">Response</span></span>
<span data-ttu-id="cc8e9-166">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc8e9-167">示例</span><span class="sxs-lookup"><span data-stu-id="cc8e9-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc8e9-168">请求</span><span class="sxs-lookup"><span data-stu-id="cc8e9-168">Request</span></span>
<span data-ttu-id="cc8e9-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc8e9-170">响应</span><span class="sxs-lookup"><span data-stu-id="cc8e9-170">Response</span></span>
<span data-ttu-id="cc8e9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc8e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



