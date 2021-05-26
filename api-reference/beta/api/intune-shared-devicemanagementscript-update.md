---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f68184a74714ee8ce74af3f25019123fe69d0891
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662933"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="2096b-103">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="2096b-103">Update deviceManagementScript</span></span>

<span data-ttu-id="2096b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2096b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2096b-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2096b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2096b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2096b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2096b-107">更新 [deviceManagementScript 对象](../resources/intune-shared-devicemanagementscript.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2096b-107">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2096b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2096b-108">Prerequisites</span></span>
<span data-ttu-id="2096b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2096b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2096b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2096b-111">Permission type</span></span>|<span data-ttu-id="2096b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2096b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2096b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2096b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2096b-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="2096b-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2096b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2096b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2096b-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="2096b-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2096b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2096b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2096b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2096b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2096b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2096b-119">Not supported.</span></span>|
|<span data-ttu-id="2096b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2096b-120">Application</span></span>||
| <span data-ttu-id="2096b-121">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="2096b-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2096b-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2096b-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2096b-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="2096b-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2096b-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2096b-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2096b-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2096b-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="2096b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="2096b-126">Request headers</span></span>
|<span data-ttu-id="2096b-127">标头</span><span class="sxs-lookup"><span data-stu-id="2096b-127">Header</span></span>|<span data-ttu-id="2096b-128">值</span><span class="sxs-lookup"><span data-stu-id="2096b-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2096b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2096b-129">Authorization</span></span>|<span data-ttu-id="2096b-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2096b-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2096b-131">接受</span><span class="sxs-lookup"><span data-stu-id="2096b-131">Accept</span></span>|<span data-ttu-id="2096b-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2096b-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2096b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2096b-133">Request body</span></span>
<span data-ttu-id="2096b-134">在请求正文中，提供 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2096b-134">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="2096b-135">下表显示创建 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2096b-135">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="2096b-136">属性</span><span class="sxs-lookup"><span data-stu-id="2096b-136">Property</span></span>|<span data-ttu-id="2096b-137">类型</span><span class="sxs-lookup"><span data-stu-id="2096b-137">Type</span></span>|<span data-ttu-id="2096b-138">说明</span><span class="sxs-lookup"><span data-stu-id="2096b-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2096b-139">id</span><span class="sxs-lookup"><span data-stu-id="2096b-139">id</span></span>|<span data-ttu-id="2096b-140">String</span><span class="sxs-lookup"><span data-stu-id="2096b-140">String</span></span>|<span data-ttu-id="2096b-141">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2096b-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="2096b-142">displayName</span><span class="sxs-lookup"><span data-stu-id="2096b-142">displayName</span></span>|<span data-ttu-id="2096b-143">String</span><span class="sxs-lookup"><span data-stu-id="2096b-143">String</span></span>|<span data-ttu-id="2096b-144">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="2096b-144">Name of the device management script.</span></span>|
|<span data-ttu-id="2096b-145">说明</span><span class="sxs-lookup"><span data-stu-id="2096b-145">description</span></span>|<span data-ttu-id="2096b-146">String</span><span class="sxs-lookup"><span data-stu-id="2096b-146">String</span></span>|<span data-ttu-id="2096b-147">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="2096b-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="2096b-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="2096b-148">scriptContent</span></span>|<span data-ttu-id="2096b-149">二进制</span><span class="sxs-lookup"><span data-stu-id="2096b-149">Binary</span></span>|<span data-ttu-id="2096b-150">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="2096b-150">The script content.</span></span>|
|<span data-ttu-id="2096b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2096b-151">createdDateTime</span></span>|<span data-ttu-id="2096b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2096b-152">DateTimeOffset</span></span>|<span data-ttu-id="2096b-153">创建设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2096b-153">The date and time the device management script was created.</span></span> <span data-ttu-id="2096b-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2096b-154">This property is read-only.</span></span>|
|<span data-ttu-id="2096b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2096b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2096b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2096b-156">DateTimeOffset</span></span>|<span data-ttu-id="2096b-157">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2096b-157">The date and time the device management script was last modified.</span></span> <span data-ttu-id="2096b-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2096b-158">This property is read-only.</span></span>|
|<span data-ttu-id="2096b-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="2096b-159">runAsAccount</span></span>|[<span data-ttu-id="2096b-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="2096b-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="2096b-161">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="2096b-161">Indicates the type of execution context.</span></span> <span data-ttu-id="2096b-162">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="2096b-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="2096b-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="2096b-163">enforceSignatureCheck</span></span>|<span data-ttu-id="2096b-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="2096b-164">Boolean</span></span>|<span data-ttu-id="2096b-165">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="2096b-165">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="2096b-166">fileName</span><span class="sxs-lookup"><span data-stu-id="2096b-166">fileName</span></span>|<span data-ttu-id="2096b-167">String</span><span class="sxs-lookup"><span data-stu-id="2096b-167">String</span></span>|<span data-ttu-id="2096b-168">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="2096b-168">Script file name.</span></span>|
|<span data-ttu-id="2096b-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2096b-169">roleScopeTagIds</span></span>|<span data-ttu-id="2096b-170">String collection</span><span class="sxs-lookup"><span data-stu-id="2096b-170">String collection</span></span>|<span data-ttu-id="2096b-171">此 PowerShellScript 实例的范围标记标识列表。</span><span class="sxs-lookup"><span data-stu-id="2096b-171">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="2096b-172">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="2096b-172">runAs32Bit</span></span>|<span data-ttu-id="2096b-173">布尔值</span><span class="sxs-lookup"><span data-stu-id="2096b-173">Boolean</span></span>|<span data-ttu-id="2096b-174">指示 PowerShell 脚本是否应该作为 32 位运行的值</span><span class="sxs-lookup"><span data-stu-id="2096b-174">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="2096b-175">响应</span><span class="sxs-lookup"><span data-stu-id="2096b-175">Response</span></span>
<span data-ttu-id="2096b-176">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2096b-176">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2096b-177">示例</span><span class="sxs-lookup"><span data-stu-id="2096b-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="2096b-178">请求</span><span class="sxs-lookup"><span data-stu-id="2096b-178">Request</span></span>
<span data-ttu-id="2096b-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2096b-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="2096b-180">响应</span><span class="sxs-lookup"><span data-stu-id="2096b-180">Response</span></span>
<span data-ttu-id="2096b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2096b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
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







