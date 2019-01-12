---
title: 创建 iosUpdateDeviceStatus
description: 创建新的 iosUpdateDeviceStatus 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49ceef58c5f381fc89a4bff20c5ffa1274df0c15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934126"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="0ac8d-103">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="0ac8d-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="0ac8d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ac8d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ac8d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ac8d-107">创建新的 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ac8d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ac8d-108">Prerequisites</span></span>
<span data-ttu-id="0ac8d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0ac8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac8d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ac8d-111">Permission type</span></span>|<span data-ttu-id="0ac8d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ac8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ac8d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac8d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ac8d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac8d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ac8d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac8d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ac8d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-116">Not supported.</span></span>|
|<span data-ttu-id="0ac8d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ac8d-117">Application</span></span>|<span data-ttu-id="0ac8d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ac8d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ac8d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0ac8d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ac8d-120">Request headers</span></span>
|<span data-ttu-id="0ac8d-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ac8d-121">Header</span></span>|<span data-ttu-id="0ac8d-122">值</span><span class="sxs-lookup"><span data-stu-id="0ac8d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ac8d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac8d-123">Authorization</span></span>|<span data-ttu-id="0ac8d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ac8d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ac8d-125">Accept</span></span>|<span data-ttu-id="0ac8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ac8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac8d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ac8d-127">Request body</span></span>
<span data-ttu-id="0ac8d-128">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="0ac8d-129">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="0ac8d-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ac8d-130">Property</span></span>|<span data-ttu-id="0ac8d-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ac8d-131">Type</span></span>|<span data-ttu-id="0ac8d-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ac8d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ac8d-133">id</span><span class="sxs-lookup"><span data-stu-id="0ac8d-133">id</span></span>|<span data-ttu-id="0ac8d-134">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-134">String</span></span>|<span data-ttu-id="0ac8d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-135">Key of the entity.</span></span>|
|<span data-ttu-id="0ac8d-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="0ac8d-136">installStatus</span></span>|[<span data-ttu-id="0ac8d-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="0ac8d-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="0ac8d-138">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-138">The installation status of the policy report.</span></span> <span data-ttu-id="0ac8d-139">可能的值为： `success`， `available`， `idle`， `unknown`， `downloading`， `downloadFailed`， `downloadRequiresComputer`， `downloadInsufficientSpace`， `downloadInsufficientPower`， `downloadInsufficientNetwork`， `installing`， `installInsufficientSpace`， `installInsufficientPower`， `installPhoneCallInProgress`， `installFailed`， `notSupportedOperation`， `sharedDeviceUserLoggedInError`。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="0ac8d-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="0ac8d-140">osVersion</span></span>|<span data-ttu-id="0ac8d-141">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-141">String</span></span>|<span data-ttu-id="0ac8d-142">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="0ac8d-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="0ac8d-143">deviceId</span></span>|<span data-ttu-id="0ac8d-144">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-144">String</span></span>|<span data-ttu-id="0ac8d-145">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="0ac8d-146">userId</span><span class="sxs-lookup"><span data-stu-id="0ac8d-146">userId</span></span>|<span data-ttu-id="0ac8d-147">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-147">String</span></span>|<span data-ttu-id="0ac8d-148">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="0ac8d-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0ac8d-149">deviceDisplayName</span></span>|<span data-ttu-id="0ac8d-150">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-150">String</span></span>|<span data-ttu-id="0ac8d-151">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="0ac8d-152">userName</span><span class="sxs-lookup"><span data-stu-id="0ac8d-152">userName</span></span>|<span data-ttu-id="0ac8d-153">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-153">String</span></span>|<span data-ttu-id="0ac8d-154">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="0ac8d-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="0ac8d-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0ac8d-155">deviceModel</span></span>|<span data-ttu-id="0ac8d-156">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-156">String</span></span>|<span data-ttu-id="0ac8d-157">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="0ac8d-157">The device model that is being reported</span></span>|
|<span data-ttu-id="0ac8d-158">platform</span><span class="sxs-lookup"><span data-stu-id="0ac8d-158">platform</span></span>|<span data-ttu-id="0ac8d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac8d-159">Int32</span></span>|<span data-ttu-id="0ac8d-160">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="0ac8d-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="0ac8d-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac8d-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0ac8d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac8d-162">DateTimeOffset</span></span>|<span data-ttu-id="0ac8d-163">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="0ac8d-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0ac8d-164">status</span><span class="sxs-lookup"><span data-stu-id="0ac8d-164">status</span></span>|[<span data-ttu-id="0ac8d-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0ac8d-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0ac8d-166">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-166">Compliance status of the policy report.</span></span> <span data-ttu-id="0ac8d-167">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0ac8d-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac8d-168">lastReportedDateTime</span></span>|<span data-ttu-id="0ac8d-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac8d-169">DateTimeOffset</span></span>|<span data-ttu-id="0ac8d-170">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="0ac8d-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0ac8d-171">userPrincipalName</span></span>|<span data-ttu-id="0ac8d-172">String</span><span class="sxs-lookup"><span data-stu-id="0ac8d-172">String</span></span>|<span data-ttu-id="0ac8d-173">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="0ac8d-174">响应</span><span class="sxs-lookup"><span data-stu-id="0ac8d-174">Response</span></span>
<span data-ttu-id="0ac8d-175">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac8d-176">示例</span><span class="sxs-lookup"><span data-stu-id="0ac8d-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ac8d-177">请求</span><span class="sxs-lookup"><span data-stu-id="0ac8d-177">Request</span></span>
<span data-ttu-id="0ac8d-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ac8d-179">响应</span><span class="sxs-lookup"><span data-stu-id="0ac8d-179">Response</span></span>
<span data-ttu-id="0ac8d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ac8d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





