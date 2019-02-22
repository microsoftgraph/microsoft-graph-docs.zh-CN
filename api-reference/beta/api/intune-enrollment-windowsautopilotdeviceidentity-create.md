---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d87a27c120f4866725e2f91828e8c267f655e69c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175302"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="0a86c-103">创建 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0a86c-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="0a86c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a86c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a86c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a86c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a86c-106">创建新的[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0a86c-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a86c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0a86c-107">Prerequisites</span></span>
<span data-ttu-id="0a86c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0a86c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0a86c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a86c-110">Permission type</span></span>|<span data-ttu-id="0a86c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0a86c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a86c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a86c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a86c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a86c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a86c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a86c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a86c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a86c-115">Not supported.</span></span>|
|<span data-ttu-id="0a86c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a86c-116">Application</span></span>|<span data-ttu-id="0a86c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a86c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a86c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a86c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="0a86c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a86c-119">Request headers</span></span>
|<span data-ttu-id="0a86c-120">标头</span><span class="sxs-lookup"><span data-stu-id="0a86c-120">Header</span></span>|<span data-ttu-id="0a86c-121">值</span><span class="sxs-lookup"><span data-stu-id="0a86c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a86c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a86c-122">Authorization</span></span>|<span data-ttu-id="0a86c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0a86c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a86c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0a86c-124">Accept</span></span>|<span data-ttu-id="0a86c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a86c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a86c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a86c-126">Request body</span></span>
<span data-ttu-id="0a86c-127">在请求正文中, 提供 windowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a86c-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="0a86c-128">下表显示创建 windowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0a86c-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="0a86c-129">属性</span><span class="sxs-lookup"><span data-stu-id="0a86c-129">Property</span></span>|<span data-ttu-id="0a86c-130">类型</span><span class="sxs-lookup"><span data-stu-id="0a86c-130">Type</span></span>|<span data-ttu-id="0a86c-131">说明</span><span class="sxs-lookup"><span data-stu-id="0a86c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a86c-132">id</span><span class="sxs-lookup"><span data-stu-id="0a86c-132">id</span></span>|<span data-ttu-id="0a86c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0a86c-133">String</span></span>|<span data-ttu-id="0a86c-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="0a86c-134">The GUID for the object</span></span>|
|<span data-ttu-id="0a86c-135">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="0a86c-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="0a86c-136">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="0a86c-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="0a86c-137">Windows autopilot 设备的配置文件分配状态。</span><span class="sxs-lookup"><span data-stu-id="0a86c-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="0a86c-138">可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="0a86c-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="0a86c-139">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="0a86c-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="0a86c-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="0a86c-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="0a86c-141">配置文件分配 Windows autopilot 设备的详细状态。</span><span class="sxs-lookup"><span data-stu-id="0a86c-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="0a86c-142">可取值为：`none`、`hardwareRequirementsNotMet`。</span><span class="sxs-lookup"><span data-stu-id="0a86c-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="0a86c-143">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a86c-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="0a86c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a86c-144">DateTimeOffset</span></span>|<span data-ttu-id="0a86c-145">Windows autopilot 设备的配置文件设置时间。</span><span class="sxs-lookup"><span data-stu-id="0a86c-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="0a86c-146">orderIdentifier</span></span>|<span data-ttu-id="0a86c-147">String</span><span class="sxs-lookup"><span data-stu-id="0a86c-147">String</span></span>|<span data-ttu-id="0a86c-148">Windows autopilot 设备的顺序标识符。</span><span class="sxs-lookup"><span data-stu-id="0a86c-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-149">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="0a86c-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="0a86c-150">字符串</span><span class="sxs-lookup"><span data-stu-id="0a86c-150">String</span></span>|<span data-ttu-id="0a86c-151">Windows autopilot 设备的采购订单标识符。</span><span class="sxs-lookup"><span data-stu-id="0a86c-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0a86c-152">serialNumber</span></span>|<span data-ttu-id="0a86c-153">String</span><span class="sxs-lookup"><span data-stu-id="0a86c-153">String</span></span>|<span data-ttu-id="0a86c-154">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="0a86c-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-155">productKey</span><span class="sxs-lookup"><span data-stu-id="0a86c-155">productKey</span></span>|<span data-ttu-id="0a86c-156">字符串</span><span class="sxs-lookup"><span data-stu-id="0a86c-156">String</span></span>|<span data-ttu-id="0a86c-157">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="0a86c-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-158">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0a86c-158">manufacturer</span></span>|<span data-ttu-id="0a86c-159">字符串</span><span class="sxs-lookup"><span data-stu-id="0a86c-159">String</span></span>|<span data-ttu-id="0a86c-160">Windows autopilot 设备的 Oem 制造商。</span><span class="sxs-lookup"><span data-stu-id="0a86c-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-161">model</span><span class="sxs-lookup"><span data-stu-id="0a86c-161">model</span></span>|<span data-ttu-id="0a86c-162">String</span><span class="sxs-lookup"><span data-stu-id="0a86c-162">String</span></span>|<span data-ttu-id="0a86c-163">Windows autopilot 设备的模型名称。</span><span class="sxs-lookup"><span data-stu-id="0a86c-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0a86c-164">enrollmentState</span></span>|[<span data-ttu-id="0a86c-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="0a86c-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="0a86c-166">Windows autopilot 设备的 Intune 注册状态。</span><span class="sxs-lookup"><span data-stu-id="0a86c-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="0a86c-167">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="0a86c-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="0a86c-168">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a86c-168">lastContactedDateTime</span></span>|<span data-ttu-id="0a86c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a86c-169">DateTimeOffset</span></span>|<span data-ttu-id="0a86c-170">Intune 上次联系 Windows autopilot 设备的日期时间。</span><span class="sxs-lookup"><span data-stu-id="0a86c-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0a86c-171">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="0a86c-171">addressableUserName</span></span>|<span data-ttu-id="0a86c-172">字符串</span><span class="sxs-lookup"><span data-stu-id="0a86c-172">String</span></span>|<span data-ttu-id="0a86c-173">可寻址的用户名。</span><span class="sxs-lookup"><span data-stu-id="0a86c-173">Addressable user name.</span></span>|
|<span data-ttu-id="0a86c-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a86c-174">userPrincipalName</span></span>|<span data-ttu-id="0a86c-175">字符串</span><span class="sxs-lookup"><span data-stu-id="0a86c-175">String</span></span>|<span data-ttu-id="0a86c-176">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="0a86c-176">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="0a86c-177">响应</span><span class="sxs-lookup"><span data-stu-id="0a86c-177">Response</span></span>
<span data-ttu-id="0a86c-178">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0a86c-178">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a86c-179">示例</span><span class="sxs-lookup"><span data-stu-id="0a86c-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a86c-180">请求</span><span class="sxs-lookup"><span data-stu-id="0a86c-180">Request</span></span>
<span data-ttu-id="0a86c-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a86c-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a86c-182">响应</span><span class="sxs-lookup"><span data-stu-id="0a86c-182">Response</span></span>
<span data-ttu-id="0a86c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a86c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




