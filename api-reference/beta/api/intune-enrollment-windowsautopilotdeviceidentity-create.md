---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 725d6d5c0cb0f03c9fcb1b2c161959a4242e2a13
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153851"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="44d46-103">创建 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="44d46-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="44d46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44d46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44d46-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44d46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44d46-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44d46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44d46-107">创建新的 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44d46-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44d46-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44d46-108">Prerequisites</span></span>
<span data-ttu-id="44d46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44d46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44d46-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44d46-111">Permission type</span></span>|<span data-ttu-id="44d46-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44d46-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44d46-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44d46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44d46-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d46-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="44d46-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44d46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44d46-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44d46-116">Not supported.</span></span>|
|<span data-ttu-id="44d46-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="44d46-117">Application</span></span>|<span data-ttu-id="44d46-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d46-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44d46-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44d46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="44d46-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44d46-120">Request headers</span></span>
|<span data-ttu-id="44d46-121">标头</span><span class="sxs-lookup"><span data-stu-id="44d46-121">Header</span></span>|<span data-ttu-id="44d46-122">值</span><span class="sxs-lookup"><span data-stu-id="44d46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44d46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44d46-123">Authorization</span></span>|<span data-ttu-id="44d46-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44d46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44d46-125">接受</span><span class="sxs-lookup"><span data-stu-id="44d46-125">Accept</span></span>|<span data-ttu-id="44d46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44d46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44d46-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44d46-127">Request body</span></span>
<span data-ttu-id="44d46-128">在请求正文中，提供 windowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44d46-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="44d46-129">下表显示创建 windowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44d46-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="44d46-130">属性</span><span class="sxs-lookup"><span data-stu-id="44d46-130">Property</span></span>|<span data-ttu-id="44d46-131">类型</span><span class="sxs-lookup"><span data-stu-id="44d46-131">Type</span></span>|<span data-ttu-id="44d46-132">说明</span><span class="sxs-lookup"><span data-stu-id="44d46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d46-133">id</span><span class="sxs-lookup"><span data-stu-id="44d46-133">id</span></span>|<span data-ttu-id="44d46-134">String</span><span class="sxs-lookup"><span data-stu-id="44d46-134">String</span></span>|<span data-ttu-id="44d46-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="44d46-135">The GUID for the object</span></span>|
|<span data-ttu-id="44d46-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="44d46-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="44d46-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="44d46-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="44d46-138">Windows Autopilot 设备的配置文件分配状态。</span><span class="sxs-lookup"><span data-stu-id="44d46-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="44d46-139">可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="44d46-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="44d46-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="44d46-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="44d46-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="44d46-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="44d46-142">配置文件分配 Windows Autopilot 设备的详细状态。</span><span class="sxs-lookup"><span data-stu-id="44d46-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="44d46-143">可取值为：`none`、`hardwareRequirementsNotMet`、`surfaceHubProfileNotSupported`、`holoLensProfileNotSupported`、`windowsPcProfileNotSupported`。</span><span class="sxs-lookup"><span data-stu-id="44d46-143">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="44d46-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="44d46-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="44d46-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44d46-145">DateTimeOffset</span></span>|<span data-ttu-id="44d46-146">Windows Autopilot 设备的配置文件设置时间。</span><span class="sxs-lookup"><span data-stu-id="44d46-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-147">groupTag</span><span class="sxs-lookup"><span data-stu-id="44d46-147">groupTag</span></span>|<span data-ttu-id="44d46-148">String</span><span class="sxs-lookup"><span data-stu-id="44d46-148">String</span></span>|<span data-ttu-id="44d46-149">Windows autopilot 设备的组标记。</span><span class="sxs-lookup"><span data-stu-id="44d46-149">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="44d46-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="44d46-151">String</span><span class="sxs-lookup"><span data-stu-id="44d46-151">String</span></span>|<span data-ttu-id="44d46-152">Purchase Order Windows autopilot 设备的标识符。</span><span class="sxs-lookup"><span data-stu-id="44d46-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="44d46-153">serialNumber</span></span>|<span data-ttu-id="44d46-154">String</span><span class="sxs-lookup"><span data-stu-id="44d46-154">String</span></span>|<span data-ttu-id="44d46-155">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="44d46-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-156">productKey</span><span class="sxs-lookup"><span data-stu-id="44d46-156">productKey</span></span>|<span data-ttu-id="44d46-157">String</span><span class="sxs-lookup"><span data-stu-id="44d46-157">String</span></span>|<span data-ttu-id="44d46-158">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="44d46-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="44d46-159">manufacturer</span></span>|<span data-ttu-id="44d46-160">String</span><span class="sxs-lookup"><span data-stu-id="44d46-160">String</span></span>|<span data-ttu-id="44d46-161">Windows autopilot 设备的 Oem 制造商。</span><span class="sxs-lookup"><span data-stu-id="44d46-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-162">model</span><span class="sxs-lookup"><span data-stu-id="44d46-162">model</span></span>|<span data-ttu-id="44d46-163">String</span><span class="sxs-lookup"><span data-stu-id="44d46-163">String</span></span>|<span data-ttu-id="44d46-164">Windows autopilot 设备的型号名称。</span><span class="sxs-lookup"><span data-stu-id="44d46-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="44d46-165">enrollmentState</span></span>|[<span data-ttu-id="44d46-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="44d46-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="44d46-167">Windows Autopilot 设备的 Intune 注册状态。</span><span class="sxs-lookup"><span data-stu-id="44d46-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="44d46-168">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="44d46-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="44d46-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="44d46-169">lastContactedDateTime</span></span>|<span data-ttu-id="44d46-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44d46-170">DateTimeOffset</span></span>|<span data-ttu-id="44d46-171">Intune Windows Autopilot 设备的上次联系日期时间。</span><span class="sxs-lookup"><span data-stu-id="44d46-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="44d46-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="44d46-172">addressableUserName</span></span>|<span data-ttu-id="44d46-173">String</span><span class="sxs-lookup"><span data-stu-id="44d46-173">String</span></span>|<span data-ttu-id="44d46-174">可地址用户名。</span><span class="sxs-lookup"><span data-stu-id="44d46-174">Addressable user name.</span></span>|
|<span data-ttu-id="44d46-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44d46-175">userPrincipalName</span></span>|<span data-ttu-id="44d46-176">String</span><span class="sxs-lookup"><span data-stu-id="44d46-176">String</span></span>|<span data-ttu-id="44d46-177">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="44d46-177">User Principal Name.</span></span>|
|<span data-ttu-id="44d46-178">resourceName</span><span class="sxs-lookup"><span data-stu-id="44d46-178">resourceName</span></span>|<span data-ttu-id="44d46-179">String</span><span class="sxs-lookup"><span data-stu-id="44d46-179">String</span></span>|<span data-ttu-id="44d46-180">资源名称。</span><span class="sxs-lookup"><span data-stu-id="44d46-180">Resource Name.</span></span>|
|<span data-ttu-id="44d46-181">skuNumber</span><span class="sxs-lookup"><span data-stu-id="44d46-181">skuNumber</span></span>|<span data-ttu-id="44d46-182">String</span><span class="sxs-lookup"><span data-stu-id="44d46-182">String</span></span>|<span data-ttu-id="44d46-183">SKU 号</span><span class="sxs-lookup"><span data-stu-id="44d46-183">SKU Number</span></span>|
|<span data-ttu-id="44d46-184">systemFamily</span><span class="sxs-lookup"><span data-stu-id="44d46-184">systemFamily</span></span>|<span data-ttu-id="44d46-185">String</span><span class="sxs-lookup"><span data-stu-id="44d46-185">String</span></span>|<span data-ttu-id="44d46-186">系统系列</span><span class="sxs-lookup"><span data-stu-id="44d46-186">System Family</span></span>|
|<span data-ttu-id="44d46-187">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="44d46-187">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="44d46-188">String</span><span class="sxs-lookup"><span data-stu-id="44d46-188">String</span></span>|<span data-ttu-id="44d46-189">AAD 设备 ID - 已弃用</span><span class="sxs-lookup"><span data-stu-id="44d46-189">AAD Device ID - to be deprecated</span></span>|
|<span data-ttu-id="44d46-190">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="44d46-190">azureAdDeviceId</span></span>|<span data-ttu-id="44d46-191">String</span><span class="sxs-lookup"><span data-stu-id="44d46-191">String</span></span>|<span data-ttu-id="44d46-192">AAD 设备 ID</span><span class="sxs-lookup"><span data-stu-id="44d46-192">AAD Device ID</span></span>|
|<span data-ttu-id="44d46-193">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="44d46-193">managedDeviceId</span></span>|<span data-ttu-id="44d46-194">String</span><span class="sxs-lookup"><span data-stu-id="44d46-194">String</span></span>|<span data-ttu-id="44d46-195">托管设备 ID</span><span class="sxs-lookup"><span data-stu-id="44d46-195">Managed Device ID</span></span>|
|<span data-ttu-id="44d46-196">displayName</span><span class="sxs-lookup"><span data-stu-id="44d46-196">displayName</span></span>|<span data-ttu-id="44d46-197">String</span><span class="sxs-lookup"><span data-stu-id="44d46-197">String</span></span>|<span data-ttu-id="44d46-198">显示名称</span><span class="sxs-lookup"><span data-stu-id="44d46-198">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="44d46-199">响应</span><span class="sxs-lookup"><span data-stu-id="44d46-199">Response</span></span>
<span data-ttu-id="44d46-200">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44d46-200">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44d46-201">示例</span><span class="sxs-lookup"><span data-stu-id="44d46-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="44d46-202">请求</span><span class="sxs-lookup"><span data-stu-id="44d46-202">Request</span></span>
<span data-ttu-id="44d46-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44d46-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1077

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
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
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="44d46-204">响应</span><span class="sxs-lookup"><span data-stu-id="44d46-204">Response</span></span>
<span data-ttu-id="44d46-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44d46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
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
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```




