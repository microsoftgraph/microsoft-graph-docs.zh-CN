---
title: 更新 deviceHealthScript
description: 更新 deviceHealthScript 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd5d44e45639ed59518cc4af413b8db76a6c6430
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311631"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="986f0-103">更新 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="986f0-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="986f0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="986f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="986f0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="986f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="986f0-106">更新[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="986f0-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="986f0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="986f0-107">Prerequisites</span></span>
<span data-ttu-id="986f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="986f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="986f0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="986f0-110">Permission type</span></span>|<span data-ttu-id="986f0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="986f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="986f0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="986f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="986f0-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="986f0-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="986f0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="986f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="986f0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="986f0-115">Not supported.</span></span>|
|<span data-ttu-id="986f0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="986f0-116">Application</span></span>|<span data-ttu-id="986f0-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="986f0-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="986f0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="986f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="986f0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="986f0-119">Request headers</span></span>
|<span data-ttu-id="986f0-120">标头</span><span class="sxs-lookup"><span data-stu-id="986f0-120">Header</span></span>|<span data-ttu-id="986f0-121">值</span><span class="sxs-lookup"><span data-stu-id="986f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="986f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="986f0-122">Authorization</span></span>|<span data-ttu-id="986f0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="986f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="986f0-124">接受</span><span class="sxs-lookup"><span data-stu-id="986f0-124">Accept</span></span>|<span data-ttu-id="986f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="986f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="986f0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="986f0-126">Request body</span></span>
<span data-ttu-id="986f0-127">在请求正文中, 提供[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="986f0-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="986f0-128">下表显示创建[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="986f0-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="986f0-129">属性</span><span class="sxs-lookup"><span data-stu-id="986f0-129">Property</span></span>|<span data-ttu-id="986f0-130">类型</span><span class="sxs-lookup"><span data-stu-id="986f0-130">Type</span></span>|<span data-ttu-id="986f0-131">说明</span><span class="sxs-lookup"><span data-stu-id="986f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="986f0-132">id</span><span class="sxs-lookup"><span data-stu-id="986f0-132">id</span></span>|<span data-ttu-id="986f0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="986f0-133">String</span></span>|<span data-ttu-id="986f0-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="986f0-134">Unique Identifier for the device management script.</span></span> <span data-ttu-id="986f0-135">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-135">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="986f0-136">displayName</span></span>|<span data-ttu-id="986f0-137">字符串</span><span class="sxs-lookup"><span data-stu-id="986f0-137">String</span></span>|<span data-ttu-id="986f0-138">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="986f0-138">Name of the device management script.</span></span> <span data-ttu-id="986f0-139">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-139">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-140">说明</span><span class="sxs-lookup"><span data-stu-id="986f0-140">description</span></span>|<span data-ttu-id="986f0-141">String</span><span class="sxs-lookup"><span data-stu-id="986f0-141">String</span></span>|<span data-ttu-id="986f0-142">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="986f0-142">Optional description for the device management script.</span></span> <span data-ttu-id="986f0-143">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-143">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="986f0-144">runSchedule</span></span>|[<span data-ttu-id="986f0-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="986f0-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="986f0-146">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="986f0-146">The interval for script to run.</span></span> <span data-ttu-id="986f0-147">如果未定义, 脚本将在从[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)继承后运行。</span><span class="sxs-lookup"><span data-stu-id="986f0-147">If not defined the script will run once Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="986f0-148">scriptContent</span></span>|<span data-ttu-id="986f0-149">Binary</span><span class="sxs-lookup"><span data-stu-id="986f0-149">Binary</span></span>|<span data-ttu-id="986f0-150">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="986f0-150">The script content.</span></span> <span data-ttu-id="986f0-151">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-151">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="986f0-152">createdDateTime</span></span>|<span data-ttu-id="986f0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="986f0-153">DateTimeOffset</span></span>|<span data-ttu-id="986f0-154">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="986f0-154">The date and time the device management script was created.</span></span> <span data-ttu-id="986f0-155">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-155">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="986f0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="986f0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="986f0-157">DateTimeOffset</span></span>|<span data-ttu-id="986f0-158">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="986f0-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="986f0-159">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-159">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="986f0-160">runAsAccount</span></span>|[<span data-ttu-id="986f0-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="986f0-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="986f0-162">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="986f0-162">Indicates the type of execution context.</span></span> <span data-ttu-id="986f0-163">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)。</span><span class="sxs-lookup"><span data-stu-id="986f0-163">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span> <span data-ttu-id="986f0-164">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="986f0-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="986f0-165">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="986f0-165">enforceSignatureCheck</span></span>|<span data-ttu-id="986f0-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="986f0-166">Boolean</span></span>|<span data-ttu-id="986f0-167">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="986f0-167">Indicate whether the script signature needs be checked.</span></span> <span data-ttu-id="986f0-168">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-168">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-169">fileName</span><span class="sxs-lookup"><span data-stu-id="986f0-169">fileName</span></span>|<span data-ttu-id="986f0-170">String</span><span class="sxs-lookup"><span data-stu-id="986f0-170">String</span></span>|<span data-ttu-id="986f0-171">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="986f0-171">Script file name.</span></span> <span data-ttu-id="986f0-172">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-172">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="986f0-173">roleScopeTagIds</span></span>|<span data-ttu-id="986f0-174">String collection</span><span class="sxs-lookup"><span data-stu-id="986f0-174">String collection</span></span>|<span data-ttu-id="986f0-175">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="986f0-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span> <span data-ttu-id="986f0-176">继承自[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="986f0-176">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-177">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="986f0-177">runAs32Bit</span></span>|<span data-ttu-id="986f0-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="986f0-178">Boolean</span></span>|<span data-ttu-id="986f0-179">一个指示 PowerShell 脚本是否应作为从[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)继承的32位运行的值</span><span class="sxs-lookup"><span data-stu-id="986f0-179">A value indicating whether the PowerShell script should run as 32-bit Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="986f0-180">complianceRule</span><span class="sxs-lookup"><span data-stu-id="986f0-180">complianceRule</span></span>|[<span data-ttu-id="986f0-181">deviceHealthScriptComplianceRule</span><span class="sxs-lookup"><span data-stu-id="986f0-181">deviceHealthScriptComplianceRule</span></span>](../resources/intune-devices-devicehealthscriptcompliancerule.md)|<span data-ttu-id="986f0-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="986f0-182">Not yet documented</span></span>|
|<span data-ttu-id="986f0-183">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="986f0-183">remediationScriptContent</span></span>|<span data-ttu-id="986f0-184">Binary</span><span class="sxs-lookup"><span data-stu-id="986f0-184">Binary</span></span>|<span data-ttu-id="986f0-185">尚未记录</span><span class="sxs-lookup"><span data-stu-id="986f0-185">Not yet documented</span></span>|
|<span data-ttu-id="986f0-186">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="986f0-186">runRemediationScript</span></span>|<span data-ttu-id="986f0-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="986f0-187">Boolean</span></span>|<span data-ttu-id="986f0-188">尚未记录</span><span class="sxs-lookup"><span data-stu-id="986f0-188">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="986f0-189">响应</span><span class="sxs-lookup"><span data-stu-id="986f0-189">Response</span></span>
<span data-ttu-id="986f0-190">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="986f0-190">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="986f0-191">示例</span><span class="sxs-lookup"><span data-stu-id="986f0-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="986f0-192">请求</span><span class="sxs-lookup"><span data-stu-id="986f0-192">Request</span></span>
<span data-ttu-id="986f0-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="986f0-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
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

### <a name="response"></a><span data-ttu-id="986f0-194">响应</span><span class="sxs-lookup"><span data-stu-id="986f0-194">Response</span></span>
<span data-ttu-id="986f0-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="986f0-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






