---
title: 创建 deviceCompliancePolicySettingStateSummary
description: 创建新的 deviceCompliancePolicySettingStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bd0ab97129dda08db107e588c5c3103fbce2365
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975684"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="aaa3d-103">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="aaa3d-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="aaa3d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaa3d-105">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaa3d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="aaa3d-106">Prerequisites</span></span>
<span data-ttu-id="aaa3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaa3d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aaa3d-109">Permission type</span></span>|<span data-ttu-id="aaa3d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aaa3d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaa3d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aaa3d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aaa3d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaa3d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aaa3d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aaa3d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaa3d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-114">Not supported.</span></span>|
|<span data-ttu-id="aaa3d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aaa3d-115">Application</span></span>|<span data-ttu-id="aaa3d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaa3d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aaa3d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="aaa3d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="aaa3d-118">Request headers</span></span>
|<span data-ttu-id="aaa3d-119">标头</span><span class="sxs-lookup"><span data-stu-id="aaa3d-119">Header</span></span>|<span data-ttu-id="aaa3d-120">值</span><span class="sxs-lookup"><span data-stu-id="aaa3d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaa3d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaa3d-121">Authorization</span></span>|<span data-ttu-id="aaa3d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaa3d-123">接受</span><span class="sxs-lookup"><span data-stu-id="aaa3d-123">Accept</span></span>|<span data-ttu-id="aaa3d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aaa3d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaa3d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="aaa3d-125">Request body</span></span>
<span data-ttu-id="aaa3d-126">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="aaa3d-127">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="aaa3d-128">属性</span><span class="sxs-lookup"><span data-stu-id="aaa3d-128">Property</span></span>|<span data-ttu-id="aaa3d-129">类型</span><span class="sxs-lookup"><span data-stu-id="aaa3d-129">Type</span></span>|<span data-ttu-id="aaa3d-130">说明</span><span class="sxs-lookup"><span data-stu-id="aaa3d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaa3d-131">id</span><span class="sxs-lookup"><span data-stu-id="aaa3d-131">id</span></span>|<span data-ttu-id="aaa3d-132">String</span><span class="sxs-lookup"><span data-stu-id="aaa3d-132">String</span></span>|<span data-ttu-id="aaa3d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-133">Key of the entity.</span></span>|
|<span data-ttu-id="aaa3d-134">setting</span><span class="sxs-lookup"><span data-stu-id="aaa3d-134">setting</span></span>|<span data-ttu-id="aaa3d-135">String</span><span class="sxs-lookup"><span data-stu-id="aaa3d-135">String</span></span>|<span data-ttu-id="aaa3d-136">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="aaa3d-137">settingName</span><span class="sxs-lookup"><span data-stu-id="aaa3d-137">settingName</span></span>|<span data-ttu-id="aaa3d-138">String</span><span class="sxs-lookup"><span data-stu-id="aaa3d-138">String</span></span>|<span data-ttu-id="aaa3d-139">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-139">Name of the setting.</span></span>|
|<span data-ttu-id="aaa3d-140">platformType</span><span class="sxs-lookup"><span data-stu-id="aaa3d-140">platformType</span></span>|[<span data-ttu-id="aaa3d-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="aaa3d-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="aaa3d-142">设置平台。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-142">Setting platform.</span></span> <span data-ttu-id="aaa3d-143">可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="aaa3d-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaa3d-144">unknownDeviceCount</span></span>|<span data-ttu-id="aaa3d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa3d-145">Int32</span></span>|<span data-ttu-id="aaa3d-146">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaa3d-146">Number of unknown devices</span></span>|
|<span data-ttu-id="aaa3d-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaa3d-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="aaa3d-148">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa3d-148">Int32</span></span>|<span data-ttu-id="aaa3d-149">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaa3d-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="aaa3d-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaa3d-150">compliantDeviceCount</span></span>|<span data-ttu-id="aaa3d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa3d-151">Int32</span></span>|<span data-ttu-id="aaa3d-152">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaa3d-152">Number of compliant devices</span></span>|
|<span data-ttu-id="aaa3d-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaa3d-153">remediatedDeviceCount</span></span>|<span data-ttu-id="aaa3d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa3d-154">Int32</span></span>|<span data-ttu-id="aaa3d-155">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaa3d-155">Number of remediated devices</span></span>|
|<span data-ttu-id="aaa3d-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaa3d-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="aaa3d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa3d-157">Int32</span></span>|<span data-ttu-id="aaa3d-158">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaa3d-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="aaa3d-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaa3d-159">errorDeviceCount</span></span>|<span data-ttu-id="aaa3d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa3d-160">Int32</span></span>|<span data-ttu-id="aaa3d-161">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaa3d-161">Number of error devices</span></span>|
|<span data-ttu-id="aaa3d-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaa3d-162">conflictDeviceCount</span></span>|<span data-ttu-id="aaa3d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="aaa3d-163">Int32</span></span>|<span data-ttu-id="aaa3d-164">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaa3d-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="aaa3d-165">响应</span><span class="sxs-lookup"><span data-stu-id="aaa3d-165">Response</span></span>
<span data-ttu-id="aaa3d-166">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaa3d-167">示例</span><span class="sxs-lookup"><span data-stu-id="aaa3d-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaa3d-168">请求</span><span class="sxs-lookup"><span data-stu-id="aaa3d-168">Request</span></span>
<span data-ttu-id="aaa3d-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aaa3d-170">响应</span><span class="sxs-lookup"><span data-stu-id="aaa3d-170">Response</span></span>
<span data-ttu-id="aaa3d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aaa3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



