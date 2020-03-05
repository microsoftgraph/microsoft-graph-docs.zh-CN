---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f16d40792835086b8c87bf3a3636138deba794d7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458460"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="d0030-103">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="d0030-103">Update deviceManagementScript</span></span>

<span data-ttu-id="d0030-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d0030-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0030-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0030-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0030-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0030-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0030-107">更新[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d0030-107">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0030-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0030-108">Prerequisites</span></span>
<span data-ttu-id="d0030-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0030-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0030-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0030-111">Permission type</span></span>|<span data-ttu-id="d0030-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0030-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0030-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0030-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d0030-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="d0030-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d0030-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0030-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d0030-116">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="d0030-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d0030-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0030-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0030-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0030-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0030-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0030-119">Not supported.</span></span>|
|<span data-ttu-id="d0030-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0030-120">Application</span></span>||
| <span data-ttu-id="d0030-121">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="d0030-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d0030-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0030-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d0030-123">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="d0030-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d0030-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0030-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0030-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0030-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="d0030-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0030-126">Request headers</span></span>
|<span data-ttu-id="d0030-127">标头</span><span class="sxs-lookup"><span data-stu-id="d0030-127">Header</span></span>|<span data-ttu-id="d0030-128">值</span><span class="sxs-lookup"><span data-stu-id="d0030-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0030-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0030-129">Authorization</span></span>|<span data-ttu-id="d0030-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0030-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0030-131">接受</span><span class="sxs-lookup"><span data-stu-id="d0030-131">Accept</span></span>|<span data-ttu-id="d0030-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d0030-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0030-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0030-133">Request body</span></span>
<span data-ttu-id="d0030-134">在请求正文中，提供[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0030-134">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="d0030-135">下表显示创建[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d0030-135">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="d0030-136">属性</span><span class="sxs-lookup"><span data-stu-id="d0030-136">Property</span></span>|<span data-ttu-id="d0030-137">类型</span><span class="sxs-lookup"><span data-stu-id="d0030-137">Type</span></span>|<span data-ttu-id="d0030-138">说明</span><span class="sxs-lookup"><span data-stu-id="d0030-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0030-139">id</span><span class="sxs-lookup"><span data-stu-id="d0030-139">id</span></span>|<span data-ttu-id="d0030-140">字符串</span><span class="sxs-lookup"><span data-stu-id="d0030-140">String</span></span>|<span data-ttu-id="d0030-141">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d0030-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="d0030-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d0030-142">displayName</span></span>|<span data-ttu-id="d0030-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d0030-143">String</span></span>|<span data-ttu-id="d0030-144">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="d0030-144">Name of the device management script.</span></span>|
|<span data-ttu-id="d0030-145">说明</span><span class="sxs-lookup"><span data-stu-id="d0030-145">description</span></span>|<span data-ttu-id="d0030-146">String</span><span class="sxs-lookup"><span data-stu-id="d0030-146">String</span></span>|<span data-ttu-id="d0030-147">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="d0030-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="d0030-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d0030-148">runSchedule</span></span>|[<span data-ttu-id="d0030-149">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d0030-149">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="d0030-150">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="d0030-150">The interval for script to run.</span></span> <span data-ttu-id="d0030-151">如果未定义，脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="d0030-151">If not defined the script will run once</span></span>|
|<span data-ttu-id="d0030-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="d0030-152">scriptContent</span></span>|<span data-ttu-id="d0030-153">Binary</span><span class="sxs-lookup"><span data-stu-id="d0030-153">Binary</span></span>|<span data-ttu-id="d0030-154">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="d0030-154">The script content.</span></span>|
|<span data-ttu-id="d0030-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0030-155">createdDateTime</span></span>|<span data-ttu-id="d0030-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0030-156">DateTimeOffset</span></span>|<span data-ttu-id="d0030-157">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d0030-157">The date and time the device management script was created.</span></span> <span data-ttu-id="d0030-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d0030-158">This property is read-only.</span></span>|
|<span data-ttu-id="d0030-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0030-159">lastModifiedDateTime</span></span>|<span data-ttu-id="d0030-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0030-160">DateTimeOffset</span></span>|<span data-ttu-id="d0030-161">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d0030-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="d0030-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d0030-162">This property is read-only.</span></span>|
|<span data-ttu-id="d0030-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d0030-163">runAsAccount</span></span>|[<span data-ttu-id="d0030-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="d0030-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d0030-165">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="d0030-165">Indicates the type of execution context.</span></span> <span data-ttu-id="d0030-166">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="d0030-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="d0030-167">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="d0030-167">enforceSignatureCheck</span></span>|<span data-ttu-id="d0030-168">布尔</span><span class="sxs-lookup"><span data-stu-id="d0030-168">Boolean</span></span>|<span data-ttu-id="d0030-169">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="d0030-169">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="d0030-170">fileName</span><span class="sxs-lookup"><span data-stu-id="d0030-170">fileName</span></span>|<span data-ttu-id="d0030-171">String</span><span class="sxs-lookup"><span data-stu-id="d0030-171">String</span></span>|<span data-ttu-id="d0030-172">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="d0030-172">Script file name.</span></span>|
|<span data-ttu-id="d0030-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0030-173">roleScopeTagIds</span></span>|<span data-ttu-id="d0030-174">String 集合</span><span class="sxs-lookup"><span data-stu-id="d0030-174">String collection</span></span>|<span data-ttu-id="d0030-175">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="d0030-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="d0030-176">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="d0030-176">runAs32Bit</span></span>|<span data-ttu-id="d0030-177">布尔</span><span class="sxs-lookup"><span data-stu-id="d0030-177">Boolean</span></span>|<span data-ttu-id="d0030-178">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="d0030-178">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="d0030-179">响应</span><span class="sxs-lookup"><span data-stu-id="d0030-179">Response</span></span>
<span data-ttu-id="d0030-180">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d0030-180">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0030-181">示例</span><span class="sxs-lookup"><span data-stu-id="d0030-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0030-182">请求</span><span class="sxs-lookup"><span data-stu-id="d0030-182">Request</span></span>
<span data-ttu-id="d0030-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0030-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0030-184">响应</span><span class="sxs-lookup"><span data-stu-id="d0030-184">Response</span></span>
<span data-ttu-id="d0030-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0030-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








