---
title: 创建 iosUpdateDeviceStatus
description: 创建新的 iosUpdateDeviceStatus 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 484b7155feed87a36e717177555c2512acf285ff
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948646"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="c6ae8-103">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="c6ae8-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="c6ae8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6ae8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6ae8-106">创建新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-106">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6ae8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6ae8-107">Prerequisites</span></span>
<span data-ttu-id="c6ae8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6ae8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6ae8-110">Permission type</span></span>|<span data-ttu-id="c6ae8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c6ae8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6ae8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6ae8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6ae8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6ae8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6ae8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6ae8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6ae8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-115">Not supported.</span></span>|
|<span data-ttu-id="c6ae8-116">Application</span><span class="sxs-lookup"><span data-stu-id="c6ae8-116">Application</span></span>|<span data-ttu-id="c6ae8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6ae8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6ae8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6ae8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c6ae8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6ae8-119">Request headers</span></span>
|<span data-ttu-id="c6ae8-120">标头</span><span class="sxs-lookup"><span data-stu-id="c6ae8-120">Header</span></span>|<span data-ttu-id="c6ae8-121">值</span><span class="sxs-lookup"><span data-stu-id="c6ae8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6ae8-122">授权</span><span class="sxs-lookup"><span data-stu-id="c6ae8-122">Authorization</span></span>|<span data-ttu-id="c6ae8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6ae8-124">接受</span><span class="sxs-lookup"><span data-stu-id="c6ae8-124">Accept</span></span>|<span data-ttu-id="c6ae8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6ae8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6ae8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6ae8-126">Request body</span></span>
<span data-ttu-id="c6ae8-127">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-127">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="c6ae8-128">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-128">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="c6ae8-129">属性</span><span class="sxs-lookup"><span data-stu-id="c6ae8-129">Property</span></span>|<span data-ttu-id="c6ae8-130">类型</span><span class="sxs-lookup"><span data-stu-id="c6ae8-130">Type</span></span>|<span data-ttu-id="c6ae8-131">说明</span><span class="sxs-lookup"><span data-stu-id="c6ae8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ae8-132">id</span><span class="sxs-lookup"><span data-stu-id="c6ae8-132">id</span></span>|<span data-ttu-id="c6ae8-133">String</span><span class="sxs-lookup"><span data-stu-id="c6ae8-133">String</span></span>|<span data-ttu-id="c6ae8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-134">Key of the entity.</span></span>|
|<span data-ttu-id="c6ae8-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="c6ae8-135">installStatus</span></span>|[<span data-ttu-id="c6ae8-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c6ae8-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="c6ae8-137">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-137">The installation status of the policy report.</span></span> <span data-ttu-id="c6ae8-138">可能的值是`success`： `available`、 `idle`、 `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、、、、、。 `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`</span><span class="sxs-lookup"><span data-stu-id="c6ae8-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="c6ae8-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="c6ae8-139">osVersion</span></span>|<span data-ttu-id="c6ae8-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c6ae8-140">String</span></span>|<span data-ttu-id="c6ae8-141">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="c6ae8-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="c6ae8-142">deviceId</span></span>|<span data-ttu-id="c6ae8-143">String</span><span class="sxs-lookup"><span data-stu-id="c6ae8-143">String</span></span>|<span data-ttu-id="c6ae8-144">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="c6ae8-145">userId</span><span class="sxs-lookup"><span data-stu-id="c6ae8-145">userId</span></span>|<span data-ttu-id="c6ae8-146">String</span><span class="sxs-lookup"><span data-stu-id="c6ae8-146">String</span></span>|<span data-ttu-id="c6ae8-147">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="c6ae8-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c6ae8-148">deviceDisplayName</span></span>|<span data-ttu-id="c6ae8-149">字符串</span><span class="sxs-lookup"><span data-stu-id="c6ae8-149">String</span></span>|<span data-ttu-id="c6ae8-150">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c6ae8-151">userName</span><span class="sxs-lookup"><span data-stu-id="c6ae8-151">userName</span></span>|<span data-ttu-id="c6ae8-152">字符串</span><span class="sxs-lookup"><span data-stu-id="c6ae8-152">String</span></span>|<span data-ttu-id="c6ae8-153">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="c6ae8-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="c6ae8-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c6ae8-154">deviceModel</span></span>|<span data-ttu-id="c6ae8-155">String</span><span class="sxs-lookup"><span data-stu-id="c6ae8-155">String</span></span>|<span data-ttu-id="c6ae8-156">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="c6ae8-156">The device model that is being reported</span></span>|
|<span data-ttu-id="c6ae8-157">platform</span><span class="sxs-lookup"><span data-stu-id="c6ae8-157">platform</span></span>|<span data-ttu-id="c6ae8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c6ae8-158">Int32</span></span>|<span data-ttu-id="c6ae8-159">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="c6ae8-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="c6ae8-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ae8-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c6ae8-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ae8-161">DateTimeOffset</span></span>|<span data-ttu-id="c6ae8-162">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="c6ae8-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="c6ae8-163">status</span><span class="sxs-lookup"><span data-stu-id="c6ae8-163">status</span></span>|[<span data-ttu-id="c6ae8-164">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c6ae8-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c6ae8-165">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-165">Compliance status of the policy report.</span></span> <span data-ttu-id="c6ae8-166">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c6ae8-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ae8-167">lastReportedDateTime</span></span>|<span data-ttu-id="c6ae8-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ae8-168">DateTimeOffset</span></span>|<span data-ttu-id="c6ae8-169">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c6ae8-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c6ae8-170">userPrincipalName</span></span>|<span data-ttu-id="c6ae8-171">字符串</span><span class="sxs-lookup"><span data-stu-id="c6ae8-171">String</span></span>|<span data-ttu-id="c6ae8-172">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c6ae8-173">响应</span><span class="sxs-lookup"><span data-stu-id="c6ae8-173">Response</span></span>
<span data-ttu-id="c6ae8-174">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-174">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6ae8-175">示例</span><span class="sxs-lookup"><span data-stu-id="c6ae8-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6ae8-176">请求</span><span class="sxs-lookup"><span data-stu-id="c6ae8-176">Request</span></span>
<span data-ttu-id="c6ae8-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6ae8-178">响应</span><span class="sxs-lookup"><span data-stu-id="c6ae8-178">Response</span></span>
<span data-ttu-id="c6ae8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6ae8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





