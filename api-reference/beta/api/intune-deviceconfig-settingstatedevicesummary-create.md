---
title: 创建 settingStateDeviceSummary
description: 创建新的 settingStateDeviceSummary 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df407dbcf131dfa2ab61fc3599878babf3ca33b8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976342"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="7b2a1-103">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7b2a1-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="7b2a1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b2a1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b2a1-106">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-106">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b2a1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b2a1-107">Prerequisites</span></span>
<span data-ttu-id="7b2a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b2a1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b2a1-110">Permission type</span></span>|<span data-ttu-id="7b2a1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b2a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b2a1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b2a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b2a1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b2a1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b2a1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b2a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b2a1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-115">Not supported.</span></span>|
|<span data-ttu-id="7b2a1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b2a1-116">Application</span></span>|<span data-ttu-id="7b2a1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b2a1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b2a1-118">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7b2a1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b2a1-119">Request headers</span></span>
|<span data-ttu-id="7b2a1-120">标头</span><span class="sxs-lookup"><span data-stu-id="7b2a1-120">Header</span></span>|<span data-ttu-id="7b2a1-121">值</span><span class="sxs-lookup"><span data-stu-id="7b2a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b2a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b2a1-122">Authorization</span></span>|<span data-ttu-id="7b2a1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b2a1-124">接受</span><span class="sxs-lookup"><span data-stu-id="7b2a1-124">Accept</span></span>|<span data-ttu-id="7b2a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b2a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b2a1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b2a1-126">Request body</span></span>
<span data-ttu-id="7b2a1-127">在请求正文中，提供 settingStateDeviceSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-127">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="7b2a1-128">下表显示了创建 settingStateDeviceSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-128">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="7b2a1-129">属性</span><span class="sxs-lookup"><span data-stu-id="7b2a1-129">Property</span></span>|<span data-ttu-id="7b2a1-130">类型</span><span class="sxs-lookup"><span data-stu-id="7b2a1-130">Type</span></span>|<span data-ttu-id="7b2a1-131">说明</span><span class="sxs-lookup"><span data-stu-id="7b2a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b2a1-132">id</span><span class="sxs-lookup"><span data-stu-id="7b2a1-132">id</span></span>|<span data-ttu-id="7b2a1-133">String</span><span class="sxs-lookup"><span data-stu-id="7b2a1-133">String</span></span>|<span data-ttu-id="7b2a1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-134">Key of the entity.</span></span>|
|<span data-ttu-id="7b2a1-135">settingName</span><span class="sxs-lookup"><span data-stu-id="7b2a1-135">settingName</span></span>|<span data-ttu-id="7b2a1-136">String</span><span class="sxs-lookup"><span data-stu-id="7b2a1-136">String</span></span>|<span data-ttu-id="7b2a1-137">设置的名称</span><span class="sxs-lookup"><span data-stu-id="7b2a1-137">Name of the setting</span></span>|
|<span data-ttu-id="7b2a1-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="7b2a1-138">instancePath</span></span>|<span data-ttu-id="7b2a1-139">String</span><span class="sxs-lookup"><span data-stu-id="7b2a1-139">String</span></span>|<span data-ttu-id="7b2a1-140">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="7b2a1-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="7b2a1-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b2a1-141">unknownDeviceCount</span></span>|<span data-ttu-id="7b2a1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2a1-142">Int32</span></span>|<span data-ttu-id="7b2a1-143">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="7b2a1-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="7b2a1-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b2a1-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="7b2a1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2a1-145">Int32</span></span>|<span data-ttu-id="7b2a1-146">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="7b2a1-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="7b2a1-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b2a1-147">compliantDeviceCount</span></span>|<span data-ttu-id="7b2a1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2a1-148">Int32</span></span>|<span data-ttu-id="7b2a1-149">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="7b2a1-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="7b2a1-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b2a1-150">remediatedDeviceCount</span></span>|<span data-ttu-id="7b2a1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2a1-151">Int32</span></span>|<span data-ttu-id="7b2a1-152">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="7b2a1-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="7b2a1-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b2a1-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7b2a1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2a1-154">Int32</span></span>|<span data-ttu-id="7b2a1-155">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="7b2a1-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="7b2a1-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b2a1-156">errorDeviceCount</span></span>|<span data-ttu-id="7b2a1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2a1-157">Int32</span></span>|<span data-ttu-id="7b2a1-158">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="7b2a1-158">Device error count for the setting</span></span>|
|<span data-ttu-id="7b2a1-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b2a1-159">conflictDeviceCount</span></span>|<span data-ttu-id="7b2a1-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7b2a1-160">Int32</span></span>|<span data-ttu-id="7b2a1-161">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="7b2a1-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="7b2a1-162">响应</span><span class="sxs-lookup"><span data-stu-id="7b2a1-162">Response</span></span>
<span data-ttu-id="7b2a1-163">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-163">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b2a1-164">示例</span><span class="sxs-lookup"><span data-stu-id="7b2a1-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b2a1-165">请求</span><span class="sxs-lookup"><span data-stu-id="7b2a1-165">Request</span></span>
<span data-ttu-id="7b2a1-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b2a1-167">响应</span><span class="sxs-lookup"><span data-stu-id="7b2a1-167">Response</span></span>
<span data-ttu-id="7b2a1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b2a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





