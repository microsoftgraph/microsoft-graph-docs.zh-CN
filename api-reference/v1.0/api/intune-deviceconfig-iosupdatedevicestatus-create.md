---
title: 创建 iosUpdateDeviceStatus
description: 创建新的 iosUpdateDeviceStatus 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95a9234320263e45c718e8c706ede12569b03352
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017236"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="46cbd-103">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="46cbd-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="46cbd-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46cbd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46cbd-105">创建新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46cbd-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46cbd-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="46cbd-106">Prerequisites</span></span>
<span data-ttu-id="46cbd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46cbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46cbd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="46cbd-109">Permission type</span></span>|<span data-ttu-id="46cbd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46cbd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46cbd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46cbd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46cbd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46cbd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46cbd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46cbd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46cbd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="46cbd-114">Not supported.</span></span>|
|<span data-ttu-id="46cbd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="46cbd-115">Application</span></span>|<span data-ttu-id="46cbd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46cbd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46cbd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46cbd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="46cbd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="46cbd-118">Request headers</span></span>
|<span data-ttu-id="46cbd-119">标头</span><span class="sxs-lookup"><span data-stu-id="46cbd-119">Header</span></span>|<span data-ttu-id="46cbd-120">值</span><span class="sxs-lookup"><span data-stu-id="46cbd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46cbd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46cbd-121">Authorization</span></span>|<span data-ttu-id="46cbd-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46cbd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46cbd-123">接受</span><span class="sxs-lookup"><span data-stu-id="46cbd-123">Accept</span></span>|<span data-ttu-id="46cbd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46cbd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46cbd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="46cbd-125">Request body</span></span>
<span data-ttu-id="46cbd-126">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46cbd-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="46cbd-127">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="46cbd-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="46cbd-128">属性</span><span class="sxs-lookup"><span data-stu-id="46cbd-128">Property</span></span>|<span data-ttu-id="46cbd-129">类型</span><span class="sxs-lookup"><span data-stu-id="46cbd-129">Type</span></span>|<span data-ttu-id="46cbd-130">说明</span><span class="sxs-lookup"><span data-stu-id="46cbd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46cbd-131">id</span><span class="sxs-lookup"><span data-stu-id="46cbd-131">id</span></span>|<span data-ttu-id="46cbd-132">String</span><span class="sxs-lookup"><span data-stu-id="46cbd-132">String</span></span>|<span data-ttu-id="46cbd-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="46cbd-133">Key of the entity.</span></span>|
|<span data-ttu-id="46cbd-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="46cbd-134">installStatus</span></span>|[<span data-ttu-id="46cbd-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="46cbd-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="46cbd-136">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="46cbd-136">The installation status of the policy report.</span></span> <span data-ttu-id="46cbd-137">可能的值是`success`: `available`、 `idle`、 `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、、、、、。 `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`</span><span class="sxs-lookup"><span data-stu-id="46cbd-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="46cbd-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="46cbd-138">osVersion</span></span>|<span data-ttu-id="46cbd-139">String</span><span class="sxs-lookup"><span data-stu-id="46cbd-139">String</span></span>|<span data-ttu-id="46cbd-140">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="46cbd-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="46cbd-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="46cbd-141">deviceId</span></span>|<span data-ttu-id="46cbd-142">String</span><span class="sxs-lookup"><span data-stu-id="46cbd-142">String</span></span>|<span data-ttu-id="46cbd-143">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="46cbd-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="46cbd-144">userId</span><span class="sxs-lookup"><span data-stu-id="46cbd-144">userId</span></span>|<span data-ttu-id="46cbd-145">String</span><span class="sxs-lookup"><span data-stu-id="46cbd-145">String</span></span>|<span data-ttu-id="46cbd-146">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="46cbd-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="46cbd-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="46cbd-147">deviceDisplayName</span></span>|<span data-ttu-id="46cbd-148">String</span><span class="sxs-lookup"><span data-stu-id="46cbd-148">String</span></span>|<span data-ttu-id="46cbd-149">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="46cbd-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="46cbd-150">userName</span><span class="sxs-lookup"><span data-stu-id="46cbd-150">userName</span></span>|<span data-ttu-id="46cbd-151">String</span><span class="sxs-lookup"><span data-stu-id="46cbd-151">String</span></span>|<span data-ttu-id="46cbd-152">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="46cbd-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="46cbd-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="46cbd-153">deviceModel</span></span>|<span data-ttu-id="46cbd-154">String</span><span class="sxs-lookup"><span data-stu-id="46cbd-154">String</span></span>|<span data-ttu-id="46cbd-155">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="46cbd-155">The device model that is being reported</span></span>|
|<span data-ttu-id="46cbd-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="46cbd-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="46cbd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46cbd-157">DateTimeOffset</span></span>|<span data-ttu-id="46cbd-158">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="46cbd-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="46cbd-159">status</span><span class="sxs-lookup"><span data-stu-id="46cbd-159">status</span></span>|[<span data-ttu-id="46cbd-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="46cbd-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="46cbd-161">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="46cbd-161">Compliance status of the policy report.</span></span> <span data-ttu-id="46cbd-162">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="46cbd-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="46cbd-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="46cbd-163">lastReportedDateTime</span></span>|<span data-ttu-id="46cbd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46cbd-164">DateTimeOffset</span></span>|<span data-ttu-id="46cbd-165">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="46cbd-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="46cbd-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46cbd-166">userPrincipalName</span></span>|<span data-ttu-id="46cbd-167">字符串</span><span class="sxs-lookup"><span data-stu-id="46cbd-167">String</span></span>|<span data-ttu-id="46cbd-168">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="46cbd-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="46cbd-169">响应</span><span class="sxs-lookup"><span data-stu-id="46cbd-169">Response</span></span>
<span data-ttu-id="46cbd-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46cbd-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46cbd-171">示例</span><span class="sxs-lookup"><span data-stu-id="46cbd-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="46cbd-172">请求</span><span class="sxs-lookup"><span data-stu-id="46cbd-172">Request</span></span>
<span data-ttu-id="46cbd-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46cbd-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
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

### <a name="response"></a><span data-ttu-id="46cbd-174">响应</span><span class="sxs-lookup"><span data-stu-id="46cbd-174">Response</span></span>
<span data-ttu-id="46cbd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46cbd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



