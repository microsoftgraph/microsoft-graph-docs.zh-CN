---
title: 更新 settingStateDeviceSummary
description: 更新 settingStateDeviceSummary 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f232069fac647bc45680f206ec41e7a8f218f7aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408731"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="63577-103">更新 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="63577-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="63577-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="63577-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63577-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63577-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63577-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63577-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63577-107">更新 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="63577-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63577-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="63577-108">Prerequisites</span></span>
<span data-ttu-id="63577-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="63577-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="63577-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63577-111">Permission type</span></span>|<span data-ttu-id="63577-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63577-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63577-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63577-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63577-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63577-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63577-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63577-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63577-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63577-116">Not supported.</span></span>|
|<span data-ttu-id="63577-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="63577-117">Application</span></span>|<span data-ttu-id="63577-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="63577-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63577-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63577-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="63577-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="63577-120">Request headers</span></span>
|<span data-ttu-id="63577-121">标头</span><span class="sxs-lookup"><span data-stu-id="63577-121">Header</span></span>|<span data-ttu-id="63577-122">值</span><span class="sxs-lookup"><span data-stu-id="63577-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63577-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63577-123">Authorization</span></span>|<span data-ttu-id="63577-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63577-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63577-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63577-125">Accept</span></span>|<span data-ttu-id="63577-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63577-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63577-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63577-127">Request body</span></span>
<span data-ttu-id="63577-128">在请求正文中，提供 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63577-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="63577-129">下表显示了创建 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63577-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="63577-130">属性</span><span class="sxs-lookup"><span data-stu-id="63577-130">Property</span></span>|<span data-ttu-id="63577-131">类型</span><span class="sxs-lookup"><span data-stu-id="63577-131">Type</span></span>|<span data-ttu-id="63577-132">说明</span><span class="sxs-lookup"><span data-stu-id="63577-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63577-133">id</span><span class="sxs-lookup"><span data-stu-id="63577-133">id</span></span>|<span data-ttu-id="63577-134">String</span><span class="sxs-lookup"><span data-stu-id="63577-134">String</span></span>|<span data-ttu-id="63577-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63577-135">Key of the entity.</span></span>|
|<span data-ttu-id="63577-136">settingName</span><span class="sxs-lookup"><span data-stu-id="63577-136">settingName</span></span>|<span data-ttu-id="63577-137">String</span><span class="sxs-lookup"><span data-stu-id="63577-137">String</span></span>|<span data-ttu-id="63577-138">设置的名称</span><span class="sxs-lookup"><span data-stu-id="63577-138">Name of the setting</span></span>|
|<span data-ttu-id="63577-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="63577-139">instancePath</span></span>|<span data-ttu-id="63577-140">String</span><span class="sxs-lookup"><span data-stu-id="63577-140">String</span></span>|<span data-ttu-id="63577-141">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="63577-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="63577-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63577-142">unknownDeviceCount</span></span>|<span data-ttu-id="63577-143">Int32</span><span class="sxs-lookup"><span data-stu-id="63577-143">Int32</span></span>|<span data-ttu-id="63577-144">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="63577-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="63577-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63577-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="63577-146">Int32</span><span class="sxs-lookup"><span data-stu-id="63577-146">Int32</span></span>|<span data-ttu-id="63577-147">设置的设备不适用计数</span><span class="sxs-lookup"><span data-stu-id="63577-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="63577-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63577-148">compliantDeviceCount</span></span>|<span data-ttu-id="63577-149">Int32</span><span class="sxs-lookup"><span data-stu-id="63577-149">Int32</span></span>|<span data-ttu-id="63577-150">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="63577-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="63577-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63577-151">remediatedDeviceCount</span></span>|<span data-ttu-id="63577-152">Int32</span><span class="sxs-lookup"><span data-stu-id="63577-152">Int32</span></span>|<span data-ttu-id="63577-153">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="63577-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="63577-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63577-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="63577-155">Int32</span><span class="sxs-lookup"><span data-stu-id="63577-155">Int32</span></span>|<span data-ttu-id="63577-156">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="63577-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="63577-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63577-157">errorDeviceCount</span></span>|<span data-ttu-id="63577-158">Int32</span><span class="sxs-lookup"><span data-stu-id="63577-158">Int32</span></span>|<span data-ttu-id="63577-159">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="63577-159">Device error count for the setting</span></span>|
|<span data-ttu-id="63577-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63577-160">conflictDeviceCount</span></span>|<span data-ttu-id="63577-161">Int32</span><span class="sxs-lookup"><span data-stu-id="63577-161">Int32</span></span>|<span data-ttu-id="63577-162">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="63577-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="63577-163">响应</span><span class="sxs-lookup"><span data-stu-id="63577-163">Response</span></span>
<span data-ttu-id="63577-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63577-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63577-165">示例</span><span class="sxs-lookup"><span data-stu-id="63577-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="63577-166">请求</span><span class="sxs-lookup"><span data-stu-id="63577-166">Request</span></span>
<span data-ttu-id="63577-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63577-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63577-168">响应</span><span class="sxs-lookup"><span data-stu-id="63577-168">Response</span></span>
<span data-ttu-id="63577-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63577-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




