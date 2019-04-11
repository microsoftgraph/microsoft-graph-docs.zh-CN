---
title: 创建 iosUpdateDeviceStatus
description: 创建新的 iosUpdateDeviceStatus 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87afdbd29f05ec1c8fe1a36f3d5c13d841bd5730
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784127"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="8c3ba-103">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8c3ba-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="8c3ba-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c3ba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c3ba-106">创建新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-106">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c3ba-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c3ba-107">Prerequisites</span></span>
<span data-ttu-id="8c3ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c3ba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c3ba-110">Permission type</span></span>|<span data-ttu-id="8c3ba-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c3ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c3ba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c3ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c3ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c3ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c3ba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c3ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c3ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-115">Not supported.</span></span>|
|<span data-ttu-id="8c3ba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c3ba-116">Application</span></span>|<span data-ttu-id="8c3ba-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c3ba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c3ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8c3ba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c3ba-119">Request headers</span></span>
|<span data-ttu-id="8c3ba-120">标头</span><span class="sxs-lookup"><span data-stu-id="8c3ba-120">Header</span></span>|<span data-ttu-id="8c3ba-121">值</span><span class="sxs-lookup"><span data-stu-id="8c3ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c3ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c3ba-122">Authorization</span></span>|<span data-ttu-id="8c3ba-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c3ba-124">接受</span><span class="sxs-lookup"><span data-stu-id="8c3ba-124">Accept</span></span>|<span data-ttu-id="8c3ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c3ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c3ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c3ba-126">Request body</span></span>
<span data-ttu-id="8c3ba-127">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-127">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="8c3ba-128">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-128">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="8c3ba-129">属性</span><span class="sxs-lookup"><span data-stu-id="8c3ba-129">Property</span></span>|<span data-ttu-id="8c3ba-130">类型</span><span class="sxs-lookup"><span data-stu-id="8c3ba-130">Type</span></span>|<span data-ttu-id="8c3ba-131">说明</span><span class="sxs-lookup"><span data-stu-id="8c3ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c3ba-132">id</span><span class="sxs-lookup"><span data-stu-id="8c3ba-132">id</span></span>|<span data-ttu-id="8c3ba-133">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-133">String</span></span>|<span data-ttu-id="8c3ba-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-134">Key of the entity.</span></span>|
|<span data-ttu-id="8c3ba-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="8c3ba-135">installStatus</span></span>|[<span data-ttu-id="8c3ba-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="8c3ba-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="8c3ba-137">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-137">The installation status of the policy report.</span></span> <span data-ttu-id="8c3ba-138">可能的值是`success`: `available`、 `idle`、 `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、、、、、。 `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`</span><span class="sxs-lookup"><span data-stu-id="8c3ba-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="8c3ba-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="8c3ba-139">osVersion</span></span>|<span data-ttu-id="8c3ba-140">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-140">String</span></span>|<span data-ttu-id="8c3ba-141">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="8c3ba-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="8c3ba-142">deviceId</span></span>|<span data-ttu-id="8c3ba-143">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-143">String</span></span>|<span data-ttu-id="8c3ba-144">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="8c3ba-145">userId</span><span class="sxs-lookup"><span data-stu-id="8c3ba-145">userId</span></span>|<span data-ttu-id="8c3ba-146">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-146">String</span></span>|<span data-ttu-id="8c3ba-147">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="8c3ba-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8c3ba-148">deviceDisplayName</span></span>|<span data-ttu-id="8c3ba-149">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-149">String</span></span>|<span data-ttu-id="8c3ba-150">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8c3ba-151">userName</span><span class="sxs-lookup"><span data-stu-id="8c3ba-151">userName</span></span>|<span data-ttu-id="8c3ba-152">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-152">String</span></span>|<span data-ttu-id="8c3ba-153">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="8c3ba-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="8c3ba-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8c3ba-154">deviceModel</span></span>|<span data-ttu-id="8c3ba-155">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-155">String</span></span>|<span data-ttu-id="8c3ba-156">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="8c3ba-156">The device model that is being reported</span></span>|
|<span data-ttu-id="8c3ba-157">platform</span><span class="sxs-lookup"><span data-stu-id="8c3ba-157">platform</span></span>|<span data-ttu-id="8c3ba-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8c3ba-158">Int32</span></span>|<span data-ttu-id="8c3ba-159">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="8c3ba-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="8c3ba-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8c3ba-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8c3ba-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c3ba-161">DateTimeOffset</span></span>|<span data-ttu-id="8c3ba-162">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="8c3ba-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="8c3ba-163">status</span><span class="sxs-lookup"><span data-stu-id="8c3ba-163">status</span></span>|[<span data-ttu-id="8c3ba-164">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8c3ba-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8c3ba-165">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-165">Compliance status of the policy report.</span></span> <span data-ttu-id="8c3ba-166">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8c3ba-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c3ba-167">lastReportedDateTime</span></span>|<span data-ttu-id="8c3ba-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c3ba-168">DateTimeOffset</span></span>|<span data-ttu-id="8c3ba-169">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8c3ba-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8c3ba-170">userPrincipalName</span></span>|<span data-ttu-id="8c3ba-171">String</span><span class="sxs-lookup"><span data-stu-id="8c3ba-171">String</span></span>|<span data-ttu-id="8c3ba-172">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8c3ba-173">响应</span><span class="sxs-lookup"><span data-stu-id="8c3ba-173">Response</span></span>
<span data-ttu-id="8c3ba-174">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-174">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c3ba-175">示例</span><span class="sxs-lookup"><span data-stu-id="8c3ba-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c3ba-176">请求</span><span class="sxs-lookup"><span data-stu-id="8c3ba-176">Request</span></span>
<span data-ttu-id="8c3ba-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
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

### <a name="response"></a><span data-ttu-id="8c3ba-178">响应</span><span class="sxs-lookup"><span data-stu-id="8c3ba-178">Response</span></span>
<span data-ttu-id="8c3ba-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c3ba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 619

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
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





