---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01f7f4f0216f11cc968cd147ca0b477add65eed9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452414"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="91967-103">创建 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="91967-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="91967-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91967-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91967-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91967-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91967-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91967-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91967-107">创建新的[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91967-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91967-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="91967-108">Prerequisites</span></span>
<span data-ttu-id="91967-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91967-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91967-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="91967-111">Permission type</span></span>|<span data-ttu-id="91967-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="91967-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91967-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91967-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91967-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91967-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="91967-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91967-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91967-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91967-116">Not supported.</span></span>|
|<span data-ttu-id="91967-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="91967-117">Application</span></span>|<span data-ttu-id="91967-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91967-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91967-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91967-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="91967-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="91967-120">Request headers</span></span>
|<span data-ttu-id="91967-121">标头</span><span class="sxs-lookup"><span data-stu-id="91967-121">Header</span></span>|<span data-ttu-id="91967-122">值</span><span class="sxs-lookup"><span data-stu-id="91967-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91967-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91967-123">Authorization</span></span>|<span data-ttu-id="91967-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91967-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91967-125">接受</span><span class="sxs-lookup"><span data-stu-id="91967-125">Accept</span></span>|<span data-ttu-id="91967-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91967-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91967-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="91967-127">Request body</span></span>
<span data-ttu-id="91967-128">在请求正文中，提供 windowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91967-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="91967-129">下表显示创建 windowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="91967-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="91967-130">属性</span><span class="sxs-lookup"><span data-stu-id="91967-130">Property</span></span>|<span data-ttu-id="91967-131">类型</span><span class="sxs-lookup"><span data-stu-id="91967-131">Type</span></span>|<span data-ttu-id="91967-132">说明</span><span class="sxs-lookup"><span data-stu-id="91967-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91967-133">id</span><span class="sxs-lookup"><span data-stu-id="91967-133">id</span></span>|<span data-ttu-id="91967-134">String</span><span class="sxs-lookup"><span data-stu-id="91967-134">String</span></span>|<span data-ttu-id="91967-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="91967-135">The GUID for the object</span></span>|
|<span data-ttu-id="91967-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="91967-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="91967-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="91967-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="91967-138">Windows autopilot 设备的配置文件分配状态。</span><span class="sxs-lookup"><span data-stu-id="91967-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="91967-139">可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="91967-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="91967-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="91967-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="91967-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="91967-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="91967-142">配置文件分配 Windows autopilot 设备的详细状态。</span><span class="sxs-lookup"><span data-stu-id="91967-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="91967-143">可取值为：`none`、`hardwareRequirementsNotMet`、`surfaceHubProfileNotSupported`、`holoLensProfileNotSupported`、`windowsPcProfileNotSupported`。</span><span class="sxs-lookup"><span data-stu-id="91967-143">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="91967-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="91967-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="91967-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91967-145">DateTimeOffset</span></span>|<span data-ttu-id="91967-146">Windows autopilot 设备的配置文件设置时间。</span><span class="sxs-lookup"><span data-stu-id="91967-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="91967-147">orderIdentifier</span></span>|<span data-ttu-id="91967-148">String</span><span class="sxs-lookup"><span data-stu-id="91967-148">String</span></span>|<span data-ttu-id="91967-149">Windows autopilot 设备的顺序标识符-已弃用</span><span class="sxs-lookup"><span data-stu-id="91967-149">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="91967-150">groupTag</span><span class="sxs-lookup"><span data-stu-id="91967-150">groupTag</span></span>|<span data-ttu-id="91967-151">String</span><span class="sxs-lookup"><span data-stu-id="91967-151">String</span></span>|<span data-ttu-id="91967-152">Windows autopilot 设备的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="91967-152">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-153">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="91967-153">purchaseOrderIdentifier</span></span>|<span data-ttu-id="91967-154">String</span><span class="sxs-lookup"><span data-stu-id="91967-154">String</span></span>|<span data-ttu-id="91967-155">Windows autopilot 设备的采购订单标识符。</span><span class="sxs-lookup"><span data-stu-id="91967-155">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-156">serialNumber</span><span class="sxs-lookup"><span data-stu-id="91967-156">serialNumber</span></span>|<span data-ttu-id="91967-157">String</span><span class="sxs-lookup"><span data-stu-id="91967-157">String</span></span>|<span data-ttu-id="91967-158">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="91967-158">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-159">productKey</span><span class="sxs-lookup"><span data-stu-id="91967-159">productKey</span></span>|<span data-ttu-id="91967-160">字符串</span><span class="sxs-lookup"><span data-stu-id="91967-160">String</span></span>|<span data-ttu-id="91967-161">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="91967-161">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="91967-162">manufacturer</span></span>|<span data-ttu-id="91967-163">String</span><span class="sxs-lookup"><span data-stu-id="91967-163">String</span></span>|<span data-ttu-id="91967-164">Windows autopilot 设备的 Oem 制造商。</span><span class="sxs-lookup"><span data-stu-id="91967-164">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-165">model</span><span class="sxs-lookup"><span data-stu-id="91967-165">model</span></span>|<span data-ttu-id="91967-166">String</span><span class="sxs-lookup"><span data-stu-id="91967-166">String</span></span>|<span data-ttu-id="91967-167">Windows autopilot 设备的模型名称。</span><span class="sxs-lookup"><span data-stu-id="91967-167">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="91967-168">enrollmentState</span></span>|[<span data-ttu-id="91967-169">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="91967-169">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="91967-170">Windows autopilot 设备的 Intune 注册状态。</span><span class="sxs-lookup"><span data-stu-id="91967-170">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="91967-171">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="91967-171">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="91967-172">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="91967-172">lastContactedDateTime</span></span>|<span data-ttu-id="91967-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91967-173">DateTimeOffset</span></span>|<span data-ttu-id="91967-174">Intune 上次联系 Windows autopilot 设备的日期时间。</span><span class="sxs-lookup"><span data-stu-id="91967-174">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="91967-175">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="91967-175">addressableUserName</span></span>|<span data-ttu-id="91967-176">String</span><span class="sxs-lookup"><span data-stu-id="91967-176">String</span></span>|<span data-ttu-id="91967-177">可寻址的用户名。</span><span class="sxs-lookup"><span data-stu-id="91967-177">Addressable user name.</span></span>|
|<span data-ttu-id="91967-178">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="91967-178">userPrincipalName</span></span>|<span data-ttu-id="91967-179">String</span><span class="sxs-lookup"><span data-stu-id="91967-179">String</span></span>|<span data-ttu-id="91967-180">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="91967-180">User Principal Name.</span></span>|
|<span data-ttu-id="91967-181">resourceName</span><span class="sxs-lookup"><span data-stu-id="91967-181">resourceName</span></span>|<span data-ttu-id="91967-182">String</span><span class="sxs-lookup"><span data-stu-id="91967-182">String</span></span>|<span data-ttu-id="91967-183">资源名称。</span><span class="sxs-lookup"><span data-stu-id="91967-183">Resource Name.</span></span>|
|<span data-ttu-id="91967-184">skuNumber</span><span class="sxs-lookup"><span data-stu-id="91967-184">skuNumber</span></span>|<span data-ttu-id="91967-185">String</span><span class="sxs-lookup"><span data-stu-id="91967-185">String</span></span>|<span data-ttu-id="91967-186">SKU 编号</span><span class="sxs-lookup"><span data-stu-id="91967-186">SKU Number</span></span>|
|<span data-ttu-id="91967-187">systemFamily</span><span class="sxs-lookup"><span data-stu-id="91967-187">systemFamily</span></span>|<span data-ttu-id="91967-188">String</span><span class="sxs-lookup"><span data-stu-id="91967-188">String</span></span>|<span data-ttu-id="91967-189">系统系列</span><span class="sxs-lookup"><span data-stu-id="91967-189">System Family</span></span>|
|<span data-ttu-id="91967-190">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="91967-190">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="91967-191">String</span><span class="sxs-lookup"><span data-stu-id="91967-191">String</span></span>|<span data-ttu-id="91967-192">AAD 设备 ID</span><span class="sxs-lookup"><span data-stu-id="91967-192">AAD Device ID</span></span>|
|<span data-ttu-id="91967-193">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="91967-193">managedDeviceId</span></span>|<span data-ttu-id="91967-194">String</span><span class="sxs-lookup"><span data-stu-id="91967-194">String</span></span>|<span data-ttu-id="91967-195">托管设备 ID</span><span class="sxs-lookup"><span data-stu-id="91967-195">Managed Device ID</span></span>|
|<span data-ttu-id="91967-196">displayName</span><span class="sxs-lookup"><span data-stu-id="91967-196">displayName</span></span>|<span data-ttu-id="91967-197">String</span><span class="sxs-lookup"><span data-stu-id="91967-197">String</span></span>|<span data-ttu-id="91967-198">显示名称</span><span class="sxs-lookup"><span data-stu-id="91967-198">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="91967-199">响应</span><span class="sxs-lookup"><span data-stu-id="91967-199">Response</span></span>
<span data-ttu-id="91967-200">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91967-200">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91967-201">示例</span><span class="sxs-lookup"><span data-stu-id="91967-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="91967-202">请求</span><span class="sxs-lookup"><span data-stu-id="91967-202">Request</span></span>
<span data-ttu-id="91967-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91967-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91967-204">响应</span><span class="sxs-lookup"><span data-stu-id="91967-204">Response</span></span>
<span data-ttu-id="91967-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91967-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



