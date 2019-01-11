---
title: 更新 deviceConfigurationDeviceOverview
description: 更新 deviceConfigurationDeviceOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b91138cfd3a63a44cfe8b5cda502f165705fad7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863964"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="846f2-103">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="846f2-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="846f2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="846f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="846f2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="846f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="846f2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="846f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="846f2-107">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="846f2-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="846f2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="846f2-108">Prerequisites</span></span>
<span data-ttu-id="846f2-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="846f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="846f2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="846f2-111">Permission type</span></span>|<span data-ttu-id="846f2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="846f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="846f2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="846f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="846f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="846f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="846f2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="846f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="846f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="846f2-116">Not supported.</span></span>|
|<span data-ttu-id="846f2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="846f2-117">Application</span></span>|<span data-ttu-id="846f2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="846f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="846f2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="846f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="846f2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="846f2-120">Request headers</span></span>
|<span data-ttu-id="846f2-121">标头</span><span class="sxs-lookup"><span data-stu-id="846f2-121">Header</span></span>|<span data-ttu-id="846f2-122">值</span><span class="sxs-lookup"><span data-stu-id="846f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="846f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="846f2-123">Authorization</span></span>|<span data-ttu-id="846f2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="846f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="846f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="846f2-125">Accept</span></span>|<span data-ttu-id="846f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="846f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="846f2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="846f2-127">Request body</span></span>
<span data-ttu-id="846f2-128">在请求正文中，提供 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="846f2-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="846f2-129">下表显示创建 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="846f2-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="846f2-130">属性</span><span class="sxs-lookup"><span data-stu-id="846f2-130">Property</span></span>|<span data-ttu-id="846f2-131">类型</span><span class="sxs-lookup"><span data-stu-id="846f2-131">Type</span></span>|<span data-ttu-id="846f2-132">说明</span><span class="sxs-lookup"><span data-stu-id="846f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="846f2-133">id</span><span class="sxs-lookup"><span data-stu-id="846f2-133">id</span></span>|<span data-ttu-id="846f2-134">String</span><span class="sxs-lookup"><span data-stu-id="846f2-134">String</span></span>|<span data-ttu-id="846f2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="846f2-135">Key of the entity.</span></span>|
|<span data-ttu-id="846f2-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="846f2-136">pendingCount</span></span>|<span data-ttu-id="846f2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-137">Int32</span></span>|<span data-ttu-id="846f2-138">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="846f2-138">Number of pending devices</span></span>|
|<span data-ttu-id="846f2-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="846f2-139">notApplicableCount</span></span>|<span data-ttu-id="846f2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-140">Int32</span></span>|<span data-ttu-id="846f2-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="846f2-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="846f2-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="846f2-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="846f2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-143">Int32</span></span>|<span data-ttu-id="846f2-144">由于不匹配平台和策略不适用设备数</span><span class="sxs-lookup"><span data-stu-id="846f2-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="846f2-145">successCount</span><span class="sxs-lookup"><span data-stu-id="846f2-145">successCount</span></span>|<span data-ttu-id="846f2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-146">Int32</span></span>|<span data-ttu-id="846f2-147">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="846f2-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="846f2-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="846f2-148">errorCount</span></span>|<span data-ttu-id="846f2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-149">Int32</span></span>|<span data-ttu-id="846f2-150">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="846f2-150">Number of error devices</span></span>|
|<span data-ttu-id="846f2-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="846f2-151">failedCount</span></span>|<span data-ttu-id="846f2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-152">Int32</span></span>|<span data-ttu-id="846f2-153">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="846f2-153">Number of failed devices</span></span>|
|<span data-ttu-id="846f2-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="846f2-154">conflictCount</span></span>|<span data-ttu-id="846f2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-155">Int32</span></span>|<span data-ttu-id="846f2-156">存在冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="846f2-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="846f2-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="846f2-157">lastUpdateDateTime</span></span>|<span data-ttu-id="846f2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="846f2-158">DateTimeOffset</span></span>|<span data-ttu-id="846f2-159">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="846f2-159">Last update time</span></span>|
|<span data-ttu-id="846f2-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="846f2-160">configurationVersion</span></span>|<span data-ttu-id="846f2-161">Int32</span><span class="sxs-lookup"><span data-stu-id="846f2-161">Int32</span></span>|<span data-ttu-id="846f2-162">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="846f2-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="846f2-163">响应</span><span class="sxs-lookup"><span data-stu-id="846f2-163">Response</span></span>
<span data-ttu-id="846f2-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="846f2-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="846f2-165">示例</span><span class="sxs-lookup"><span data-stu-id="846f2-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="846f2-166">请求</span><span class="sxs-lookup"><span data-stu-id="846f2-166">Request</span></span>
<span data-ttu-id="846f2-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="846f2-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 273

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="846f2-168">响应</span><span class="sxs-lookup"><span data-stu-id="846f2-168">Response</span></span>
<span data-ttu-id="846f2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="846f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





