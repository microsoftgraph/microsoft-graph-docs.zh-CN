---
title: 更新 settingStateDeviceSummary
description: 更新 settingStateDeviceSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 951b76545e7c11f2a17ad9f787d898e77b3023d9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792644"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="edbaa-103">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="edbaa-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="edbaa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edbaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edbaa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edbaa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edbaa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edbaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edbaa-107">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="edbaa-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edbaa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="edbaa-108">Prerequisites</span></span>
<span data-ttu-id="edbaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edbaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edbaa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="edbaa-111">Permission type</span></span>|<span data-ttu-id="edbaa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="edbaa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edbaa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edbaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edbaa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbaa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="edbaa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edbaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edbaa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="edbaa-116">Not supported.</span></span>|
|<span data-ttu-id="edbaa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="edbaa-117">Application</span></span>|<span data-ttu-id="edbaa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbaa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edbaa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edbaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="edbaa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="edbaa-120">Request headers</span></span>
|<span data-ttu-id="edbaa-121">标头</span><span class="sxs-lookup"><span data-stu-id="edbaa-121">Header</span></span>|<span data-ttu-id="edbaa-122">值</span><span class="sxs-lookup"><span data-stu-id="edbaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edbaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edbaa-123">Authorization</span></span>|<span data-ttu-id="edbaa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="edbaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edbaa-125">接受</span><span class="sxs-lookup"><span data-stu-id="edbaa-125">Accept</span></span>|<span data-ttu-id="edbaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edbaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edbaa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="edbaa-127">Request body</span></span>
<span data-ttu-id="edbaa-128">在请求正文中，提供 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edbaa-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="edbaa-129">下表显示了创建 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="edbaa-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="edbaa-130">属性</span><span class="sxs-lookup"><span data-stu-id="edbaa-130">Property</span></span>|<span data-ttu-id="edbaa-131">类型</span><span class="sxs-lookup"><span data-stu-id="edbaa-131">Type</span></span>|<span data-ttu-id="edbaa-132">说明</span><span class="sxs-lookup"><span data-stu-id="edbaa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edbaa-133">id</span><span class="sxs-lookup"><span data-stu-id="edbaa-133">id</span></span>|<span data-ttu-id="edbaa-134">String</span><span class="sxs-lookup"><span data-stu-id="edbaa-134">String</span></span>|<span data-ttu-id="edbaa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="edbaa-135">Key of the entity.</span></span>|
|<span data-ttu-id="edbaa-136">settingName</span><span class="sxs-lookup"><span data-stu-id="edbaa-136">settingName</span></span>|<span data-ttu-id="edbaa-137">String</span><span class="sxs-lookup"><span data-stu-id="edbaa-137">String</span></span>|<span data-ttu-id="edbaa-138">设置的名称</span><span class="sxs-lookup"><span data-stu-id="edbaa-138">Name of the setting</span></span>|
|<span data-ttu-id="edbaa-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="edbaa-139">instancePath</span></span>|<span data-ttu-id="edbaa-140">String</span><span class="sxs-lookup"><span data-stu-id="edbaa-140">String</span></span>|<span data-ttu-id="edbaa-141">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="edbaa-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="edbaa-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="edbaa-142">unknownDeviceCount</span></span>|<span data-ttu-id="edbaa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="edbaa-143">Int32</span></span>|<span data-ttu-id="edbaa-144">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="edbaa-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="edbaa-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="edbaa-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="edbaa-146">Int32</span><span class="sxs-lookup"><span data-stu-id="edbaa-146">Int32</span></span>|<span data-ttu-id="edbaa-147">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="edbaa-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="edbaa-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="edbaa-148">compliantDeviceCount</span></span>|<span data-ttu-id="edbaa-149">Int32</span><span class="sxs-lookup"><span data-stu-id="edbaa-149">Int32</span></span>|<span data-ttu-id="edbaa-150">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="edbaa-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="edbaa-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="edbaa-151">remediatedDeviceCount</span></span>|<span data-ttu-id="edbaa-152">Int32</span><span class="sxs-lookup"><span data-stu-id="edbaa-152">Int32</span></span>|<span data-ttu-id="edbaa-153">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="edbaa-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="edbaa-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="edbaa-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="edbaa-155">Int32</span><span class="sxs-lookup"><span data-stu-id="edbaa-155">Int32</span></span>|<span data-ttu-id="edbaa-156">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="edbaa-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="edbaa-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="edbaa-157">errorDeviceCount</span></span>|<span data-ttu-id="edbaa-158">Int32</span><span class="sxs-lookup"><span data-stu-id="edbaa-158">Int32</span></span>|<span data-ttu-id="edbaa-159">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="edbaa-159">Device error count for the setting</span></span>|
|<span data-ttu-id="edbaa-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="edbaa-160">conflictDeviceCount</span></span>|<span data-ttu-id="edbaa-161">Int32</span><span class="sxs-lookup"><span data-stu-id="edbaa-161">Int32</span></span>|<span data-ttu-id="edbaa-162">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="edbaa-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="edbaa-163">响应</span><span class="sxs-lookup"><span data-stu-id="edbaa-163">Response</span></span>
<span data-ttu-id="edbaa-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edbaa-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edbaa-165">示例</span><span class="sxs-lookup"><span data-stu-id="edbaa-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="edbaa-166">请求</span><span class="sxs-lookup"><span data-stu-id="edbaa-166">Request</span></span>
<span data-ttu-id="edbaa-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="edbaa-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
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

### <a name="response"></a><span data-ttu-id="edbaa-168">响应</span><span class="sxs-lookup"><span data-stu-id="edbaa-168">Response</span></span>
<span data-ttu-id="edbaa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="edbaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



