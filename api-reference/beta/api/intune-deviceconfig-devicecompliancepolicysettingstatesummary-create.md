---
title: 创建 deviceCompliancePolicySettingStateSummary
description: 创建新的 deviceCompliancePolicySettingStateSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b7abdece5f85eb5d93dddd5eb19237ffcedba40
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666448"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="0b296-103">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="0b296-103">Create deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="0b296-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b296-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b296-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b296-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b296-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b296-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b296-107">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b296-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b296-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b296-108">Prerequisites</span></span>
<span data-ttu-id="0b296-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b296-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b296-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b296-111">Permission type</span></span>|<span data-ttu-id="0b296-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b296-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b296-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b296-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b296-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b296-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b296-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b296-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b296-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b296-116">Not supported.</span></span>|
|<span data-ttu-id="0b296-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b296-117">Application</span></span>|<span data-ttu-id="0b296-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b296-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b296-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b296-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="0b296-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b296-120">Request headers</span></span>
|<span data-ttu-id="0b296-121">标头</span><span class="sxs-lookup"><span data-stu-id="0b296-121">Header</span></span>|<span data-ttu-id="0b296-122">值</span><span class="sxs-lookup"><span data-stu-id="0b296-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b296-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b296-123">Authorization</span></span>|<span data-ttu-id="0b296-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b296-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b296-125">接受</span><span class="sxs-lookup"><span data-stu-id="0b296-125">Accept</span></span>|<span data-ttu-id="0b296-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b296-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b296-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b296-127">Request body</span></span>
<span data-ttu-id="0b296-128">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b296-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="0b296-129">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b296-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="0b296-130">属性</span><span class="sxs-lookup"><span data-stu-id="0b296-130">Property</span></span>|<span data-ttu-id="0b296-131">类型</span><span class="sxs-lookup"><span data-stu-id="0b296-131">Type</span></span>|<span data-ttu-id="0b296-132">说明</span><span class="sxs-lookup"><span data-stu-id="0b296-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b296-133">id</span><span class="sxs-lookup"><span data-stu-id="0b296-133">id</span></span>|<span data-ttu-id="0b296-134">String</span><span class="sxs-lookup"><span data-stu-id="0b296-134">String</span></span>|<span data-ttu-id="0b296-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b296-135">Key of the entity.</span></span>|
|<span data-ttu-id="0b296-136">setting</span><span class="sxs-lookup"><span data-stu-id="0b296-136">setting</span></span>|<span data-ttu-id="0b296-137">String</span><span class="sxs-lookup"><span data-stu-id="0b296-137">String</span></span>|<span data-ttu-id="0b296-138">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="0b296-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="0b296-139">settingName</span><span class="sxs-lookup"><span data-stu-id="0b296-139">settingName</span></span>|<span data-ttu-id="0b296-140">String</span><span class="sxs-lookup"><span data-stu-id="0b296-140">String</span></span>|<span data-ttu-id="0b296-141">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="0b296-141">Name of the setting.</span></span>|
|<span data-ttu-id="0b296-142">platformType</span><span class="sxs-lookup"><span data-stu-id="0b296-142">platformType</span></span>|[<span data-ttu-id="0b296-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0b296-143">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="0b296-144">设置平台。</span><span class="sxs-lookup"><span data-stu-id="0b296-144">Setting platform.</span></span> <span data-ttu-id="0b296-145">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`androidAOSP`、`all`。</span><span class="sxs-lookup"><span data-stu-id="0b296-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `androidAOSP`, `all`.</span></span>|
|<span data-ttu-id="0b296-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b296-146">unknownDeviceCount</span></span>|<span data-ttu-id="0b296-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0b296-147">Int32</span></span>|<span data-ttu-id="0b296-148">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="0b296-148">Number of unknown devices</span></span>|
|<span data-ttu-id="0b296-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b296-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="0b296-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0b296-150">Int32</span></span>|<span data-ttu-id="0b296-151">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="0b296-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="0b296-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b296-152">compliantDeviceCount</span></span>|<span data-ttu-id="0b296-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0b296-153">Int32</span></span>|<span data-ttu-id="0b296-154">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="0b296-154">Number of compliant devices</span></span>|
|<span data-ttu-id="0b296-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b296-155">remediatedDeviceCount</span></span>|<span data-ttu-id="0b296-156">Int32</span><span class="sxs-lookup"><span data-stu-id="0b296-156">Int32</span></span>|<span data-ttu-id="0b296-157">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="0b296-157">Number of remediated devices</span></span>|
|<span data-ttu-id="0b296-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b296-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0b296-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0b296-159">Int32</span></span>|<span data-ttu-id="0b296-160">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="0b296-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="0b296-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b296-161">errorDeviceCount</span></span>|<span data-ttu-id="0b296-162">Int32</span><span class="sxs-lookup"><span data-stu-id="0b296-162">Int32</span></span>|<span data-ttu-id="0b296-163">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="0b296-163">Number of error devices</span></span>|
|<span data-ttu-id="0b296-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b296-164">conflictDeviceCount</span></span>|<span data-ttu-id="0b296-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0b296-165">Int32</span></span>|<span data-ttu-id="0b296-166">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="0b296-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="0b296-167">响应</span><span class="sxs-lookup"><span data-stu-id="0b296-167">Response</span></span>
<span data-ttu-id="0b296-168">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b296-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b296-169">示例</span><span class="sxs-lookup"><span data-stu-id="0b296-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b296-170">请求</span><span class="sxs-lookup"><span data-stu-id="0b296-170">Request</span></span>
<span data-ttu-id="0b296-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b296-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b296-172">响应</span><span class="sxs-lookup"><span data-stu-id="0b296-172">Response</span></span>
<span data-ttu-id="0b296-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b296-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




