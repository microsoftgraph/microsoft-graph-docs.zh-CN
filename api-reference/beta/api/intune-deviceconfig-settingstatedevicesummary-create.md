---
title: 创建 settingStateDeviceSummary
description: 创建新的 settingStateDeviceSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cac52b58876bf1943462e370aefbab0699615319
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792672"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="e6c16-103">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e6c16-103">Create settingStateDeviceSummary</span></span>

<span data-ttu-id="e6c16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6c16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6c16-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6c16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6c16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6c16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6c16-107">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6c16-107">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6c16-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6c16-108">Prerequisites</span></span>
<span data-ttu-id="e6c16-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e6c16-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e6c16-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6c16-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c16-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6c16-111">Permission type</span></span>|<span data-ttu-id="e6c16-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6c16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6c16-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6c16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6c16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6c16-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6c16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6c16-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6c16-116">Not supported.</span></span>|
|<span data-ttu-id="e6c16-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6c16-117">Application</span></span>|<span data-ttu-id="e6c16-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c16-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6c16-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6c16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e6c16-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6c16-120">Request headers</span></span>
|<span data-ttu-id="e6c16-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6c16-121">Header</span></span>|<span data-ttu-id="e6c16-122">值</span><span class="sxs-lookup"><span data-stu-id="e6c16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6c16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6c16-123">Authorization</span></span>|<span data-ttu-id="e6c16-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6c16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6c16-125">接受</span><span class="sxs-lookup"><span data-stu-id="e6c16-125">Accept</span></span>|<span data-ttu-id="e6c16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6c16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6c16-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6c16-127">Request body</span></span>
<span data-ttu-id="e6c16-128">在请求正文中，提供 settingStateDeviceSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6c16-128">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="e6c16-129">下表显示了创建 settingStateDeviceSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6c16-129">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="e6c16-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6c16-130">Property</span></span>|<span data-ttu-id="e6c16-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6c16-131">Type</span></span>|<span data-ttu-id="e6c16-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6c16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6c16-133">id</span><span class="sxs-lookup"><span data-stu-id="e6c16-133">id</span></span>|<span data-ttu-id="e6c16-134">String</span><span class="sxs-lookup"><span data-stu-id="e6c16-134">String</span></span>|<span data-ttu-id="e6c16-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6c16-135">Key of the entity.</span></span>|
|<span data-ttu-id="e6c16-136">settingName</span><span class="sxs-lookup"><span data-stu-id="e6c16-136">settingName</span></span>|<span data-ttu-id="e6c16-137">String</span><span class="sxs-lookup"><span data-stu-id="e6c16-137">String</span></span>|<span data-ttu-id="e6c16-138">设置的名称</span><span class="sxs-lookup"><span data-stu-id="e6c16-138">Name of the setting</span></span>|
|<span data-ttu-id="e6c16-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="e6c16-139">instancePath</span></span>|<span data-ttu-id="e6c16-140">String</span><span class="sxs-lookup"><span data-stu-id="e6c16-140">String</span></span>|<span data-ttu-id="e6c16-141">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="e6c16-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="e6c16-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6c16-142">unknownDeviceCount</span></span>|<span data-ttu-id="e6c16-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c16-143">Int32</span></span>|<span data-ttu-id="e6c16-144">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="e6c16-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="e6c16-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6c16-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="e6c16-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c16-146">Int32</span></span>|<span data-ttu-id="e6c16-147">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="e6c16-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="e6c16-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6c16-148">compliantDeviceCount</span></span>|<span data-ttu-id="e6c16-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c16-149">Int32</span></span>|<span data-ttu-id="e6c16-150">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="e6c16-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="e6c16-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6c16-151">remediatedDeviceCount</span></span>|<span data-ttu-id="e6c16-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c16-152">Int32</span></span>|<span data-ttu-id="e6c16-153">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="e6c16-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="e6c16-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6c16-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e6c16-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c16-155">Int32</span></span>|<span data-ttu-id="e6c16-156">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="e6c16-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="e6c16-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6c16-157">errorDeviceCount</span></span>|<span data-ttu-id="e6c16-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c16-158">Int32</span></span>|<span data-ttu-id="e6c16-159">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="e6c16-159">Device error count for the setting</span></span>|
|<span data-ttu-id="e6c16-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6c16-160">conflictDeviceCount</span></span>|<span data-ttu-id="e6c16-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e6c16-161">Int32</span></span>|<span data-ttu-id="e6c16-162">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="e6c16-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="e6c16-163">响应</span><span class="sxs-lookup"><span data-stu-id="e6c16-163">Response</span></span>
<span data-ttu-id="e6c16-164">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6c16-164">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6c16-165">示例</span><span class="sxs-lookup"><span data-stu-id="e6c16-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6c16-166">请求</span><span class="sxs-lookup"><span data-stu-id="e6c16-166">Request</span></span>
<span data-ttu-id="e6c16-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6c16-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="e6c16-168">响应</span><span class="sxs-lookup"><span data-stu-id="e6c16-168">Response</span></span>
<span data-ttu-id="e6c16-169">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e6c16-169">Here is an example of the response.</span></span> <span data-ttu-id="e6c16-170">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e6c16-170">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e6c16-171">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e6c16-171">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



