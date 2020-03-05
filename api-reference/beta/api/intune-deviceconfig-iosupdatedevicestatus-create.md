---
title: 创建 iosUpdateDeviceStatus
description: 创建新的 iosUpdateDeviceStatus 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92d412a6426c5832ea6ecebc1f24a9af9dc65145
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442598"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="d3944-103">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d3944-103">Create iosUpdateDeviceStatus</span></span>

<span data-ttu-id="d3944-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d3944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3944-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3944-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3944-107">创建新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3944-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3944-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3944-108">Prerequisites</span></span>
<span data-ttu-id="d3944-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3944-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3944-111">Permission type</span></span>|<span data-ttu-id="d3944-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d3944-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3944-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3944-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3944-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3944-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3944-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3944-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3944-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3944-116">Not supported.</span></span>|
|<span data-ttu-id="d3944-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3944-117">Application</span></span>|<span data-ttu-id="d3944-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3944-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3944-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3944-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d3944-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3944-120">Request headers</span></span>
|<span data-ttu-id="d3944-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3944-121">Header</span></span>|<span data-ttu-id="d3944-122">值</span><span class="sxs-lookup"><span data-stu-id="d3944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3944-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3944-123">Authorization</span></span>|<span data-ttu-id="d3944-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3944-125">接受</span><span class="sxs-lookup"><span data-stu-id="d3944-125">Accept</span></span>|<span data-ttu-id="d3944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3944-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3944-127">Request body</span></span>
<span data-ttu-id="d3944-128">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3944-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="d3944-129">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d3944-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="d3944-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3944-130">Property</span></span>|<span data-ttu-id="d3944-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3944-131">Type</span></span>|<span data-ttu-id="d3944-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3944-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3944-133">id</span><span class="sxs-lookup"><span data-stu-id="d3944-133">id</span></span>|<span data-ttu-id="d3944-134">String</span><span class="sxs-lookup"><span data-stu-id="d3944-134">String</span></span>|<span data-ttu-id="d3944-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d3944-135">Key of the entity.</span></span>|
|<span data-ttu-id="d3944-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="d3944-136">installStatus</span></span>|[<span data-ttu-id="d3944-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d3944-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="d3944-138">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="d3944-138">The installation status of the policy report.</span></span> <span data-ttu-id="d3944-139">可能的值是`success`： `available`、 `idle`、 `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `sharedDeviceUserLoggedInError`、、 `installing`、、、、、、、、、、、、。 `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation`</span><span class="sxs-lookup"><span data-stu-id="d3944-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="d3944-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="d3944-140">osVersion</span></span>|<span data-ttu-id="d3944-141">String</span><span class="sxs-lookup"><span data-stu-id="d3944-141">String</span></span>|<span data-ttu-id="d3944-142">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="d3944-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="d3944-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="d3944-143">deviceId</span></span>|<span data-ttu-id="d3944-144">String</span><span class="sxs-lookup"><span data-stu-id="d3944-144">String</span></span>|<span data-ttu-id="d3944-145">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="d3944-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="d3944-146">userId</span><span class="sxs-lookup"><span data-stu-id="d3944-146">userId</span></span>|<span data-ttu-id="d3944-147">String</span><span class="sxs-lookup"><span data-stu-id="d3944-147">String</span></span>|<span data-ttu-id="d3944-148">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d3944-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="d3944-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d3944-149">deviceDisplayName</span></span>|<span data-ttu-id="d3944-150">String</span><span class="sxs-lookup"><span data-stu-id="d3944-150">String</span></span>|<span data-ttu-id="d3944-151">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="d3944-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d3944-152">userName</span><span class="sxs-lookup"><span data-stu-id="d3944-152">userName</span></span>|<span data-ttu-id="d3944-153">String</span><span class="sxs-lookup"><span data-stu-id="d3944-153">String</span></span>|<span data-ttu-id="d3944-154">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="d3944-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="d3944-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d3944-155">deviceModel</span></span>|<span data-ttu-id="d3944-156">String</span><span class="sxs-lookup"><span data-stu-id="d3944-156">String</span></span>|<span data-ttu-id="d3944-157">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="d3944-157">The device model that is being reported</span></span>|
|<span data-ttu-id="d3944-158">platform</span><span class="sxs-lookup"><span data-stu-id="d3944-158">platform</span></span>|<span data-ttu-id="d3944-159">Int32</span><span class="sxs-lookup"><span data-stu-id="d3944-159">Int32</span></span>|<span data-ttu-id="d3944-160">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="d3944-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="d3944-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d3944-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d3944-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3944-162">DateTimeOffset</span></span>|<span data-ttu-id="d3944-163">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d3944-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d3944-164">status</span><span class="sxs-lookup"><span data-stu-id="d3944-164">status</span></span>|[<span data-ttu-id="d3944-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d3944-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d3944-166">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d3944-166">Compliance status of the policy report.</span></span> <span data-ttu-id="d3944-167">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d3944-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d3944-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3944-168">lastReportedDateTime</span></span>|<span data-ttu-id="d3944-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3944-169">DateTimeOffset</span></span>|<span data-ttu-id="d3944-170">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="d3944-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d3944-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d3944-171">userPrincipalName</span></span>|<span data-ttu-id="d3944-172">字符串</span><span class="sxs-lookup"><span data-stu-id="d3944-172">String</span></span>|<span data-ttu-id="d3944-173">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d3944-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d3944-174">响应</span><span class="sxs-lookup"><span data-stu-id="d3944-174">Response</span></span>
<span data-ttu-id="d3944-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3944-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3944-176">示例</span><span class="sxs-lookup"><span data-stu-id="d3944-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3944-177">请求</span><span class="sxs-lookup"><span data-stu-id="d3944-177">Request</span></span>
<span data-ttu-id="d3944-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3944-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3944-179">响应</span><span class="sxs-lookup"><span data-stu-id="d3944-179">Response</span></span>
<span data-ttu-id="d3944-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3944-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





