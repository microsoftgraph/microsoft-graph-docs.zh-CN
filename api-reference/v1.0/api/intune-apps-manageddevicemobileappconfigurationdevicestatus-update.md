---
title: 更新 managedDeviceMobileAppConfigurationDeviceStatus
description: 更新 managedDeviceMobileAppConfigurationDeviceStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df78a37d8bf3ede65243c5e1b2eb903e3c1998b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002277"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="cdb42-103">更新 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="cdb42-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="cdb42-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdb42-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdb42-105">更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cdb42-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdb42-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cdb42-106">Prerequisites</span></span>
<span data-ttu-id="cdb42-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdb42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdb42-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdb42-109">Permission type</span></span>|<span data-ttu-id="cdb42-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cdb42-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdb42-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdb42-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdb42-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdb42-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cdb42-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdb42-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdb42-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdb42-114">Not supported.</span></span>|
|<span data-ttu-id="cdb42-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdb42-115">Application</span></span>|<span data-ttu-id="cdb42-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdb42-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdb42-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdb42-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="cdb42-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdb42-118">Request headers</span></span>
|<span data-ttu-id="cdb42-119">标头</span><span class="sxs-lookup"><span data-stu-id="cdb42-119">Header</span></span>|<span data-ttu-id="cdb42-120">值</span><span class="sxs-lookup"><span data-stu-id="cdb42-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdb42-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdb42-121">Authorization</span></span>|<span data-ttu-id="cdb42-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cdb42-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdb42-123">接受</span><span class="sxs-lookup"><span data-stu-id="cdb42-123">Accept</span></span>|<span data-ttu-id="cdb42-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdb42-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdb42-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdb42-125">Request body</span></span>
<span data-ttu-id="cdb42-126">在请求正文中, 提供[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdb42-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="cdb42-127">下表显示创建[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cdb42-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="cdb42-128">属性</span><span class="sxs-lookup"><span data-stu-id="cdb42-128">Property</span></span>|<span data-ttu-id="cdb42-129">类型</span><span class="sxs-lookup"><span data-stu-id="cdb42-129">Type</span></span>|<span data-ttu-id="cdb42-130">说明</span><span class="sxs-lookup"><span data-stu-id="cdb42-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdb42-131">id</span><span class="sxs-lookup"><span data-stu-id="cdb42-131">id</span></span>|<span data-ttu-id="cdb42-132">String</span><span class="sxs-lookup"><span data-stu-id="cdb42-132">String</span></span>|<span data-ttu-id="cdb42-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cdb42-133">Key of the entity.</span></span>|
|<span data-ttu-id="cdb42-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cdb42-134">deviceDisplayName</span></span>|<span data-ttu-id="cdb42-135">String</span><span class="sxs-lookup"><span data-stu-id="cdb42-135">String</span></span>|<span data-ttu-id="cdb42-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="cdb42-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="cdb42-137">userName</span><span class="sxs-lookup"><span data-stu-id="cdb42-137">userName</span></span>|<span data-ttu-id="cdb42-138">String</span><span class="sxs-lookup"><span data-stu-id="cdb42-138">String</span></span>|<span data-ttu-id="cdb42-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="cdb42-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="cdb42-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="cdb42-140">deviceModel</span></span>|<span data-ttu-id="cdb42-141">String</span><span class="sxs-lookup"><span data-stu-id="cdb42-141">String</span></span>|<span data-ttu-id="cdb42-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="cdb42-142">The device model that is being reported</span></span>|
|<span data-ttu-id="cdb42-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cdb42-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="cdb42-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdb42-144">DateTimeOffset</span></span>|<span data-ttu-id="cdb42-145">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="cdb42-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="cdb42-146">status</span><span class="sxs-lookup"><span data-stu-id="cdb42-146">status</span></span>|[<span data-ttu-id="cdb42-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="cdb42-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="cdb42-148">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="cdb42-148">Compliance status of the policy report.</span></span> <span data-ttu-id="cdb42-149">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="cdb42-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="cdb42-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdb42-150">lastReportedDateTime</span></span>|<span data-ttu-id="cdb42-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdb42-151">DateTimeOffset</span></span>|<span data-ttu-id="cdb42-152">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="cdb42-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="cdb42-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cdb42-153">userPrincipalName</span></span>|<span data-ttu-id="cdb42-154">String</span><span class="sxs-lookup"><span data-stu-id="cdb42-154">String</span></span>|<span data-ttu-id="cdb42-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="cdb42-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="cdb42-156">响应</span><span class="sxs-lookup"><span data-stu-id="cdb42-156">Response</span></span>
<span data-ttu-id="cdb42-157">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cdb42-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdb42-158">示例</span><span class="sxs-lookup"><span data-stu-id="cdb42-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdb42-159">请求</span><span class="sxs-lookup"><span data-stu-id="cdb42-159">Request</span></span>
<span data-ttu-id="cdb42-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdb42-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="cdb42-161">响应</span><span class="sxs-lookup"><span data-stu-id="cdb42-161">Response</span></span>
<span data-ttu-id="cdb42-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdb42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



