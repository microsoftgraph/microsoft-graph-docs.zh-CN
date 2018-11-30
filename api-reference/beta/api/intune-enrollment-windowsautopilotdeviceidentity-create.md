---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
ms.openlocfilehash: 9a68b5db287732add986bc703668c75b9245f962
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046536"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="f94c7-103">创建 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f94c7-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="f94c7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f94c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f94c7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f94c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f94c7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f94c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f94c7-107">创建新的[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f94c7-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f94c7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f94c7-108">Prerequisites</span></span>
<span data-ttu-id="f94c7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f94c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f94c7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f94c7-111">Permission type</span></span>|<span data-ttu-id="f94c7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f94c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f94c7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f94c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f94c7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f94c7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f94c7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f94c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f94c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f94c7-116">Not supported.</span></span>|
|<span data-ttu-id="f94c7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f94c7-117">Application</span></span>|<span data-ttu-id="f94c7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f94c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f94c7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f94c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="f94c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f94c7-120">Request headers</span></span>
|<span data-ttu-id="f94c7-121">标头</span><span class="sxs-lookup"><span data-stu-id="f94c7-121">Header</span></span>|<span data-ttu-id="f94c7-122">值</span><span class="sxs-lookup"><span data-stu-id="f94c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f94c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f94c7-123">Authorization</span></span>|<span data-ttu-id="f94c7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f94c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f94c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f94c7-125">Accept</span></span>|<span data-ttu-id="f94c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f94c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f94c7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f94c7-127">Request body</span></span>
<span data-ttu-id="f94c7-128">在请求正文中，提供 windowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f94c7-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="f94c7-129">下表显示时创建 windowsAutopilotDeviceIdentity 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f94c7-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="f94c7-130">属性</span><span class="sxs-lookup"><span data-stu-id="f94c7-130">Property</span></span>|<span data-ttu-id="f94c7-131">类型</span><span class="sxs-lookup"><span data-stu-id="f94c7-131">Type</span></span>|<span data-ttu-id="f94c7-132">说明</span><span class="sxs-lookup"><span data-stu-id="f94c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f94c7-133">id</span><span class="sxs-lookup"><span data-stu-id="f94c7-133">id</span></span>|<span data-ttu-id="f94c7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f94c7-134">String</span></span>|<span data-ttu-id="f94c7-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="f94c7-135">The GUID for the object</span></span>|
|<span data-ttu-id="f94c7-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="f94c7-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="f94c7-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="f94c7-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="f94c7-138">配置文件 Windows 自动执行某些操作设备的工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="f94c7-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="f94c7-139">可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="f94c7-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="f94c7-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="f94c7-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="f94c7-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="f94c7-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="f94c7-142">配置文件分配详细 Windows 自动执行某些操作设备的状态。</span><span class="sxs-lookup"><span data-stu-id="f94c7-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="f94c7-143">可取值为：`none`、`hardwareRequirementsNotMet`。</span><span class="sxs-lookup"><span data-stu-id="f94c7-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="f94c7-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="f94c7-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="f94c7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f94c7-145">DateTimeOffset</span></span>|<span data-ttu-id="f94c7-146">配置文件设置的 Windows 自动执行某些操作设备的时间。</span><span class="sxs-lookup"><span data-stu-id="f94c7-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="f94c7-147">orderIdentifier</span></span>|<span data-ttu-id="f94c7-148">字符串</span><span class="sxs-lookup"><span data-stu-id="f94c7-148">String</span></span>|<span data-ttu-id="f94c7-149">Windows 自动执行某些操作设备的顺序标识符。</span><span class="sxs-lookup"><span data-stu-id="f94c7-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="f94c7-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="f94c7-151">字符串</span><span class="sxs-lookup"><span data-stu-id="f94c7-151">String</span></span>|<span data-ttu-id="f94c7-152">采购订单的 Windows 自动执行某些操作设备的标识符。</span><span class="sxs-lookup"><span data-stu-id="f94c7-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f94c7-153">serialNumber</span></span>|<span data-ttu-id="f94c7-154">字符串</span><span class="sxs-lookup"><span data-stu-id="f94c7-154">String</span></span>|<span data-ttu-id="f94c7-155">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="f94c7-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-156">productKey</span><span class="sxs-lookup"><span data-stu-id="f94c7-156">productKey</span></span>|<span data-ttu-id="f94c7-157">字符串</span><span class="sxs-lookup"><span data-stu-id="f94c7-157">String</span></span>|<span data-ttu-id="f94c7-158">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="f94c7-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f94c7-159">manufacturer</span></span>|<span data-ttu-id="f94c7-160">String</span><span class="sxs-lookup"><span data-stu-id="f94c7-160">String</span></span>|<span data-ttu-id="f94c7-161">Oem 的 Windows 自动执行某些操作设备的制造商。</span><span class="sxs-lookup"><span data-stu-id="f94c7-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-162">model</span><span class="sxs-lookup"><span data-stu-id="f94c7-162">model</span></span>|<span data-ttu-id="f94c7-163">String</span><span class="sxs-lookup"><span data-stu-id="f94c7-163">String</span></span>|<span data-ttu-id="f94c7-164">模型的 Windows 自动执行某些操作设备的名称。</span><span class="sxs-lookup"><span data-stu-id="f94c7-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f94c7-165">enrollmentState</span></span>|[<span data-ttu-id="f94c7-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f94c7-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f94c7-167">Windows 自动执行某些操作设备 Intune 注册状态。</span><span class="sxs-lookup"><span data-stu-id="f94c7-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="f94c7-168">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="f94c7-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f94c7-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f94c7-169">lastContactedDateTime</span></span>|<span data-ttu-id="f94c7-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f94c7-170">DateTimeOffset</span></span>|<span data-ttu-id="f94c7-171">Intune 上次联系日期时间的 Windows 自动执行某些操作设备。</span><span class="sxs-lookup"><span data-stu-id="f94c7-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="f94c7-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="f94c7-172">addressableUserName</span></span>|<span data-ttu-id="f94c7-173">字符串</span><span class="sxs-lookup"><span data-stu-id="f94c7-173">String</span></span>|<span data-ttu-id="f94c7-174">可寻址用户名。</span><span class="sxs-lookup"><span data-stu-id="f94c7-174">Addressable user name.</span></span>|
|<span data-ttu-id="f94c7-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f94c7-175">userPrincipalName</span></span>|<span data-ttu-id="f94c7-176">字符串</span><span class="sxs-lookup"><span data-stu-id="f94c7-176">String</span></span>|<span data-ttu-id="f94c7-177">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="f94c7-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="f94c7-178">响应</span><span class="sxs-lookup"><span data-stu-id="f94c7-178">Response</span></span>
<span data-ttu-id="f94c7-179">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f94c7-179">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f94c7-180">示例</span><span class="sxs-lookup"><span data-stu-id="f94c7-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="f94c7-181">请求</span><span class="sxs-lookup"><span data-stu-id="f94c7-181">Request</span></span>
<span data-ttu-id="f94c7-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f94c7-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 755

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="f94c7-183">响应</span><span class="sxs-lookup"><span data-stu-id="f94c7-183">Response</span></span>
<span data-ttu-id="f94c7-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f94c7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 804

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value"
}
```





