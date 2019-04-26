---
title: 更新 iosUpdateDeviceStatus
description: 更新 iosUpdateDeviceStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ede7348a948d78c2ec9f3219fa1ff072d17915f3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549865"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="7aaf1-103">更新 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="7aaf1-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="7aaf1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aaf1-105">更新 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-105">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7aaf1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7aaf1-106">Prerequisites</span></span>
<span data-ttu-id="7aaf1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aaf1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aaf1-109">Permission type</span></span>|<span data-ttu-id="7aaf1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7aaf1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aaf1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aaf1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7aaf1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aaf1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7aaf1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7aaf1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aaf1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-114">Not supported.</span></span>|
|<span data-ttu-id="7aaf1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aaf1-115">Application</span></span>|<span data-ttu-id="7aaf1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aaf1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aaf1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="7aaf1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aaf1-118">Request headers</span></span>
|<span data-ttu-id="7aaf1-119">标头</span><span class="sxs-lookup"><span data-stu-id="7aaf1-119">Header</span></span>|<span data-ttu-id="7aaf1-120">值</span><span class="sxs-lookup"><span data-stu-id="7aaf1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aaf1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aaf1-121">Authorization</span></span>|<span data-ttu-id="7aaf1-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aaf1-123">接受</span><span class="sxs-lookup"><span data-stu-id="7aaf1-123">Accept</span></span>|<span data-ttu-id="7aaf1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7aaf1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aaf1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aaf1-125">Request body</span></span>
<span data-ttu-id="7aaf1-126">在请求正文中，提供 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-126">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="7aaf1-127">下表显示了创建 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-127">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="7aaf1-128">属性</span><span class="sxs-lookup"><span data-stu-id="7aaf1-128">Property</span></span>|<span data-ttu-id="7aaf1-129">类型</span><span class="sxs-lookup"><span data-stu-id="7aaf1-129">Type</span></span>|<span data-ttu-id="7aaf1-130">说明</span><span class="sxs-lookup"><span data-stu-id="7aaf1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aaf1-131">id</span><span class="sxs-lookup"><span data-stu-id="7aaf1-131">id</span></span>|<span data-ttu-id="7aaf1-132">字符串</span><span class="sxs-lookup"><span data-stu-id="7aaf1-132">String</span></span>|<span data-ttu-id="7aaf1-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-133">Key of the entity.</span></span>|
|<span data-ttu-id="7aaf1-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="7aaf1-134">installStatus</span></span>|[<span data-ttu-id="7aaf1-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="7aaf1-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="7aaf1-136">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-136">The installation status of the policy report.</span></span> <span data-ttu-id="7aaf1-137">可能的值是`success`: `available`、 `idle`、 `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、、、、、。 `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`</span><span class="sxs-lookup"><span data-stu-id="7aaf1-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="7aaf1-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="7aaf1-138">osVersion</span></span>|<span data-ttu-id="7aaf1-139">String</span><span class="sxs-lookup"><span data-stu-id="7aaf1-139">String</span></span>|<span data-ttu-id="7aaf1-140">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="7aaf1-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="7aaf1-141">deviceId</span></span>|<span data-ttu-id="7aaf1-142">String</span><span class="sxs-lookup"><span data-stu-id="7aaf1-142">String</span></span>|<span data-ttu-id="7aaf1-143">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="7aaf1-144">userId</span><span class="sxs-lookup"><span data-stu-id="7aaf1-144">userId</span></span>|<span data-ttu-id="7aaf1-145">String</span><span class="sxs-lookup"><span data-stu-id="7aaf1-145">String</span></span>|<span data-ttu-id="7aaf1-146">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="7aaf1-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7aaf1-147">deviceDisplayName</span></span>|<span data-ttu-id="7aaf1-148">String</span><span class="sxs-lookup"><span data-stu-id="7aaf1-148">String</span></span>|<span data-ttu-id="7aaf1-149">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="7aaf1-150">userName</span><span class="sxs-lookup"><span data-stu-id="7aaf1-150">userName</span></span>|<span data-ttu-id="7aaf1-151">String</span><span class="sxs-lookup"><span data-stu-id="7aaf1-151">String</span></span>|<span data-ttu-id="7aaf1-152">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="7aaf1-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="7aaf1-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7aaf1-153">deviceModel</span></span>|<span data-ttu-id="7aaf1-154">String</span><span class="sxs-lookup"><span data-stu-id="7aaf1-154">String</span></span>|<span data-ttu-id="7aaf1-155">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="7aaf1-155">The device model that is being reported</span></span>|
|<span data-ttu-id="7aaf1-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7aaf1-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7aaf1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aaf1-157">DateTimeOffset</span></span>|<span data-ttu-id="7aaf1-158">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="7aaf1-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="7aaf1-159">status</span><span class="sxs-lookup"><span data-stu-id="7aaf1-159">status</span></span>|[<span data-ttu-id="7aaf1-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7aaf1-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7aaf1-161">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-161">Compliance status of the policy report.</span></span> <span data-ttu-id="7aaf1-162">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7aaf1-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7aaf1-163">lastReportedDateTime</span></span>|<span data-ttu-id="7aaf1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aaf1-164">DateTimeOffset</span></span>|<span data-ttu-id="7aaf1-165">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="7aaf1-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7aaf1-166">userPrincipalName</span></span>|<span data-ttu-id="7aaf1-167">String</span><span class="sxs-lookup"><span data-stu-id="7aaf1-167">String</span></span>|<span data-ttu-id="7aaf1-168">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="7aaf1-169">响应</span><span class="sxs-lookup"><span data-stu-id="7aaf1-169">Response</span></span>
<span data-ttu-id="7aaf1-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aaf1-171">示例</span><span class="sxs-lookup"><span data-stu-id="7aaf1-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="7aaf1-172">请求</span><span class="sxs-lookup"><span data-stu-id="7aaf1-172">Request</span></span>
<span data-ttu-id="7aaf1-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="7aaf1-174">响应</span><span class="sxs-lookup"><span data-stu-id="7aaf1-174">Response</span></span>
<span data-ttu-id="7aaf1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7aaf1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



