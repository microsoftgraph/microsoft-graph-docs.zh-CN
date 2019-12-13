---
title: 更新 managedDeviceMobileAppConfigurationDeviceStatus
description: 更新 managedDeviceMobileAppConfigurationDeviceStatus 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f1c2cd1c4739b036a32fe3f56debc4a35502f4a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39950555"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="91140-103">更新 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="91140-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="91140-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91140-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91140-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91140-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91140-106">更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="91140-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91140-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="91140-107">Prerequisites</span></span>
<span data-ttu-id="91140-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91140-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="91140-110">Permission type</span></span>|<span data-ttu-id="91140-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="91140-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91140-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91140-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91140-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91140-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="91140-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91140-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91140-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="91140-115">Not supported.</span></span>|
|<span data-ttu-id="91140-116">Application</span><span class="sxs-lookup"><span data-stu-id="91140-116">Application</span></span>|<span data-ttu-id="91140-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91140-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91140-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91140-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="91140-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="91140-119">Request headers</span></span>
|<span data-ttu-id="91140-120">标头</span><span class="sxs-lookup"><span data-stu-id="91140-120">Header</span></span>|<span data-ttu-id="91140-121">值</span><span class="sxs-lookup"><span data-stu-id="91140-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91140-122">授权</span><span class="sxs-lookup"><span data-stu-id="91140-122">Authorization</span></span>|<span data-ttu-id="91140-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91140-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91140-124">接受</span><span class="sxs-lookup"><span data-stu-id="91140-124">Accept</span></span>|<span data-ttu-id="91140-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91140-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91140-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="91140-126">Request body</span></span>
<span data-ttu-id="91140-127">在请求正文中，提供[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91140-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="91140-128">下表显示创建[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="91140-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="91140-129">属性</span><span class="sxs-lookup"><span data-stu-id="91140-129">Property</span></span>|<span data-ttu-id="91140-130">类型</span><span class="sxs-lookup"><span data-stu-id="91140-130">Type</span></span>|<span data-ttu-id="91140-131">说明</span><span class="sxs-lookup"><span data-stu-id="91140-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91140-132">id</span><span class="sxs-lookup"><span data-stu-id="91140-132">id</span></span>|<span data-ttu-id="91140-133">String</span><span class="sxs-lookup"><span data-stu-id="91140-133">String</span></span>|<span data-ttu-id="91140-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="91140-134">Key of the entity.</span></span>|
|<span data-ttu-id="91140-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="91140-135">deviceDisplayName</span></span>|<span data-ttu-id="91140-136">字符串</span><span class="sxs-lookup"><span data-stu-id="91140-136">String</span></span>|<span data-ttu-id="91140-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="91140-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="91140-138">userName</span><span class="sxs-lookup"><span data-stu-id="91140-138">userName</span></span>|<span data-ttu-id="91140-139">字符串</span><span class="sxs-lookup"><span data-stu-id="91140-139">String</span></span>|<span data-ttu-id="91140-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="91140-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="91140-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="91140-141">deviceModel</span></span>|<span data-ttu-id="91140-142">String</span><span class="sxs-lookup"><span data-stu-id="91140-142">String</span></span>|<span data-ttu-id="91140-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="91140-143">The device model that is being reported</span></span>|
|<span data-ttu-id="91140-144">platform</span><span class="sxs-lookup"><span data-stu-id="91140-144">platform</span></span>|<span data-ttu-id="91140-145">Int32</span><span class="sxs-lookup"><span data-stu-id="91140-145">Int32</span></span>|<span data-ttu-id="91140-146">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="91140-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="91140-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="91140-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="91140-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91140-148">DateTimeOffset</span></span>|<span data-ttu-id="91140-149">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="91140-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="91140-150">status</span><span class="sxs-lookup"><span data-stu-id="91140-150">status</span></span>|[<span data-ttu-id="91140-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="91140-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="91140-152">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="91140-152">Compliance status of the policy report.</span></span> <span data-ttu-id="91140-153">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="91140-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="91140-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="91140-154">lastReportedDateTime</span></span>|<span data-ttu-id="91140-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91140-155">DateTimeOffset</span></span>|<span data-ttu-id="91140-156">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="91140-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="91140-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="91140-157">userPrincipalName</span></span>|<span data-ttu-id="91140-158">字符串</span><span class="sxs-lookup"><span data-stu-id="91140-158">String</span></span>|<span data-ttu-id="91140-159">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="91140-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="91140-160">响应</span><span class="sxs-lookup"><span data-stu-id="91140-160">Response</span></span>
<span data-ttu-id="91140-161">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91140-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91140-162">示例</span><span class="sxs-lookup"><span data-stu-id="91140-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="91140-163">请求</span><span class="sxs-lookup"><span data-stu-id="91140-163">Request</span></span>
<span data-ttu-id="91140-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91140-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="91140-165">响应</span><span class="sxs-lookup"><span data-stu-id="91140-165">Response</span></span>
<span data-ttu-id="91140-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91140-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
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





