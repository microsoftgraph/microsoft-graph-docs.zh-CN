---
title: 创建 iosUpdateDeviceStatus
description: 创建新的 iosUpdateDeviceStatus 对象。
ms.openlocfilehash: 205bc02b37f3ba846e2fc7df0685d50fbd9e5279
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046353"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="ceac5-103">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="ceac5-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="ceac5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ceac5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ceac5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ceac5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ceac5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ceac5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceac5-107">创建新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceac5-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ceac5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ceac5-108">Prerequisites</span></span>
<span data-ttu-id="ceac5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ceac5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceac5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ceac5-111">Permission type</span></span>|<span data-ttu-id="ceac5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ceac5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceac5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ceac5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ceac5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceac5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ceac5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ceac5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceac5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ceac5-116">Not supported.</span></span>|
|<span data-ttu-id="ceac5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ceac5-117">Application</span></span>|<span data-ttu-id="ceac5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ceac5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceac5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ceac5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ceac5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ceac5-120">Request headers</span></span>
|<span data-ttu-id="ceac5-121">标头</span><span class="sxs-lookup"><span data-stu-id="ceac5-121">Header</span></span>|<span data-ttu-id="ceac5-122">值</span><span class="sxs-lookup"><span data-stu-id="ceac5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceac5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceac5-123">Authorization</span></span>|<span data-ttu-id="ceac5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ceac5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceac5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ceac5-125">Accept</span></span>|<span data-ttu-id="ceac5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ceac5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceac5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ceac5-127">Request body</span></span>
<span data-ttu-id="ceac5-128">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ceac5-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="ceac5-129">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ceac5-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="ceac5-130">属性</span><span class="sxs-lookup"><span data-stu-id="ceac5-130">Property</span></span>|<span data-ttu-id="ceac5-131">类型</span><span class="sxs-lookup"><span data-stu-id="ceac5-131">Type</span></span>|<span data-ttu-id="ceac5-132">说明</span><span class="sxs-lookup"><span data-stu-id="ceac5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceac5-133">id</span><span class="sxs-lookup"><span data-stu-id="ceac5-133">id</span></span>|<span data-ttu-id="ceac5-134">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-134">String</span></span>|<span data-ttu-id="ceac5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ceac5-135">Key of the entity.</span></span>|
|<span data-ttu-id="ceac5-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="ceac5-136">installStatus</span></span>|[<span data-ttu-id="ceac5-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ceac5-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="ceac5-138">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="ceac5-138">The installation status of the policy report.</span></span> <span data-ttu-id="ceac5-139">可能的值为： `success`， `available`， `idle`， `unknown`， `downloading`， `downloadFailed`， `downloadRequiresComputer`， `downloadInsufficientSpace`， `downloadInsufficientPower`， `downloadInsufficientNetwork`， `installing`， `installInsufficientSpace`， `installInsufficientPower`， `installPhoneCallInProgress`， `installFailed`， `notSupportedOperation`， `sharedDeviceUserLoggedInError`。</span><span class="sxs-lookup"><span data-stu-id="ceac5-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="ceac5-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="ceac5-140">osVersion</span></span>|<span data-ttu-id="ceac5-141">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-141">String</span></span>|<span data-ttu-id="ceac5-142">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="ceac5-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="ceac5-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="ceac5-143">deviceId</span></span>|<span data-ttu-id="ceac5-144">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-144">String</span></span>|<span data-ttu-id="ceac5-145">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="ceac5-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="ceac5-146">userId</span><span class="sxs-lookup"><span data-stu-id="ceac5-146">userId</span></span>|<span data-ttu-id="ceac5-147">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-147">String</span></span>|<span data-ttu-id="ceac5-148">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="ceac5-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="ceac5-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ceac5-149">deviceDisplayName</span></span>|<span data-ttu-id="ceac5-150">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-150">String</span></span>|<span data-ttu-id="ceac5-151">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="ceac5-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ceac5-152">userName</span><span class="sxs-lookup"><span data-stu-id="ceac5-152">userName</span></span>|<span data-ttu-id="ceac5-153">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-153">String</span></span>|<span data-ttu-id="ceac5-154">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="ceac5-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="ceac5-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ceac5-155">deviceModel</span></span>|<span data-ttu-id="ceac5-156">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-156">String</span></span>|<span data-ttu-id="ceac5-157">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="ceac5-157">The device model that is being reported</span></span>|
|<span data-ttu-id="ceac5-158">platform</span><span class="sxs-lookup"><span data-stu-id="ceac5-158">platform</span></span>|<span data-ttu-id="ceac5-159">Int32</span><span class="sxs-lookup"><span data-stu-id="ceac5-159">Int32</span></span>|<span data-ttu-id="ceac5-160">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="ceac5-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="ceac5-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ceac5-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ceac5-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceac5-162">DateTimeOffset</span></span>|<span data-ttu-id="ceac5-163">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="ceac5-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ceac5-164">状态</span><span class="sxs-lookup"><span data-stu-id="ceac5-164">status</span></span>|[<span data-ttu-id="ceac5-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ceac5-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ceac5-166">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="ceac5-166">Compliance status of the policy report.</span></span> <span data-ttu-id="ceac5-167">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="ceac5-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ceac5-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ceac5-168">lastReportedDateTime</span></span>|<span data-ttu-id="ceac5-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceac5-169">DateTimeOffset</span></span>|<span data-ttu-id="ceac5-170">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="ceac5-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ceac5-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ceac5-171">userPrincipalName</span></span>|<span data-ttu-id="ceac5-172">String</span><span class="sxs-lookup"><span data-stu-id="ceac5-172">String</span></span>|<span data-ttu-id="ceac5-173">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ceac5-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ceac5-174">响应</span><span class="sxs-lookup"><span data-stu-id="ceac5-174">Response</span></span>
<span data-ttu-id="ceac5-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceac5-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceac5-176">示例</span><span class="sxs-lookup"><span data-stu-id="ceac5-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="ceac5-177">请求</span><span class="sxs-lookup"><span data-stu-id="ceac5-177">Request</span></span>
<span data-ttu-id="ceac5-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ceac5-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ceac5-179">响应</span><span class="sxs-lookup"><span data-stu-id="ceac5-179">Response</span></span>
<span data-ttu-id="ceac5-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ceac5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





