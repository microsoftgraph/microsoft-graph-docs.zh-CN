---
title: 创建 iosUpdateDeviceStatus
description: 创建新的 iosUpdateDeviceStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9575fc17cf108e0b0960332224932bdb062f517
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131412"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="3b3fb-103">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="3b3fb-103">Create iosUpdateDeviceStatus</span></span>

<span data-ttu-id="3b3fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b3fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b3fb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b3fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b3fb-107">创建新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b3fb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b3fb-108">Prerequisites</span></span>
<span data-ttu-id="3b3fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b3fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b3fb-111">Permission type</span></span>|<span data-ttu-id="3b3fb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b3fb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b3fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b3fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b3fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b3fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b3fb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b3fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b3fb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-116">Not supported.</span></span>|
|<span data-ttu-id="3b3fb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b3fb-117">Application</span></span>|<span data-ttu-id="3b3fb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b3fb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b3fb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b3fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="3b3fb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b3fb-120">Request headers</span></span>
|<span data-ttu-id="3b3fb-121">标头</span><span class="sxs-lookup"><span data-stu-id="3b3fb-121">Header</span></span>|<span data-ttu-id="3b3fb-122">值</span><span class="sxs-lookup"><span data-stu-id="3b3fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b3fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b3fb-123">Authorization</span></span>|<span data-ttu-id="3b3fb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b3fb-125">接受</span><span class="sxs-lookup"><span data-stu-id="3b3fb-125">Accept</span></span>|<span data-ttu-id="3b3fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b3fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b3fb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b3fb-127">Request body</span></span>
<span data-ttu-id="3b3fb-128">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="3b3fb-129">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="3b3fb-130">属性</span><span class="sxs-lookup"><span data-stu-id="3b3fb-130">Property</span></span>|<span data-ttu-id="3b3fb-131">类型</span><span class="sxs-lookup"><span data-stu-id="3b3fb-131">Type</span></span>|<span data-ttu-id="3b3fb-132">说明</span><span class="sxs-lookup"><span data-stu-id="3b3fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b3fb-133">id</span><span class="sxs-lookup"><span data-stu-id="3b3fb-133">id</span></span>|<span data-ttu-id="3b3fb-134">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-134">String</span></span>|<span data-ttu-id="3b3fb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-135">Key of the entity.</span></span>|
|<span data-ttu-id="3b3fb-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="3b3fb-136">installStatus</span></span>|[<span data-ttu-id="3b3fb-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="3b3fb-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="3b3fb-138">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-138">The installation status of the policy report.</span></span> <span data-ttu-id="3b3fb-139">可能的值是 `success` `available` `idle` ：、、、、、、、、、、 `unknown` `mdmClientCrashed` `timeout` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation` `sharedDeviceUserLoggedInError` `updateError` `deviceOsHigherThanDesiredOsVersion` `updateScanFailed` 。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-139">Possible values are: `success`, `available`, `idle`, `unknown`, `mdmClientCrashed`, `timeout`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`, `updateError`, `deviceOsHigherThanDesiredOsVersion`, `updateScanFailed`.</span></span>|
|<span data-ttu-id="3b3fb-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="3b3fb-140">osVersion</span></span>|<span data-ttu-id="3b3fb-141">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-141">String</span></span>|<span data-ttu-id="3b3fb-142">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="3b3fb-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="3b3fb-143">deviceId</span></span>|<span data-ttu-id="3b3fb-144">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-144">String</span></span>|<span data-ttu-id="3b3fb-145">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="3b3fb-146">userId</span><span class="sxs-lookup"><span data-stu-id="3b3fb-146">userId</span></span>|<span data-ttu-id="3b3fb-147">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-147">String</span></span>|<span data-ttu-id="3b3fb-148">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="3b3fb-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3b3fb-149">deviceDisplayName</span></span>|<span data-ttu-id="3b3fb-150">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-150">String</span></span>|<span data-ttu-id="3b3fb-151">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="3b3fb-152">userName</span><span class="sxs-lookup"><span data-stu-id="3b3fb-152">userName</span></span>|<span data-ttu-id="3b3fb-153">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-153">String</span></span>|<span data-ttu-id="3b3fb-154">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="3b3fb-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="3b3fb-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3b3fb-155">deviceModel</span></span>|<span data-ttu-id="3b3fb-156">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-156">String</span></span>|<span data-ttu-id="3b3fb-157">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="3b3fb-157">The device model that is being reported</span></span>|
|<span data-ttu-id="3b3fb-158">平台</span><span class="sxs-lookup"><span data-stu-id="3b3fb-158">platform</span></span>|<span data-ttu-id="3b3fb-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3b3fb-159">Int32</span></span>|<span data-ttu-id="3b3fb-160">报告的设备平台</span><span class="sxs-lookup"><span data-stu-id="3b3fb-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="3b3fb-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b3fb-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3b3fb-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b3fb-162">DateTimeOffset</span></span>|<span data-ttu-id="3b3fb-163">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="3b3fb-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="3b3fb-164">status</span><span class="sxs-lookup"><span data-stu-id="3b3fb-164">status</span></span>|[<span data-ttu-id="3b3fb-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3b3fb-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3b3fb-166">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-166">Compliance status of the policy report.</span></span> <span data-ttu-id="3b3fb-167">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3b3fb-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b3fb-168">lastReportedDateTime</span></span>|<span data-ttu-id="3b3fb-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b3fb-169">DateTimeOffset</span></span>|<span data-ttu-id="3b3fb-170">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="3b3fb-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b3fb-171">userPrincipalName</span></span>|<span data-ttu-id="3b3fb-172">String</span><span class="sxs-lookup"><span data-stu-id="3b3fb-172">String</span></span>|<span data-ttu-id="3b3fb-173">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="3b3fb-174">响应</span><span class="sxs-lookup"><span data-stu-id="3b3fb-174">Response</span></span>
<span data-ttu-id="3b3fb-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b3fb-176">示例</span><span class="sxs-lookup"><span data-stu-id="3b3fb-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b3fb-177">请求</span><span class="sxs-lookup"><span data-stu-id="3b3fb-177">Request</span></span>
<span data-ttu-id="3b3fb-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b3fb-179">响应</span><span class="sxs-lookup"><span data-stu-id="3b3fb-179">Response</span></span>
<span data-ttu-id="3b3fb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b3fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




