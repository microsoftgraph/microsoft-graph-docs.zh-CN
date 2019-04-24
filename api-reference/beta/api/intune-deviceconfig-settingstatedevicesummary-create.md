---
title: 创建 settingStateDeviceSummary
description: 创建新的 settingStateDeviceSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f42ee2fa96cb7b46054ed7605233e7b30ea9fed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518210"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="a635f-103">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a635f-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="a635f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a635f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a635f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a635f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a635f-106">创建新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a635f-106">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a635f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a635f-107">Prerequisites</span></span>
<span data-ttu-id="a635f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a635f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a635f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a635f-110">Permission type</span></span>|<span data-ttu-id="a635f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a635f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a635f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a635f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a635f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a635f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a635f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a635f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a635f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a635f-115">Not supported.</span></span>|
|<span data-ttu-id="a635f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a635f-116">Application</span></span>|<span data-ttu-id="a635f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a635f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a635f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a635f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a635f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a635f-119">Request headers</span></span>
|<span data-ttu-id="a635f-120">标头</span><span class="sxs-lookup"><span data-stu-id="a635f-120">Header</span></span>|<span data-ttu-id="a635f-121">值</span><span class="sxs-lookup"><span data-stu-id="a635f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a635f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a635f-122">Authorization</span></span>|<span data-ttu-id="a635f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a635f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a635f-124">接受</span><span class="sxs-lookup"><span data-stu-id="a635f-124">Accept</span></span>|<span data-ttu-id="a635f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a635f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a635f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a635f-126">Request body</span></span>
<span data-ttu-id="a635f-127">在请求正文中，提供 settingStateDeviceSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a635f-127">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="a635f-128">下表显示了创建 settingStateDeviceSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a635f-128">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="a635f-129">属性</span><span class="sxs-lookup"><span data-stu-id="a635f-129">Property</span></span>|<span data-ttu-id="a635f-130">类型</span><span class="sxs-lookup"><span data-stu-id="a635f-130">Type</span></span>|<span data-ttu-id="a635f-131">说明</span><span class="sxs-lookup"><span data-stu-id="a635f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a635f-132">id</span><span class="sxs-lookup"><span data-stu-id="a635f-132">id</span></span>|<span data-ttu-id="a635f-133">String</span><span class="sxs-lookup"><span data-stu-id="a635f-133">String</span></span>|<span data-ttu-id="a635f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a635f-134">Key of the entity.</span></span>|
|<span data-ttu-id="a635f-135">settingName</span><span class="sxs-lookup"><span data-stu-id="a635f-135">settingName</span></span>|<span data-ttu-id="a635f-136">字符串</span><span class="sxs-lookup"><span data-stu-id="a635f-136">String</span></span>|<span data-ttu-id="a635f-137">设置的名称</span><span class="sxs-lookup"><span data-stu-id="a635f-137">Name of the setting</span></span>|
|<span data-ttu-id="a635f-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="a635f-138">instancePath</span></span>|<span data-ttu-id="a635f-139">String</span><span class="sxs-lookup"><span data-stu-id="a635f-139">String</span></span>|<span data-ttu-id="a635f-140">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="a635f-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="a635f-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a635f-141">unknownDeviceCount</span></span>|<span data-ttu-id="a635f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a635f-142">Int32</span></span>|<span data-ttu-id="a635f-143">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="a635f-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="a635f-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a635f-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="a635f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a635f-145">Int32</span></span>|<span data-ttu-id="a635f-146">设置的设备不可用计数</span><span class="sxs-lookup"><span data-stu-id="a635f-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="a635f-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a635f-147">compliantDeviceCount</span></span>|<span data-ttu-id="a635f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a635f-148">Int32</span></span>|<span data-ttu-id="a635f-149">设置的设备符合计数</span><span class="sxs-lookup"><span data-stu-id="a635f-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a635f-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a635f-150">remediatedDeviceCount</span></span>|<span data-ttu-id="a635f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a635f-151">Int32</span></span>|<span data-ttu-id="a635f-152">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="a635f-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="a635f-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a635f-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a635f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a635f-154">Int32</span></span>|<span data-ttu-id="a635f-155">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="a635f-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="a635f-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a635f-156">errorDeviceCount</span></span>|<span data-ttu-id="a635f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a635f-157">Int32</span></span>|<span data-ttu-id="a635f-158">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="a635f-158">Device error count for the setting</span></span>|
|<span data-ttu-id="a635f-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a635f-159">conflictDeviceCount</span></span>|<span data-ttu-id="a635f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a635f-160">Int32</span></span>|<span data-ttu-id="a635f-161">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="a635f-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="a635f-162">响应</span><span class="sxs-lookup"><span data-stu-id="a635f-162">Response</span></span>
<span data-ttu-id="a635f-163">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a635f-163">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a635f-164">示例</span><span class="sxs-lookup"><span data-stu-id="a635f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="a635f-165">请求</span><span class="sxs-lookup"><span data-stu-id="a635f-165">Request</span></span>
<span data-ttu-id="a635f-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a635f-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a635f-167">响应</span><span class="sxs-lookup"><span data-stu-id="a635f-167">Response</span></span>
<span data-ttu-id="a635f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a635f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





