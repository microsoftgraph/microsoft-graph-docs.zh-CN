---
title: 更新 deviceConfigurationDeviceOverview
description: 更新 deviceConfigurationDeviceOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73ab98258b40129c9ef64776a0c775b74bd64eb2
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792959"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="7336f-103">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7336f-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="7336f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7336f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7336f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7336f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7336f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7336f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7336f-107">更新 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7336f-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7336f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7336f-108">Prerequisites</span></span>
<span data-ttu-id="7336f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7336f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7336f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7336f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7336f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7336f-111">Permission type</span></span>|<span data-ttu-id="7336f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7336f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7336f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7336f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7336f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7336f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7336f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7336f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7336f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7336f-116">Not supported.</span></span>|
|<span data-ttu-id="7336f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7336f-117">Application</span></span>|<span data-ttu-id="7336f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7336f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7336f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7336f-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="7336f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7336f-120">Request headers</span></span>
|<span data-ttu-id="7336f-121">标头</span><span class="sxs-lookup"><span data-stu-id="7336f-121">Header</span></span>|<span data-ttu-id="7336f-122">值</span><span class="sxs-lookup"><span data-stu-id="7336f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7336f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7336f-123">Authorization</span></span>|<span data-ttu-id="7336f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7336f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7336f-125">接受</span><span class="sxs-lookup"><span data-stu-id="7336f-125">Accept</span></span>|<span data-ttu-id="7336f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7336f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7336f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7336f-127">Request body</span></span>
<span data-ttu-id="7336f-128">在请求正文中，提供 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7336f-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="7336f-129">下表显示创建 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7336f-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="7336f-130">属性</span><span class="sxs-lookup"><span data-stu-id="7336f-130">Property</span></span>|<span data-ttu-id="7336f-131">类型</span><span class="sxs-lookup"><span data-stu-id="7336f-131">Type</span></span>|<span data-ttu-id="7336f-132">说明</span><span class="sxs-lookup"><span data-stu-id="7336f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7336f-133">id</span><span class="sxs-lookup"><span data-stu-id="7336f-133">id</span></span>|<span data-ttu-id="7336f-134">String</span><span class="sxs-lookup"><span data-stu-id="7336f-134">String</span></span>|<span data-ttu-id="7336f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7336f-135">Key of the entity.</span></span>|
|<span data-ttu-id="7336f-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="7336f-136">pendingCount</span></span>|<span data-ttu-id="7336f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-137">Int32</span></span>|<span data-ttu-id="7336f-138">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="7336f-138">Number of pending devices</span></span>|
|<span data-ttu-id="7336f-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7336f-139">notApplicableCount</span></span>|<span data-ttu-id="7336f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-140">Int32</span></span>|<span data-ttu-id="7336f-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="7336f-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="7336f-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="7336f-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="7336f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-143">Int32</span></span>|<span data-ttu-id="7336f-144">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="7336f-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="7336f-145">successCount</span><span class="sxs-lookup"><span data-stu-id="7336f-145">successCount</span></span>|<span data-ttu-id="7336f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-146">Int32</span></span>|<span data-ttu-id="7336f-147">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="7336f-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="7336f-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="7336f-148">errorCount</span></span>|<span data-ttu-id="7336f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-149">Int32</span></span>|<span data-ttu-id="7336f-150">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="7336f-150">Number of error devices</span></span>|
|<span data-ttu-id="7336f-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="7336f-151">failedCount</span></span>|<span data-ttu-id="7336f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-152">Int32</span></span>|<span data-ttu-id="7336f-153">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="7336f-153">Number of failed devices</span></span>|
|<span data-ttu-id="7336f-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="7336f-154">conflictCount</span></span>|<span data-ttu-id="7336f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-155">Int32</span></span>|<span data-ttu-id="7336f-156">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="7336f-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="7336f-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="7336f-157">lastUpdateDateTime</span></span>|<span data-ttu-id="7336f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7336f-158">DateTimeOffset</span></span>|<span data-ttu-id="7336f-159">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="7336f-159">Last update time</span></span>|
|<span data-ttu-id="7336f-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="7336f-160">configurationVersion</span></span>|<span data-ttu-id="7336f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="7336f-161">Int32</span></span>|<span data-ttu-id="7336f-162">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="7336f-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="7336f-163">响应</span><span class="sxs-lookup"><span data-stu-id="7336f-163">Response</span></span>
<span data-ttu-id="7336f-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7336f-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7336f-165">示例</span><span class="sxs-lookup"><span data-stu-id="7336f-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="7336f-166">请求</span><span class="sxs-lookup"><span data-stu-id="7336f-166">Request</span></span>
<span data-ttu-id="7336f-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7336f-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
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

### <a name="response"></a><span data-ttu-id="7336f-168">响应</span><span class="sxs-lookup"><span data-stu-id="7336f-168">Response</span></span>
<span data-ttu-id="7336f-169">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7336f-169">Here is an example of the response.</span></span> <span data-ttu-id="7336f-170">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7336f-170">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7336f-171">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7336f-171">All of the properties will be returned from an actual call.</span></span>
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



