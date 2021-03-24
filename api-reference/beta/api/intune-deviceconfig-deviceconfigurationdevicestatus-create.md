---
title: 创建 deviceConfigurationDeviceStatus
description: 创建新的 deviceConfigurationDeviceStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0a22e4fda8936355abd902c30a76a6bd25d636f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131650"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="8a82a-103">创建 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8a82a-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="8a82a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a82a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a82a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a82a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a82a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a82a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a82a-107">创建新的 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a82a-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a82a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a82a-108">Prerequisites</span></span>
<span data-ttu-id="8a82a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a82a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a82a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a82a-111">Permission type</span></span>|<span data-ttu-id="8a82a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a82a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a82a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a82a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a82a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a82a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a82a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a82a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a82a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a82a-116">Not supported.</span></span>|
|<span data-ttu-id="8a82a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a82a-117">Application</span></span>|<span data-ttu-id="8a82a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a82a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a82a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a82a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8a82a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a82a-120">Request headers</span></span>
|<span data-ttu-id="8a82a-121">标头</span><span class="sxs-lookup"><span data-stu-id="8a82a-121">Header</span></span>|<span data-ttu-id="8a82a-122">值</span><span class="sxs-lookup"><span data-stu-id="8a82a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a82a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a82a-123">Authorization</span></span>|<span data-ttu-id="8a82a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a82a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a82a-125">接受</span><span class="sxs-lookup"><span data-stu-id="8a82a-125">Accept</span></span>|<span data-ttu-id="8a82a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a82a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a82a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a82a-127">Request body</span></span>
<span data-ttu-id="8a82a-128">在请求正文中，提供 deviceConfigurationDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a82a-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="8a82a-129">下表显示创建 deviceConfigurationDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8a82a-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="8a82a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8a82a-130">Property</span></span>|<span data-ttu-id="8a82a-131">类型</span><span class="sxs-lookup"><span data-stu-id="8a82a-131">Type</span></span>|<span data-ttu-id="8a82a-132">说明</span><span class="sxs-lookup"><span data-stu-id="8a82a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a82a-133">id</span><span class="sxs-lookup"><span data-stu-id="8a82a-133">id</span></span>|<span data-ttu-id="8a82a-134">String</span><span class="sxs-lookup"><span data-stu-id="8a82a-134">String</span></span>|<span data-ttu-id="8a82a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8a82a-135">Key of the entity.</span></span>|
|<span data-ttu-id="8a82a-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8a82a-136">deviceDisplayName</span></span>|<span data-ttu-id="8a82a-137">String</span><span class="sxs-lookup"><span data-stu-id="8a82a-137">String</span></span>|<span data-ttu-id="8a82a-138">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="8a82a-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8a82a-139">userName</span><span class="sxs-lookup"><span data-stu-id="8a82a-139">userName</span></span>|<span data-ttu-id="8a82a-140">String</span><span class="sxs-lookup"><span data-stu-id="8a82a-140">String</span></span>|<span data-ttu-id="8a82a-141">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="8a82a-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="8a82a-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8a82a-142">deviceModel</span></span>|<span data-ttu-id="8a82a-143">String</span><span class="sxs-lookup"><span data-stu-id="8a82a-143">String</span></span>|<span data-ttu-id="8a82a-144">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="8a82a-144">The device model that is being reported</span></span>|
|<span data-ttu-id="8a82a-145">平台</span><span class="sxs-lookup"><span data-stu-id="8a82a-145">platform</span></span>|<span data-ttu-id="8a82a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8a82a-146">Int32</span></span>|<span data-ttu-id="8a82a-147">报告的设备平台</span><span class="sxs-lookup"><span data-stu-id="8a82a-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="8a82a-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8a82a-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8a82a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a82a-149">DateTimeOffset</span></span>|<span data-ttu-id="8a82a-150">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="8a82a-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="8a82a-151">status</span><span class="sxs-lookup"><span data-stu-id="8a82a-151">status</span></span>|[<span data-ttu-id="8a82a-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8a82a-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8a82a-153">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="8a82a-153">Compliance status of the policy report.</span></span> <span data-ttu-id="8a82a-154">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="8a82a-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8a82a-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a82a-155">lastReportedDateTime</span></span>|<span data-ttu-id="8a82a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a82a-156">DateTimeOffset</span></span>|<span data-ttu-id="8a82a-157">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="8a82a-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8a82a-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8a82a-158">userPrincipalName</span></span>|<span data-ttu-id="8a82a-159">String</span><span class="sxs-lookup"><span data-stu-id="8a82a-159">String</span></span>|<span data-ttu-id="8a82a-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="8a82a-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8a82a-161">响应</span><span class="sxs-lookup"><span data-stu-id="8a82a-161">Response</span></span>
<span data-ttu-id="8a82a-162">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a82a-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a82a-163">示例</span><span class="sxs-lookup"><span data-stu-id="8a82a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a82a-164">请求</span><span class="sxs-lookup"><span data-stu-id="8a82a-164">Request</span></span>
<span data-ttu-id="8a82a-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a82a-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a82a-166">响应</span><span class="sxs-lookup"><span data-stu-id="8a82a-166">Response</span></span>
<span data-ttu-id="8a82a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a82a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




