---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0761094989125a9b5026fa4529eb3d5eb7f703b5
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160016"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="57fbd-103">创建 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="57fbd-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="57fbd-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57fbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57fbd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57fbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57fbd-106">创建新的[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="57fbd-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57fbd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="57fbd-107">Prerequisites</span></span>
<span data-ttu-id="57fbd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57fbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57fbd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="57fbd-110">Permission type</span></span>|<span data-ttu-id="57fbd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="57fbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57fbd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57fbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57fbd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57fbd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="57fbd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57fbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57fbd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57fbd-115">Not supported.</span></span>|
|<span data-ttu-id="57fbd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="57fbd-116">Application</span></span>|<span data-ttu-id="57fbd-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57fbd-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57fbd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57fbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="57fbd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="57fbd-119">Request headers</span></span>
|<span data-ttu-id="57fbd-120">标头</span><span class="sxs-lookup"><span data-stu-id="57fbd-120">Header</span></span>|<span data-ttu-id="57fbd-121">值</span><span class="sxs-lookup"><span data-stu-id="57fbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57fbd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57fbd-122">Authorization</span></span>|<span data-ttu-id="57fbd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="57fbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57fbd-124">接受</span><span class="sxs-lookup"><span data-stu-id="57fbd-124">Accept</span></span>|<span data-ttu-id="57fbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57fbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57fbd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="57fbd-126">Request body</span></span>
<span data-ttu-id="57fbd-127">在请求正文中，提供 windowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57fbd-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="57fbd-128">下表显示创建 windowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="57fbd-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="57fbd-129">属性</span><span class="sxs-lookup"><span data-stu-id="57fbd-129">Property</span></span>|<span data-ttu-id="57fbd-130">类型</span><span class="sxs-lookup"><span data-stu-id="57fbd-130">Type</span></span>|<span data-ttu-id="57fbd-131">说明</span><span class="sxs-lookup"><span data-stu-id="57fbd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57fbd-132">id</span><span class="sxs-lookup"><span data-stu-id="57fbd-132">id</span></span>|<span data-ttu-id="57fbd-133">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-133">String</span></span>|<span data-ttu-id="57fbd-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="57fbd-134">The GUID for the object</span></span>|
|<span data-ttu-id="57fbd-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="57fbd-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="57fbd-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="57fbd-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="57fbd-137">Windows autopilot 设备的配置文件分配状态。</span><span class="sxs-lookup"><span data-stu-id="57fbd-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="57fbd-138">可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="57fbd-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="57fbd-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="57fbd-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="57fbd-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="57fbd-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="57fbd-141">配置文件分配 Windows autopilot 设备的详细状态。</span><span class="sxs-lookup"><span data-stu-id="57fbd-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="57fbd-142">可取值为：`none`、`hardwareRequirementsNotMet`、`surfaceHubProfileNotSupported`、`holoLensProfileNotSupported`、`windowsPcProfileNotSupported`。</span><span class="sxs-lookup"><span data-stu-id="57fbd-142">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="57fbd-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="57fbd-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="57fbd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57fbd-144">DateTimeOffset</span></span>|<span data-ttu-id="57fbd-145">Windows autopilot 设备的配置文件设置时间。</span><span class="sxs-lookup"><span data-stu-id="57fbd-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="57fbd-146">orderIdentifier</span></span>|<span data-ttu-id="57fbd-147">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-147">String</span></span>|<span data-ttu-id="57fbd-148">Windows autopilot 设备的顺序标识符-已弃用</span><span class="sxs-lookup"><span data-stu-id="57fbd-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="57fbd-149">groupTag</span><span class="sxs-lookup"><span data-stu-id="57fbd-149">groupTag</span></span>|<span data-ttu-id="57fbd-150">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-150">String</span></span>|<span data-ttu-id="57fbd-151">Windows autopilot 设备的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="57fbd-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="57fbd-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="57fbd-153">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-153">String</span></span>|<span data-ttu-id="57fbd-154">Windows autopilot 设备的采购订单标识符。</span><span class="sxs-lookup"><span data-stu-id="57fbd-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="57fbd-155">serialNumber</span></span>|<span data-ttu-id="57fbd-156">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-156">String</span></span>|<span data-ttu-id="57fbd-157">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="57fbd-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-158">productKey</span><span class="sxs-lookup"><span data-stu-id="57fbd-158">productKey</span></span>|<span data-ttu-id="57fbd-159">字符串</span><span class="sxs-lookup"><span data-stu-id="57fbd-159">String</span></span>|<span data-ttu-id="57fbd-160">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="57fbd-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="57fbd-161">manufacturer</span></span>|<span data-ttu-id="57fbd-162">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-162">String</span></span>|<span data-ttu-id="57fbd-163">Windows autopilot 设备的 Oem 制造商。</span><span class="sxs-lookup"><span data-stu-id="57fbd-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-164">model</span><span class="sxs-lookup"><span data-stu-id="57fbd-164">model</span></span>|<span data-ttu-id="57fbd-165">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-165">String</span></span>|<span data-ttu-id="57fbd-166">Windows autopilot 设备的模型名称。</span><span class="sxs-lookup"><span data-stu-id="57fbd-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="57fbd-167">enrollmentState</span></span>|[<span data-ttu-id="57fbd-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="57fbd-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="57fbd-169">Windows autopilot 设备的 Intune 注册状态。</span><span class="sxs-lookup"><span data-stu-id="57fbd-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="57fbd-170">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="57fbd-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="57fbd-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="57fbd-171">lastContactedDateTime</span></span>|<span data-ttu-id="57fbd-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57fbd-172">DateTimeOffset</span></span>|<span data-ttu-id="57fbd-173">Intune 上次联系 Windows autopilot 设备的日期时间。</span><span class="sxs-lookup"><span data-stu-id="57fbd-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="57fbd-174">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="57fbd-174">addressableUserName</span></span>|<span data-ttu-id="57fbd-175">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-175">String</span></span>|<span data-ttu-id="57fbd-176">可寻址的用户名。</span><span class="sxs-lookup"><span data-stu-id="57fbd-176">Addressable user name.</span></span>|
|<span data-ttu-id="57fbd-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="57fbd-177">userPrincipalName</span></span>|<span data-ttu-id="57fbd-178">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-178">String</span></span>|<span data-ttu-id="57fbd-179">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="57fbd-179">User Principal Name.</span></span>|
|<span data-ttu-id="57fbd-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="57fbd-180">resourceName</span></span>|<span data-ttu-id="57fbd-181">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-181">String</span></span>|<span data-ttu-id="57fbd-182">资源名称。</span><span class="sxs-lookup"><span data-stu-id="57fbd-182">Resource Name.</span></span>|
|<span data-ttu-id="57fbd-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="57fbd-183">skuNumber</span></span>|<span data-ttu-id="57fbd-184">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-184">String</span></span>|<span data-ttu-id="57fbd-185">SKU 编号</span><span class="sxs-lookup"><span data-stu-id="57fbd-185">SKU Number</span></span>|
|<span data-ttu-id="57fbd-186">systemFamily</span><span class="sxs-lookup"><span data-stu-id="57fbd-186">systemFamily</span></span>|<span data-ttu-id="57fbd-187">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-187">String</span></span>|<span data-ttu-id="57fbd-188">系统系列</span><span class="sxs-lookup"><span data-stu-id="57fbd-188">System Family</span></span>|
|<span data-ttu-id="57fbd-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="57fbd-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="57fbd-190">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-190">String</span></span>|<span data-ttu-id="57fbd-191">AAD 设备 ID</span><span class="sxs-lookup"><span data-stu-id="57fbd-191">AAD Device ID</span></span>|
|<span data-ttu-id="57fbd-192">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="57fbd-192">managedDeviceId</span></span>|<span data-ttu-id="57fbd-193">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-193">String</span></span>|<span data-ttu-id="57fbd-194">托管设备 ID</span><span class="sxs-lookup"><span data-stu-id="57fbd-194">Managed Device ID</span></span>|
|<span data-ttu-id="57fbd-195">displayName</span><span class="sxs-lookup"><span data-stu-id="57fbd-195">displayName</span></span>|<span data-ttu-id="57fbd-196">String</span><span class="sxs-lookup"><span data-stu-id="57fbd-196">String</span></span>|<span data-ttu-id="57fbd-197">显示名称</span><span class="sxs-lookup"><span data-stu-id="57fbd-197">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="57fbd-198">响应</span><span class="sxs-lookup"><span data-stu-id="57fbd-198">Response</span></span>
<span data-ttu-id="57fbd-199">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="57fbd-199">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57fbd-200">示例</span><span class="sxs-lookup"><span data-stu-id="57fbd-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="57fbd-201">请求</span><span class="sxs-lookup"><span data-stu-id="57fbd-201">Request</span></span>
<span data-ttu-id="57fbd-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57fbd-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="57fbd-203">响应</span><span class="sxs-lookup"><span data-stu-id="57fbd-203">Response</span></span>
<span data-ttu-id="57fbd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57fbd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1124

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```





