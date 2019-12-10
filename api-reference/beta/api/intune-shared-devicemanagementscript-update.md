---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfdfc4523bf7698eb2eee483845e0bc446f8f2df
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939870"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="23e08-103">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="23e08-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="23e08-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23e08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23e08-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23e08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23e08-106">更新[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="23e08-106">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23e08-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="23e08-107">Prerequisites</span></span>
<span data-ttu-id="23e08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23e08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23e08-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="23e08-110">Permission type</span></span>|<span data-ttu-id="23e08-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="23e08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23e08-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23e08-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="23e08-113">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="23e08-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="23e08-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e08-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="23e08-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="23e08-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="23e08-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e08-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="23e08-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23e08-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23e08-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="23e08-118">Not supported.</span></span>|
|<span data-ttu-id="23e08-119">Application</span><span class="sxs-lookup"><span data-stu-id="23e08-119">Application</span></span>||
| <span data-ttu-id="23e08-120">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="23e08-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="23e08-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e08-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="23e08-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="23e08-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="23e08-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e08-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23e08-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23e08-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="23e08-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="23e08-125">Request headers</span></span>
|<span data-ttu-id="23e08-126">标头</span><span class="sxs-lookup"><span data-stu-id="23e08-126">Header</span></span>|<span data-ttu-id="23e08-127">值</span><span class="sxs-lookup"><span data-stu-id="23e08-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23e08-128">授权</span><span class="sxs-lookup"><span data-stu-id="23e08-128">Authorization</span></span>|<span data-ttu-id="23e08-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="23e08-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23e08-130">接受</span><span class="sxs-lookup"><span data-stu-id="23e08-130">Accept</span></span>|<span data-ttu-id="23e08-131">application/json</span><span class="sxs-lookup"><span data-stu-id="23e08-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23e08-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="23e08-132">Request body</span></span>
<span data-ttu-id="23e08-133">在请求正文中，提供[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23e08-133">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="23e08-134">下表显示创建[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="23e08-134">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="23e08-135">属性</span><span class="sxs-lookup"><span data-stu-id="23e08-135">Property</span></span>|<span data-ttu-id="23e08-136">类型</span><span class="sxs-lookup"><span data-stu-id="23e08-136">Type</span></span>|<span data-ttu-id="23e08-137">说明</span><span class="sxs-lookup"><span data-stu-id="23e08-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23e08-138">id</span><span class="sxs-lookup"><span data-stu-id="23e08-138">id</span></span>|<span data-ttu-id="23e08-139">字符串</span><span class="sxs-lookup"><span data-stu-id="23e08-139">String</span></span>|<span data-ttu-id="23e08-140">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="23e08-140">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="23e08-141">displayName</span><span class="sxs-lookup"><span data-stu-id="23e08-141">displayName</span></span>|<span data-ttu-id="23e08-142">字符串</span><span class="sxs-lookup"><span data-stu-id="23e08-142">String</span></span>|<span data-ttu-id="23e08-143">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="23e08-143">Name of the device management script.</span></span>|
|<span data-ttu-id="23e08-144">说明</span><span class="sxs-lookup"><span data-stu-id="23e08-144">description</span></span>|<span data-ttu-id="23e08-145">String</span><span class="sxs-lookup"><span data-stu-id="23e08-145">String</span></span>|<span data-ttu-id="23e08-146">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="23e08-146">Optional description for the device management script.</span></span>|
|<span data-ttu-id="23e08-147">runSchedule</span><span class="sxs-lookup"><span data-stu-id="23e08-147">runSchedule</span></span>|[<span data-ttu-id="23e08-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="23e08-148">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="23e08-149">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="23e08-149">The interval for script to run.</span></span> <span data-ttu-id="23e08-150">如果未定义，脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="23e08-150">If not defined the script will run once</span></span>|
|<span data-ttu-id="23e08-151">scriptContent</span><span class="sxs-lookup"><span data-stu-id="23e08-151">scriptContent</span></span>|<span data-ttu-id="23e08-152">Binary</span><span class="sxs-lookup"><span data-stu-id="23e08-152">Binary</span></span>|<span data-ttu-id="23e08-153">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="23e08-153">The script content.</span></span>|
|<span data-ttu-id="23e08-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23e08-154">createdDateTime</span></span>|<span data-ttu-id="23e08-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23e08-155">DateTimeOffset</span></span>|<span data-ttu-id="23e08-156">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="23e08-156">The date and time the device management script was created.</span></span> <span data-ttu-id="23e08-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="23e08-157">This property is read-only.</span></span>|
|<span data-ttu-id="23e08-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23e08-158">lastModifiedDateTime</span></span>|<span data-ttu-id="23e08-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23e08-159">DateTimeOffset</span></span>|<span data-ttu-id="23e08-160">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="23e08-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="23e08-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="23e08-161">This property is read-only.</span></span>|
|<span data-ttu-id="23e08-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="23e08-162">runAsAccount</span></span>|[<span data-ttu-id="23e08-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="23e08-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="23e08-164">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="23e08-164">Indicates the type of execution context.</span></span> <span data-ttu-id="23e08-165">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="23e08-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="23e08-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="23e08-166">enforceSignatureCheck</span></span>|<span data-ttu-id="23e08-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="23e08-167">Boolean</span></span>|<span data-ttu-id="23e08-168">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="23e08-168">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="23e08-169">fileName</span><span class="sxs-lookup"><span data-stu-id="23e08-169">fileName</span></span>|<span data-ttu-id="23e08-170">String</span><span class="sxs-lookup"><span data-stu-id="23e08-170">String</span></span>|<span data-ttu-id="23e08-171">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="23e08-171">Script file name.</span></span>|
|<span data-ttu-id="23e08-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23e08-172">roleScopeTagIds</span></span>|<span data-ttu-id="23e08-173">String collection</span><span class="sxs-lookup"><span data-stu-id="23e08-173">String collection</span></span>|<span data-ttu-id="23e08-174">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="23e08-174">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="23e08-175">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="23e08-175">runAs32Bit</span></span>|<span data-ttu-id="23e08-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="23e08-176">Boolean</span></span>|<span data-ttu-id="23e08-177">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="23e08-177">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="23e08-178">响应</span><span class="sxs-lookup"><span data-stu-id="23e08-178">Response</span></span>
<span data-ttu-id="23e08-179">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="23e08-179">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23e08-180">示例</span><span class="sxs-lookup"><span data-stu-id="23e08-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="23e08-181">请求</span><span class="sxs-lookup"><span data-stu-id="23e08-181">Request</span></span>
<span data-ttu-id="23e08-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23e08-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="23e08-183">响应</span><span class="sxs-lookup"><span data-stu-id="23e08-183">Response</span></span>
<span data-ttu-id="23e08-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23e08-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
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
  "runAs32Bit": true
}
```








