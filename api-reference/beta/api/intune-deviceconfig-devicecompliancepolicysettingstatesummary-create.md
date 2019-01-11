---
title: 创建 deviceCompliancePolicySettingStateSummary
description: 创建新的 deviceCompliancePolicySettingStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f9f64cca9ca75ea8d823e7aa0adedad6d3527666
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832688"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="4d594-103">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="4d594-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="4d594-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4d594-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d594-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4d594-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d594-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4d594-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d594-107">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d594-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d594-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d594-108">Prerequisites</span></span>
<span data-ttu-id="4d594-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4d594-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d594-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d594-111">Permission type</span></span>|<span data-ttu-id="4d594-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d594-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d594-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d594-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d594-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d594-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d594-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d594-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d594-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d594-116">Not supported.</span></span>|
|<span data-ttu-id="4d594-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d594-117">Application</span></span>|<span data-ttu-id="4d594-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d594-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d594-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d594-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4d594-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d594-120">Request headers</span></span>
|<span data-ttu-id="4d594-121">标头</span><span class="sxs-lookup"><span data-stu-id="4d594-121">Header</span></span>|<span data-ttu-id="4d594-122">值</span><span class="sxs-lookup"><span data-stu-id="4d594-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d594-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d594-123">Authorization</span></span>|<span data-ttu-id="4d594-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d594-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d594-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4d594-125">Accept</span></span>|<span data-ttu-id="4d594-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d594-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d594-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d594-127">Request body</span></span>
<span data-ttu-id="4d594-128">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d594-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="4d594-129">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d594-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="4d594-130">属性</span><span class="sxs-lookup"><span data-stu-id="4d594-130">Property</span></span>|<span data-ttu-id="4d594-131">类型</span><span class="sxs-lookup"><span data-stu-id="4d594-131">Type</span></span>|<span data-ttu-id="4d594-132">说明</span><span class="sxs-lookup"><span data-stu-id="4d594-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d594-133">id</span><span class="sxs-lookup"><span data-stu-id="4d594-133">id</span></span>|<span data-ttu-id="4d594-134">String</span><span class="sxs-lookup"><span data-stu-id="4d594-134">String</span></span>|<span data-ttu-id="4d594-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d594-135">Key of the entity.</span></span>|
|<span data-ttu-id="4d594-136">setting</span><span class="sxs-lookup"><span data-stu-id="4d594-136">setting</span></span>|<span data-ttu-id="4d594-137">String</span><span class="sxs-lookup"><span data-stu-id="4d594-137">String</span></span>|<span data-ttu-id="4d594-138">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="4d594-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="4d594-139">settingName</span><span class="sxs-lookup"><span data-stu-id="4d594-139">settingName</span></span>|<span data-ttu-id="4d594-140">String</span><span class="sxs-lookup"><span data-stu-id="4d594-140">String</span></span>|<span data-ttu-id="4d594-141">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="4d594-141">Name of the setting.</span></span>|
|<span data-ttu-id="4d594-142">platformType</span><span class="sxs-lookup"><span data-stu-id="4d594-142">platformType</span></span>|[<span data-ttu-id="4d594-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="4d594-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="4d594-144">设置平台。</span><span class="sxs-lookup"><span data-stu-id="4d594-144">Setting platform.</span></span> <span data-ttu-id="4d594-145">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="4d594-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="4d594-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d594-146">unknownDeviceCount</span></span>|<span data-ttu-id="4d594-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4d594-147">Int32</span></span>|<span data-ttu-id="4d594-148">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d594-148">Number of unknown devices</span></span>|
|<span data-ttu-id="4d594-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d594-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="4d594-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4d594-150">Int32</span></span>|<span data-ttu-id="4d594-151">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d594-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="4d594-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d594-152">compliantDeviceCount</span></span>|<span data-ttu-id="4d594-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4d594-153">Int32</span></span>|<span data-ttu-id="4d594-154">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d594-154">Number of compliant devices</span></span>|
|<span data-ttu-id="4d594-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d594-155">remediatedDeviceCount</span></span>|<span data-ttu-id="4d594-156">Int32</span><span class="sxs-lookup"><span data-stu-id="4d594-156">Int32</span></span>|<span data-ttu-id="4d594-157">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d594-157">Number of remediated devices</span></span>|
|<span data-ttu-id="4d594-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d594-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4d594-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4d594-159">Int32</span></span>|<span data-ttu-id="4d594-160">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d594-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="4d594-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d594-161">errorDeviceCount</span></span>|<span data-ttu-id="4d594-162">Int32</span><span class="sxs-lookup"><span data-stu-id="4d594-162">Int32</span></span>|<span data-ttu-id="4d594-163">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d594-163">Number of error devices</span></span>|
|<span data-ttu-id="4d594-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4d594-164">conflictDeviceCount</span></span>|<span data-ttu-id="4d594-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4d594-165">Int32</span></span>|<span data-ttu-id="4d594-166">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="4d594-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="4d594-167">响应</span><span class="sxs-lookup"><span data-stu-id="4d594-167">Response</span></span>
<span data-ttu-id="4d594-168">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d594-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d594-169">示例</span><span class="sxs-lookup"><span data-stu-id="4d594-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d594-170">请求</span><span class="sxs-lookup"><span data-stu-id="4d594-170">Request</span></span>
<span data-ttu-id="4d594-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d594-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d594-172">响应</span><span class="sxs-lookup"><span data-stu-id="4d594-172">Response</span></span>
<span data-ttu-id="4d594-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d594-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





