---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66b63566dcd7ca2b498e60e0a5e403492e37eeb9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356079"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="208b4-103">创建 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="208b4-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="208b4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="208b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="208b4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="208b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="208b4-106">创建新的[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="208b4-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="208b4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="208b4-107">Prerequisites</span></span>
<span data-ttu-id="208b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="208b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="208b4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="208b4-110">Permission type</span></span>|<span data-ttu-id="208b4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="208b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="208b4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="208b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="208b4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="208b4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="208b4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="208b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="208b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="208b4-115">Not supported.</span></span>|
|<span data-ttu-id="208b4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="208b4-116">Application</span></span>|<span data-ttu-id="208b4-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="208b4-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="208b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="208b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="208b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="208b4-119">Request headers</span></span>
|<span data-ttu-id="208b4-120">标头</span><span class="sxs-lookup"><span data-stu-id="208b4-120">Header</span></span>|<span data-ttu-id="208b4-121">值</span><span class="sxs-lookup"><span data-stu-id="208b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="208b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="208b4-122">Authorization</span></span>|<span data-ttu-id="208b4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="208b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="208b4-124">接受</span><span class="sxs-lookup"><span data-stu-id="208b4-124">Accept</span></span>|<span data-ttu-id="208b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="208b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="208b4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="208b4-126">Request body</span></span>
<span data-ttu-id="208b4-127">在请求正文中, 提供 windowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="208b4-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="208b4-128">下表显示创建 windowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="208b4-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="208b4-129">属性</span><span class="sxs-lookup"><span data-stu-id="208b4-129">Property</span></span>|<span data-ttu-id="208b4-130">类型</span><span class="sxs-lookup"><span data-stu-id="208b4-130">Type</span></span>|<span data-ttu-id="208b4-131">说明</span><span class="sxs-lookup"><span data-stu-id="208b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="208b4-132">id</span><span class="sxs-lookup"><span data-stu-id="208b4-132">id</span></span>|<span data-ttu-id="208b4-133">String</span><span class="sxs-lookup"><span data-stu-id="208b4-133">String</span></span>|<span data-ttu-id="208b4-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="208b4-134">The GUID for the object</span></span>|
|<span data-ttu-id="208b4-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="208b4-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="208b4-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="208b4-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="208b4-137">Windows autopilot 设备的配置文件分配状态。</span><span class="sxs-lookup"><span data-stu-id="208b4-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="208b4-138">可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="208b4-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="208b4-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="208b4-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="208b4-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="208b4-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="208b4-141">配置文件分配 Windows autopilot 设备的详细状态。</span><span class="sxs-lookup"><span data-stu-id="208b4-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="208b4-142">可取值为：`none`、`hardwareRequirementsNotMet`。</span><span class="sxs-lookup"><span data-stu-id="208b4-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="208b4-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="208b4-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="208b4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="208b4-144">DateTimeOffset</span></span>|<span data-ttu-id="208b4-145">Windows autopilot 设备的配置文件设置时间。</span><span class="sxs-lookup"><span data-stu-id="208b4-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="208b4-146">orderIdentifier</span></span>|<span data-ttu-id="208b4-147">String</span><span class="sxs-lookup"><span data-stu-id="208b4-147">String</span></span>|<span data-ttu-id="208b4-148">Windows autopilot 设备的顺序标识符-已弃用</span><span class="sxs-lookup"><span data-stu-id="208b4-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="208b4-149">groupTag</span><span class="sxs-lookup"><span data-stu-id="208b4-149">groupTag</span></span>|<span data-ttu-id="208b4-150">String</span><span class="sxs-lookup"><span data-stu-id="208b4-150">String</span></span>|<span data-ttu-id="208b4-151">Windows autopilot 设备的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="208b4-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-152">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="208b4-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="208b4-153">String</span><span class="sxs-lookup"><span data-stu-id="208b4-153">String</span></span>|<span data-ttu-id="208b4-154">Windows autopilot 设备的采购订单标识符。</span><span class="sxs-lookup"><span data-stu-id="208b4-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="208b4-155">serialNumber</span></span>|<span data-ttu-id="208b4-156">String</span><span class="sxs-lookup"><span data-stu-id="208b4-156">String</span></span>|<span data-ttu-id="208b4-157">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="208b4-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-158">productKey</span><span class="sxs-lookup"><span data-stu-id="208b4-158">productKey</span></span>|<span data-ttu-id="208b4-159">字符串</span><span class="sxs-lookup"><span data-stu-id="208b4-159">String</span></span>|<span data-ttu-id="208b4-160">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="208b4-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="208b4-161">manufacturer</span></span>|<span data-ttu-id="208b4-162">String</span><span class="sxs-lookup"><span data-stu-id="208b4-162">String</span></span>|<span data-ttu-id="208b4-163">Windows autopilot 设备的 Oem 制造商。</span><span class="sxs-lookup"><span data-stu-id="208b4-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-164">model</span><span class="sxs-lookup"><span data-stu-id="208b4-164">model</span></span>|<span data-ttu-id="208b4-165">String</span><span class="sxs-lookup"><span data-stu-id="208b4-165">String</span></span>|<span data-ttu-id="208b4-166">Windows autopilot 设备的模型名称。</span><span class="sxs-lookup"><span data-stu-id="208b4-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="208b4-167">enrollmentState</span></span>|[<span data-ttu-id="208b4-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="208b4-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="208b4-169">Windows autopilot 设备的 Intune 注册状态。</span><span class="sxs-lookup"><span data-stu-id="208b4-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="208b4-170">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="208b4-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="208b4-171">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="208b4-171">lastContactedDateTime</span></span>|<span data-ttu-id="208b4-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="208b4-172">DateTimeOffset</span></span>|<span data-ttu-id="208b4-173">Intune 上次联系 Windows autopilot 设备的日期时间。</span><span class="sxs-lookup"><span data-stu-id="208b4-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="208b4-174">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="208b4-174">addressableUserName</span></span>|<span data-ttu-id="208b4-175">String</span><span class="sxs-lookup"><span data-stu-id="208b4-175">String</span></span>|<span data-ttu-id="208b4-176">可寻址的用户名。</span><span class="sxs-lookup"><span data-stu-id="208b4-176">Addressable user name.</span></span>|
|<span data-ttu-id="208b4-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="208b4-177">userPrincipalName</span></span>|<span data-ttu-id="208b4-178">String</span><span class="sxs-lookup"><span data-stu-id="208b4-178">String</span></span>|<span data-ttu-id="208b4-179">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="208b4-179">User Principal Name.</span></span>|
|<span data-ttu-id="208b4-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="208b4-180">resourceName</span></span>|<span data-ttu-id="208b4-181">String</span><span class="sxs-lookup"><span data-stu-id="208b4-181">String</span></span>|<span data-ttu-id="208b4-182">资源名称。</span><span class="sxs-lookup"><span data-stu-id="208b4-182">Resource Name.</span></span>|
|<span data-ttu-id="208b4-183">skuNumber</span><span class="sxs-lookup"><span data-stu-id="208b4-183">skuNumber</span></span>|<span data-ttu-id="208b4-184">String</span><span class="sxs-lookup"><span data-stu-id="208b4-184">String</span></span>|<span data-ttu-id="208b4-185">SKU 编号</span><span class="sxs-lookup"><span data-stu-id="208b4-185">SKU Number</span></span>|
|<span data-ttu-id="208b4-186">systemFamily</span><span class="sxs-lookup"><span data-stu-id="208b4-186">systemFamily</span></span>|<span data-ttu-id="208b4-187">String</span><span class="sxs-lookup"><span data-stu-id="208b4-187">String</span></span>|<span data-ttu-id="208b4-188">系统系列</span><span class="sxs-lookup"><span data-stu-id="208b4-188">System Family</span></span>|
|<span data-ttu-id="208b4-189">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="208b4-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="208b4-190">String</span><span class="sxs-lookup"><span data-stu-id="208b4-190">String</span></span>|<span data-ttu-id="208b4-191">AAD 设备 ID</span><span class="sxs-lookup"><span data-stu-id="208b4-191">AAD Device ID</span></span>|
|<span data-ttu-id="208b4-192">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="208b4-192">managedDeviceId</span></span>|<span data-ttu-id="208b4-193">String</span><span class="sxs-lookup"><span data-stu-id="208b4-193">String</span></span>|<span data-ttu-id="208b4-194">托管设备 ID</span><span class="sxs-lookup"><span data-stu-id="208b4-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="208b4-195">响应</span><span class="sxs-lookup"><span data-stu-id="208b4-195">Response</span></span>
<span data-ttu-id="208b4-196">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="208b4-196">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="208b4-197">示例</span><span class="sxs-lookup"><span data-stu-id="208b4-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="208b4-198">请求</span><span class="sxs-lookup"><span data-stu-id="208b4-198">Request</span></span>
<span data-ttu-id="208b4-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="208b4-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1035

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
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="208b4-200">响应</span><span class="sxs-lookup"><span data-stu-id="208b4-200">Response</span></span>
<span data-ttu-id="208b4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="208b4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1084

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
  "managedDeviceId": "Managed Device Id value"
}
```






