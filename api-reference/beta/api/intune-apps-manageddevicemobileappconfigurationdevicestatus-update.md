---
title: 更新 managedDeviceMobileAppConfigurationDeviceStatus
description: 更新 managedDeviceMobileAppConfigurationDeviceStatus 对象的属性。
ms.openlocfilehash: 92f3b2e4b119f1da552d276f4c59b8bdac2e55e3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045684"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="0c315-103">更新 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="0c315-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="0c315-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c315-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c315-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c315-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c315-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0c315-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c315-107">更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0c315-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c315-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0c315-108">Prerequisites</span></span>
<span data-ttu-id="0c315-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0c315-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c315-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c315-111">Permission type</span></span>|<span data-ttu-id="0c315-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0c315-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c315-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c315-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c315-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c315-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c315-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c315-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c315-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c315-116">Not supported.</span></span>|
|<span data-ttu-id="0c315-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c315-117">Application</span></span>|<span data-ttu-id="0c315-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c315-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c315-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c315-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="0c315-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c315-120">Request headers</span></span>
|<span data-ttu-id="0c315-121">标头</span><span class="sxs-lookup"><span data-stu-id="0c315-121">Header</span></span>|<span data-ttu-id="0c315-122">值</span><span class="sxs-lookup"><span data-stu-id="0c315-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c315-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c315-123">Authorization</span></span>|<span data-ttu-id="0c315-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0c315-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c315-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c315-125">Accept</span></span>|<span data-ttu-id="0c315-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c315-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c315-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c315-127">Request body</span></span>
<span data-ttu-id="0c315-128">在请求正文中，提供[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c315-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="0c315-129">下表显示时创建[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c315-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="0c315-130">属性</span><span class="sxs-lookup"><span data-stu-id="0c315-130">Property</span></span>|<span data-ttu-id="0c315-131">类型</span><span class="sxs-lookup"><span data-stu-id="0c315-131">Type</span></span>|<span data-ttu-id="0c315-132">说明</span><span class="sxs-lookup"><span data-stu-id="0c315-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c315-133">id</span><span class="sxs-lookup"><span data-stu-id="0c315-133">id</span></span>|<span data-ttu-id="0c315-134">String</span><span class="sxs-lookup"><span data-stu-id="0c315-134">String</span></span>|<span data-ttu-id="0c315-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0c315-135">Key of the entity.</span></span>|
|<span data-ttu-id="0c315-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c315-136">deviceDisplayName</span></span>|<span data-ttu-id="0c315-137">String</span><span class="sxs-lookup"><span data-stu-id="0c315-137">String</span></span>|<span data-ttu-id="0c315-138">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="0c315-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="0c315-139">userName</span><span class="sxs-lookup"><span data-stu-id="0c315-139">userName</span></span>|<span data-ttu-id="0c315-140">String</span><span class="sxs-lookup"><span data-stu-id="0c315-140">String</span></span>|<span data-ttu-id="0c315-141">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="0c315-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="0c315-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0c315-142">deviceModel</span></span>|<span data-ttu-id="0c315-143">String</span><span class="sxs-lookup"><span data-stu-id="0c315-143">String</span></span>|<span data-ttu-id="0c315-144">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="0c315-144">The device model that is being reported</span></span>|
|<span data-ttu-id="0c315-145">platform</span><span class="sxs-lookup"><span data-stu-id="0c315-145">platform</span></span>|<span data-ttu-id="0c315-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0c315-146">Int32</span></span>|<span data-ttu-id="0c315-147">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="0c315-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="0c315-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c315-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0c315-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c315-149">DateTimeOffset</span></span>|<span data-ttu-id="0c315-150">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="0c315-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0c315-151">状态</span><span class="sxs-lookup"><span data-stu-id="0c315-151">status</span></span>|[<span data-ttu-id="0c315-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0c315-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0c315-153">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="0c315-153">Compliance status of the policy report.</span></span> <span data-ttu-id="0c315-154">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="0c315-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0c315-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c315-155">lastReportedDateTime</span></span>|<span data-ttu-id="0c315-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c315-156">DateTimeOffset</span></span>|<span data-ttu-id="0c315-157">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="0c315-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="0c315-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c315-158">userPrincipalName</span></span>|<span data-ttu-id="0c315-159">String</span><span class="sxs-lookup"><span data-stu-id="0c315-159">String</span></span>|<span data-ttu-id="0c315-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="0c315-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="0c315-161">响应</span><span class="sxs-lookup"><span data-stu-id="0c315-161">Response</span></span>
<span data-ttu-id="0c315-162">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0c315-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c315-163">示例</span><span class="sxs-lookup"><span data-stu-id="0c315-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c315-164">请求</span><span class="sxs-lookup"><span data-stu-id="0c315-164">Request</span></span>
<span data-ttu-id="0c315-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c315-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 377

{
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

### <a name="response"></a><span data-ttu-id="0c315-166">响应</span><span class="sxs-lookup"><span data-stu-id="0c315-166">Response</span></span>
<span data-ttu-id="0c315-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c315-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





