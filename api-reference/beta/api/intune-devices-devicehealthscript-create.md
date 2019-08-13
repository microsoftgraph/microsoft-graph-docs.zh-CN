---
title: 创建 deviceHealthScript
description: 创建新的 deviceHealthScript 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0084852f4c0cb236931ee532f12e54a08c1e2fc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311639"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="5a0ab-103">创建 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="5a0ab-103">Create deviceHealthScript</span></span>

> <span data-ttu-id="5a0ab-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a0ab-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a0ab-106">创建新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-106">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a0ab-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a0ab-107">Prerequisites</span></span>
<span data-ttu-id="5a0ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a0ab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a0ab-110">Permission type</span></span>|<span data-ttu-id="5a0ab-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5a0ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a0ab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a0ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a0ab-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0ab-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5a0ab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a0ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a0ab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-115">Not supported.</span></span>|
|<span data-ttu-id="5a0ab-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a0ab-116">Application</span></span>|<span data-ttu-id="5a0ab-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a0ab-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a0ab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a0ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="5a0ab-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a0ab-119">Request headers</span></span>
|<span data-ttu-id="5a0ab-120">标头</span><span class="sxs-lookup"><span data-stu-id="5a0ab-120">Header</span></span>|<span data-ttu-id="5a0ab-121">值</span><span class="sxs-lookup"><span data-stu-id="5a0ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a0ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a0ab-122">Authorization</span></span>|<span data-ttu-id="5a0ab-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a0ab-124">接受</span><span class="sxs-lookup"><span data-stu-id="5a0ab-124">Accept</span></span>|<span data-ttu-id="5a0ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a0ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a0ab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a0ab-126">Request body</span></span>
<span data-ttu-id="5a0ab-127">在请求正文中, 提供 deviceHealthScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-127">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="5a0ab-128">下表显示创建 deviceHealthScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-128">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="5a0ab-129">属性</span><span class="sxs-lookup"><span data-stu-id="5a0ab-129">Property</span></span>|<span data-ttu-id="5a0ab-130">类型</span><span class="sxs-lookup"><span data-stu-id="5a0ab-130">Type</span></span>|<span data-ttu-id="5a0ab-131">说明</span><span class="sxs-lookup"><span data-stu-id="5a0ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a0ab-132">id</span><span class="sxs-lookup"><span data-stu-id="5a0ab-132">id</span></span>|<span data-ttu-id="5a0ab-133">字符串</span><span class="sxs-lookup"><span data-stu-id="5a0ab-133">String</span></span>|<span data-ttu-id="5a0ab-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-134">Unique Identifier for the device management script.</span></span> <span data-ttu-id="5a0ab-135">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-135">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5a0ab-136">displayName</span></span>|<span data-ttu-id="5a0ab-137">字符串</span><span class="sxs-lookup"><span data-stu-id="5a0ab-137">String</span></span>|<span data-ttu-id="5a0ab-138">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-138">Name of the device management script.</span></span> <span data-ttu-id="5a0ab-139">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-139">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-140">说明</span><span class="sxs-lookup"><span data-stu-id="5a0ab-140">description</span></span>|<span data-ttu-id="5a0ab-141">String</span><span class="sxs-lookup"><span data-stu-id="5a0ab-141">String</span></span>|<span data-ttu-id="5a0ab-142">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-142">Optional description for the device management script.</span></span> <span data-ttu-id="5a0ab-143">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-143">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="5a0ab-144">runSchedule</span></span>|[<span data-ttu-id="5a0ab-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="5a0ab-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="5a0ab-146">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-146">The interval for script to run.</span></span> <span data-ttu-id="5a0ab-147">如果未定义, 脚本将在从[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)继承后运行。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-147">If not defined the script will run once Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="5a0ab-148">scriptContent</span></span>|<span data-ttu-id="5a0ab-149">Binary</span><span class="sxs-lookup"><span data-stu-id="5a0ab-149">Binary</span></span>|<span data-ttu-id="5a0ab-150">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-150">The script content.</span></span> <span data-ttu-id="5a0ab-151">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-151">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a0ab-152">createdDateTime</span></span>|<span data-ttu-id="5a0ab-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a0ab-153">DateTimeOffset</span></span>|<span data-ttu-id="5a0ab-154">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-154">The date and time the device management script was created.</span></span> <span data-ttu-id="5a0ab-155">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-155">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a0ab-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5a0ab-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a0ab-157">DateTimeOffset</span></span>|<span data-ttu-id="5a0ab-158">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="5a0ab-159">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-159">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="5a0ab-160">runAsAccount</span></span>|[<span data-ttu-id="5a0ab-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="5a0ab-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="5a0ab-162">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-162">Indicates the type of execution context.</span></span> <span data-ttu-id="5a0ab-163">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-163">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span> <span data-ttu-id="5a0ab-164">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="5a0ab-165">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="5a0ab-165">enforceSignatureCheck</span></span>|<span data-ttu-id="5a0ab-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a0ab-166">Boolean</span></span>|<span data-ttu-id="5a0ab-167">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-167">Indicate whether the script signature needs be checked.</span></span> <span data-ttu-id="5a0ab-168">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-168">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-169">fileName</span><span class="sxs-lookup"><span data-stu-id="5a0ab-169">fileName</span></span>|<span data-ttu-id="5a0ab-170">String</span><span class="sxs-lookup"><span data-stu-id="5a0ab-170">String</span></span>|<span data-ttu-id="5a0ab-171">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-171">Script file name.</span></span> <span data-ttu-id="5a0ab-172">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-172">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5a0ab-173">roleScopeTagIds</span></span>|<span data-ttu-id="5a0ab-174">String collection</span><span class="sxs-lookup"><span data-stu-id="5a0ab-174">String collection</span></span>|<span data-ttu-id="5a0ab-175">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span> <span data-ttu-id="5a0ab-176">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5a0ab-176">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-177">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="5a0ab-177">runAs32Bit</span></span>|<span data-ttu-id="5a0ab-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a0ab-178">Boolean</span></span>|<span data-ttu-id="5a0ab-179">一个指示 PowerShell 脚本是否应作为从[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)继承的32位运行的值</span><span class="sxs-lookup"><span data-stu-id="5a0ab-179">A value indicating whether the PowerShell script should run as 32-bit Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="5a0ab-180">complianceRule</span><span class="sxs-lookup"><span data-stu-id="5a0ab-180">complianceRule</span></span>|[<span data-ttu-id="5a0ab-181">deviceHealthScriptComplianceRule</span><span class="sxs-lookup"><span data-stu-id="5a0ab-181">deviceHealthScriptComplianceRule</span></span>](../resources/intune-devices-devicehealthscriptcompliancerule.md)|<span data-ttu-id="5a0ab-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5a0ab-182">Not yet documented</span></span>|
|<span data-ttu-id="5a0ab-183">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="5a0ab-183">remediationScriptContent</span></span>|<span data-ttu-id="5a0ab-184">Binary</span><span class="sxs-lookup"><span data-stu-id="5a0ab-184">Binary</span></span>|<span data-ttu-id="5a0ab-185">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5a0ab-185">Not yet documented</span></span>|
|<span data-ttu-id="5a0ab-186">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="5a0ab-186">runRemediationScript</span></span>|<span data-ttu-id="5a0ab-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a0ab-187">Boolean</span></span>|<span data-ttu-id="5a0ab-188">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5a0ab-188">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5a0ab-189">响应</span><span class="sxs-lookup"><span data-stu-id="5a0ab-189">Response</span></span>
<span data-ttu-id="5a0ab-190">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-190">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a0ab-191">示例</span><span class="sxs-lookup"><span data-stu-id="5a0ab-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a0ab-192">请求</span><span class="sxs-lookup"><span data-stu-id="5a0ab-192">Request</span></span>
<span data-ttu-id="5a0ab-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```

### <a name="response"></a><span data-ttu-id="5a0ab-194">响应</span><span class="sxs-lookup"><span data-stu-id="5a0ab-194">Response</span></span>
<span data-ttu-id="5a0ab-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a0ab-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```






