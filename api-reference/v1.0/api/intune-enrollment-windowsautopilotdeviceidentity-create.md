---
title: 创建 windowsAutopilotDeviceIdentity
description: 创建新的 windowsAutopilotDeviceIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ee59ca45db337f85f1c4f0f01443c2c0965e1c0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753002"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="d0624-103">创建 windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d0624-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="d0624-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0624-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0624-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0624-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0624-106">创建新的 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0624-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0624-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0624-107">Prerequisites</span></span>
<span data-ttu-id="d0624-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0624-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0624-110">Permission type</span></span>|<span data-ttu-id="d0624-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0624-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0624-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0624-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0624-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0624-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d0624-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0624-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0624-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0624-115">Not supported.</span></span>|
|<span data-ttu-id="d0624-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0624-116">Application</span></span>|<span data-ttu-id="d0624-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0624-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0624-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0624-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="d0624-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0624-119">Request headers</span></span>
|<span data-ttu-id="d0624-120">标头</span><span class="sxs-lookup"><span data-stu-id="d0624-120">Header</span></span>|<span data-ttu-id="d0624-121">值</span><span class="sxs-lookup"><span data-stu-id="d0624-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0624-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0624-122">Authorization</span></span>|<span data-ttu-id="d0624-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0624-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0624-124">接受</span><span class="sxs-lookup"><span data-stu-id="d0624-124">Accept</span></span>|<span data-ttu-id="d0624-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0624-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0624-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0624-126">Request body</span></span>
<span data-ttu-id="d0624-127">在请求正文中，提供 windowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0624-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="d0624-128">下表显示创建 windowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d0624-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="d0624-129">属性</span><span class="sxs-lookup"><span data-stu-id="d0624-129">Property</span></span>|<span data-ttu-id="d0624-130">类型</span><span class="sxs-lookup"><span data-stu-id="d0624-130">Type</span></span>|<span data-ttu-id="d0624-131">说明</span><span class="sxs-lookup"><span data-stu-id="d0624-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0624-132">id</span><span class="sxs-lookup"><span data-stu-id="d0624-132">id</span></span>|<span data-ttu-id="d0624-133">String</span><span class="sxs-lookup"><span data-stu-id="d0624-133">String</span></span>|<span data-ttu-id="d0624-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="d0624-134">The GUID for the object</span></span>|
|<span data-ttu-id="d0624-135">groupTag</span><span class="sxs-lookup"><span data-stu-id="d0624-135">groupTag</span></span>|<span data-ttu-id="d0624-136">String</span><span class="sxs-lookup"><span data-stu-id="d0624-136">String</span></span>|<span data-ttu-id="d0624-137">autopilot Windows的 Group 标记。</span><span class="sxs-lookup"><span data-stu-id="d0624-137">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d0624-138">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="d0624-138">purchaseOrderIdentifier</span></span>|<span data-ttu-id="d0624-139">String</span><span class="sxs-lookup"><span data-stu-id="d0624-139">String</span></span>|<span data-ttu-id="d0624-140">Purchase Order Autopilot Windows标识符。</span><span class="sxs-lookup"><span data-stu-id="d0624-140">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d0624-141">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d0624-141">serialNumber</span></span>|<span data-ttu-id="d0624-142">String</span><span class="sxs-lookup"><span data-stu-id="d0624-142">String</span></span>|<span data-ttu-id="d0624-143">Windows autopilot 设备序列号。</span><span class="sxs-lookup"><span data-stu-id="d0624-143">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d0624-144">productKey</span><span class="sxs-lookup"><span data-stu-id="d0624-144">productKey</span></span>|<span data-ttu-id="d0624-145">String</span><span class="sxs-lookup"><span data-stu-id="d0624-145">String</span></span>|<span data-ttu-id="d0624-146">Windows autopilot 设备产品密钥。</span><span class="sxs-lookup"><span data-stu-id="d0624-146">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d0624-147">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d0624-147">manufacturer</span></span>|<span data-ttu-id="d0624-148">String</span><span class="sxs-lookup"><span data-stu-id="d0624-148">String</span></span>|<span data-ttu-id="d0624-149">autopilot Windows Oem 制造商。</span><span class="sxs-lookup"><span data-stu-id="d0624-149">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d0624-150">model</span><span class="sxs-lookup"><span data-stu-id="d0624-150">model</span></span>|<span data-ttu-id="d0624-151">String</span><span class="sxs-lookup"><span data-stu-id="d0624-151">String</span></span>|<span data-ttu-id="d0624-152">autopilot Windows型号名称。</span><span class="sxs-lookup"><span data-stu-id="d0624-152">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d0624-153">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d0624-153">enrollmentState</span></span>|[<span data-ttu-id="d0624-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d0624-154">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d0624-155">Autopilot 设备的 intune Windows状态。</span><span class="sxs-lookup"><span data-stu-id="d0624-155">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="d0624-156">可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`。</span><span class="sxs-lookup"><span data-stu-id="d0624-156">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.</span></span>|
|<span data-ttu-id="d0624-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0624-157">lastContactedDateTime</span></span>|<span data-ttu-id="d0624-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0624-158">DateTimeOffset</span></span>|<span data-ttu-id="d0624-159">Intune Autopilot 设备的上次Windows日期时间。</span><span class="sxs-lookup"><span data-stu-id="d0624-159">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d0624-160">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="d0624-160">addressableUserName</span></span>|<span data-ttu-id="d0624-161">String</span><span class="sxs-lookup"><span data-stu-id="d0624-161">String</span></span>|<span data-ttu-id="d0624-162">可地址用户名。</span><span class="sxs-lookup"><span data-stu-id="d0624-162">Addressable user name.</span></span>|
|<span data-ttu-id="d0624-163">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0624-163">userPrincipalName</span></span>|<span data-ttu-id="d0624-164">String</span><span class="sxs-lookup"><span data-stu-id="d0624-164">String</span></span>|<span data-ttu-id="d0624-165">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="d0624-165">User Principal Name.</span></span>|
|<span data-ttu-id="d0624-166">resourceName</span><span class="sxs-lookup"><span data-stu-id="d0624-166">resourceName</span></span>|<span data-ttu-id="d0624-167">String</span><span class="sxs-lookup"><span data-stu-id="d0624-167">String</span></span>|<span data-ttu-id="d0624-168">资源名称。</span><span class="sxs-lookup"><span data-stu-id="d0624-168">Resource Name.</span></span>|
|<span data-ttu-id="d0624-169">skuNumber</span><span class="sxs-lookup"><span data-stu-id="d0624-169">skuNumber</span></span>|<span data-ttu-id="d0624-170">String</span><span class="sxs-lookup"><span data-stu-id="d0624-170">String</span></span>|<span data-ttu-id="d0624-171">SKU 号</span><span class="sxs-lookup"><span data-stu-id="d0624-171">SKU Number</span></span>|
|<span data-ttu-id="d0624-172">systemFamily</span><span class="sxs-lookup"><span data-stu-id="d0624-172">systemFamily</span></span>|<span data-ttu-id="d0624-173">String</span><span class="sxs-lookup"><span data-stu-id="d0624-173">String</span></span>|<span data-ttu-id="d0624-174">系统系列</span><span class="sxs-lookup"><span data-stu-id="d0624-174">System Family</span></span>|
|<span data-ttu-id="d0624-175">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="d0624-175">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="d0624-176">String</span><span class="sxs-lookup"><span data-stu-id="d0624-176">String</span></span>|<span data-ttu-id="d0624-177">AAD 设备 ID - 已弃用</span><span class="sxs-lookup"><span data-stu-id="d0624-177">AAD Device ID - to be deprecated</span></span>|
|<span data-ttu-id="d0624-178">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d0624-178">managedDeviceId</span></span>|<span data-ttu-id="d0624-179">String</span><span class="sxs-lookup"><span data-stu-id="d0624-179">String</span></span>|<span data-ttu-id="d0624-180">托管设备 ID</span><span class="sxs-lookup"><span data-stu-id="d0624-180">Managed Device ID</span></span>|
|<span data-ttu-id="d0624-181">displayName</span><span class="sxs-lookup"><span data-stu-id="d0624-181">displayName</span></span>|<span data-ttu-id="d0624-182">String</span><span class="sxs-lookup"><span data-stu-id="d0624-182">String</span></span>|<span data-ttu-id="d0624-183">显示名称</span><span class="sxs-lookup"><span data-stu-id="d0624-183">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="d0624-184">响应</span><span class="sxs-lookup"><span data-stu-id="d0624-184">Response</span></span>
<span data-ttu-id="d0624-185">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0624-185">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0624-186">示例</span><span class="sxs-lookup"><span data-stu-id="d0624-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0624-187">请求</span><span class="sxs-lookup"><span data-stu-id="d0624-187">Request</span></span>
<span data-ttu-id="d0624-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0624-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="d0624-189">响应</span><span class="sxs-lookup"><span data-stu-id="d0624-189">Response</span></span>
<span data-ttu-id="d0624-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0624-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
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




