---
title: 更新 iosUpdateDeviceStatus
description: 更新 iosUpdateDeviceStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c41b8f777784ce7d10f591456b0511bea903a8c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747940"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="d15ba-103">更新 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d15ba-103">Update iosUpdateDeviceStatus</span></span>

<span data-ttu-id="d15ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d15ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d15ba-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d15ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d15ba-106">更新 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d15ba-106">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d15ba-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d15ba-107">Prerequisites</span></span>
<span data-ttu-id="d15ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d15ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d15ba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d15ba-110">Permission type</span></span>|<span data-ttu-id="d15ba-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d15ba-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d15ba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d15ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d15ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d15ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d15ba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d15ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d15ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d15ba-115">Not supported.</span></span>|
|<span data-ttu-id="d15ba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d15ba-116">Application</span></span>|<span data-ttu-id="d15ba-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d15ba-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d15ba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d15ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="d15ba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d15ba-119">Request headers</span></span>
|<span data-ttu-id="d15ba-120">标头</span><span class="sxs-lookup"><span data-stu-id="d15ba-120">Header</span></span>|<span data-ttu-id="d15ba-121">值</span><span class="sxs-lookup"><span data-stu-id="d15ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d15ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d15ba-122">Authorization</span></span>|<span data-ttu-id="d15ba-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d15ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d15ba-124">接受</span><span class="sxs-lookup"><span data-stu-id="d15ba-124">Accept</span></span>|<span data-ttu-id="d15ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d15ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d15ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d15ba-126">Request body</span></span>
<span data-ttu-id="d15ba-127">在请求正文中，提供 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d15ba-127">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="d15ba-128">下表显示了创建 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d15ba-128">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="d15ba-129">属性</span><span class="sxs-lookup"><span data-stu-id="d15ba-129">Property</span></span>|<span data-ttu-id="d15ba-130">类型</span><span class="sxs-lookup"><span data-stu-id="d15ba-130">Type</span></span>|<span data-ttu-id="d15ba-131">说明</span><span class="sxs-lookup"><span data-stu-id="d15ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d15ba-132">id</span><span class="sxs-lookup"><span data-stu-id="d15ba-132">id</span></span>|<span data-ttu-id="d15ba-133">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-133">String</span></span>|<span data-ttu-id="d15ba-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d15ba-134">Key of the entity.</span></span>|
|<span data-ttu-id="d15ba-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="d15ba-135">installStatus</span></span>|[<span data-ttu-id="d15ba-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d15ba-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="d15ba-137">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="d15ba-137">The installation status of the policy report.</span></span> <span data-ttu-id="d15ba-138">可能的值是 `success` `available` `idle` ：、、、、、、、、、 `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation` `sharedDeviceUserLoggedInError` `deviceOsHigherThanDesiredOsVersion` 。</span><span class="sxs-lookup"><span data-stu-id="d15ba-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`, `deviceOsHigherThanDesiredOsVersion`.</span></span>|
|<span data-ttu-id="d15ba-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="d15ba-139">osVersion</span></span>|<span data-ttu-id="d15ba-140">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-140">String</span></span>|<span data-ttu-id="d15ba-141">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="d15ba-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="d15ba-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="d15ba-142">deviceId</span></span>|<span data-ttu-id="d15ba-143">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-143">String</span></span>|<span data-ttu-id="d15ba-144">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="d15ba-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="d15ba-145">userId</span><span class="sxs-lookup"><span data-stu-id="d15ba-145">userId</span></span>|<span data-ttu-id="d15ba-146">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-146">String</span></span>|<span data-ttu-id="d15ba-147">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d15ba-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="d15ba-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d15ba-148">deviceDisplayName</span></span>|<span data-ttu-id="d15ba-149">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-149">String</span></span>|<span data-ttu-id="d15ba-150">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="d15ba-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d15ba-151">userName</span><span class="sxs-lookup"><span data-stu-id="d15ba-151">userName</span></span>|<span data-ttu-id="d15ba-152">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-152">String</span></span>|<span data-ttu-id="d15ba-153">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="d15ba-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="d15ba-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d15ba-154">deviceModel</span></span>|<span data-ttu-id="d15ba-155">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-155">String</span></span>|<span data-ttu-id="d15ba-156">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="d15ba-156">The device model that is being reported</span></span>|
|<span data-ttu-id="d15ba-157">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d15ba-157">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d15ba-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d15ba-158">DateTimeOffset</span></span>|<span data-ttu-id="d15ba-159">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d15ba-159">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d15ba-160">status</span><span class="sxs-lookup"><span data-stu-id="d15ba-160">status</span></span>|[<span data-ttu-id="d15ba-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d15ba-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d15ba-162">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d15ba-162">Compliance status of the policy report.</span></span> <span data-ttu-id="d15ba-163">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d15ba-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d15ba-164">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d15ba-164">lastReportedDateTime</span></span>|<span data-ttu-id="d15ba-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d15ba-165">DateTimeOffset</span></span>|<span data-ttu-id="d15ba-166">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="d15ba-166">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d15ba-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d15ba-167">userPrincipalName</span></span>|<span data-ttu-id="d15ba-168">String</span><span class="sxs-lookup"><span data-stu-id="d15ba-168">String</span></span>|<span data-ttu-id="d15ba-169">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d15ba-169">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d15ba-170">响应</span><span class="sxs-lookup"><span data-stu-id="d15ba-170">Response</span></span>
<span data-ttu-id="d15ba-171">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d15ba-171">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d15ba-172">示例</span><span class="sxs-lookup"><span data-stu-id="d15ba-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d15ba-173">请求</span><span class="sxs-lookup"><span data-stu-id="d15ba-173">Request</span></span>
<span data-ttu-id="d15ba-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d15ba-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d15ba-175">响应</span><span class="sxs-lookup"><span data-stu-id="d15ba-175">Response</span></span>
<span data-ttu-id="d15ba-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d15ba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




