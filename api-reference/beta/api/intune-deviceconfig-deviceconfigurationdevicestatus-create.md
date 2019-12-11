---
title: 创建 deviceConfigurationDeviceStatus
description: 创建新的 deviceConfigurationDeviceStatus 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 225834ff8d6c752cf916b82b508fe1d2442f3a4f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949390"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="90671-103">创建 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="90671-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="90671-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90671-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90671-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90671-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90671-106">创建新的 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90671-106">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90671-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="90671-107">Prerequisites</span></span>
<span data-ttu-id="90671-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90671-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="90671-110">Permission type</span></span>|<span data-ttu-id="90671-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90671-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90671-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90671-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90671-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90671-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90671-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90671-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90671-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90671-115">Not supported.</span></span>|
|<span data-ttu-id="90671-116">Application</span><span class="sxs-lookup"><span data-stu-id="90671-116">Application</span></span>|<span data-ttu-id="90671-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90671-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90671-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90671-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="90671-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="90671-119">Request headers</span></span>
|<span data-ttu-id="90671-120">标头</span><span class="sxs-lookup"><span data-stu-id="90671-120">Header</span></span>|<span data-ttu-id="90671-121">值</span><span class="sxs-lookup"><span data-stu-id="90671-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90671-122">授权</span><span class="sxs-lookup"><span data-stu-id="90671-122">Authorization</span></span>|<span data-ttu-id="90671-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90671-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90671-124">接受</span><span class="sxs-lookup"><span data-stu-id="90671-124">Accept</span></span>|<span data-ttu-id="90671-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90671-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90671-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90671-126">Request body</span></span>
<span data-ttu-id="90671-127">在请求正文中，提供 deviceConfigurationDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90671-127">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="90671-128">下表显示创建 deviceConfigurationDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90671-128">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="90671-129">属性</span><span class="sxs-lookup"><span data-stu-id="90671-129">Property</span></span>|<span data-ttu-id="90671-130">类型</span><span class="sxs-lookup"><span data-stu-id="90671-130">Type</span></span>|<span data-ttu-id="90671-131">说明</span><span class="sxs-lookup"><span data-stu-id="90671-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90671-132">id</span><span class="sxs-lookup"><span data-stu-id="90671-132">id</span></span>|<span data-ttu-id="90671-133">String</span><span class="sxs-lookup"><span data-stu-id="90671-133">String</span></span>|<span data-ttu-id="90671-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="90671-134">Key of the entity.</span></span>|
|<span data-ttu-id="90671-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="90671-135">deviceDisplayName</span></span>|<span data-ttu-id="90671-136">字符串</span><span class="sxs-lookup"><span data-stu-id="90671-136">String</span></span>|<span data-ttu-id="90671-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="90671-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="90671-138">userName</span><span class="sxs-lookup"><span data-stu-id="90671-138">userName</span></span>|<span data-ttu-id="90671-139">字符串</span><span class="sxs-lookup"><span data-stu-id="90671-139">String</span></span>|<span data-ttu-id="90671-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="90671-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="90671-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="90671-141">deviceModel</span></span>|<span data-ttu-id="90671-142">String</span><span class="sxs-lookup"><span data-stu-id="90671-142">String</span></span>|<span data-ttu-id="90671-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="90671-143">The device model that is being reported</span></span>|
|<span data-ttu-id="90671-144">platform</span><span class="sxs-lookup"><span data-stu-id="90671-144">platform</span></span>|<span data-ttu-id="90671-145">Int32</span><span class="sxs-lookup"><span data-stu-id="90671-145">Int32</span></span>|<span data-ttu-id="90671-146">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="90671-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="90671-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="90671-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="90671-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90671-148">DateTimeOffset</span></span>|<span data-ttu-id="90671-149">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="90671-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="90671-150">status</span><span class="sxs-lookup"><span data-stu-id="90671-150">status</span></span>|[<span data-ttu-id="90671-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="90671-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="90671-152">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="90671-152">Compliance status of the policy report.</span></span> <span data-ttu-id="90671-153">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="90671-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="90671-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="90671-154">lastReportedDateTime</span></span>|<span data-ttu-id="90671-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90671-155">DateTimeOffset</span></span>|<span data-ttu-id="90671-156">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="90671-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="90671-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="90671-157">userPrincipalName</span></span>|<span data-ttu-id="90671-158">字符串</span><span class="sxs-lookup"><span data-stu-id="90671-158">String</span></span>|<span data-ttu-id="90671-159">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="90671-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="90671-160">响应</span><span class="sxs-lookup"><span data-stu-id="90671-160">Response</span></span>
<span data-ttu-id="90671-161">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90671-161">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90671-162">示例</span><span class="sxs-lookup"><span data-stu-id="90671-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="90671-163">请求</span><span class="sxs-lookup"><span data-stu-id="90671-163">Request</span></span>
<span data-ttu-id="90671-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90671-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="90671-165">响应</span><span class="sxs-lookup"><span data-stu-id="90671-165">Response</span></span>
<span data-ttu-id="90671-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90671-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





