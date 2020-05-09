---
title: 创建 deviceManagementScript
description: 创建新的 deviceManagementScript 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9564b0946158b8313c01e6bd2df7fc02b04c9a3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178855"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="0ccad-103">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0ccad-103">Create deviceManagementScript</span></span>

<span data-ttu-id="0ccad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ccad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ccad-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ccad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ccad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ccad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ccad-107">创建新的[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ccad-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ccad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ccad-108">Prerequisites</span></span>
<span data-ttu-id="0ccad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ccad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ccad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ccad-111">Permission type</span></span>|<span data-ttu-id="0ccad-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ccad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ccad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ccad-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ccad-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="0ccad-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0ccad-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccad-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="0ccad-116">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="0ccad-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0ccad-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccad-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ccad-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ccad-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ccad-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ccad-119">Not supported.</span></span>|
|<span data-ttu-id="0ccad-120">Application</span><span class="sxs-lookup"><span data-stu-id="0ccad-120">Application</span></span>||
| <span data-ttu-id="0ccad-121">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="0ccad-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0ccad-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccad-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="0ccad-123">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="0ccad-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0ccad-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccad-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ccad-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ccad-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="0ccad-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ccad-126">Request headers</span></span>
|<span data-ttu-id="0ccad-127">标头</span><span class="sxs-lookup"><span data-stu-id="0ccad-127">Header</span></span>|<span data-ttu-id="0ccad-128">值</span><span class="sxs-lookup"><span data-stu-id="0ccad-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ccad-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ccad-129">Authorization</span></span>|<span data-ttu-id="0ccad-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ccad-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ccad-131">接受</span><span class="sxs-lookup"><span data-stu-id="0ccad-131">Accept</span></span>|<span data-ttu-id="0ccad-132">application/json</span><span class="sxs-lookup"><span data-stu-id="0ccad-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ccad-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ccad-133">Request body</span></span>
<span data-ttu-id="0ccad-134">在请求正文中，提供 deviceManagementScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ccad-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="0ccad-135">下表显示创建 deviceManagementScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ccad-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="0ccad-136">属性</span><span class="sxs-lookup"><span data-stu-id="0ccad-136">Property</span></span>|<span data-ttu-id="0ccad-137">类型</span><span class="sxs-lookup"><span data-stu-id="0ccad-137">Type</span></span>|<span data-ttu-id="0ccad-138">说明</span><span class="sxs-lookup"><span data-stu-id="0ccad-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ccad-139">id</span><span class="sxs-lookup"><span data-stu-id="0ccad-139">id</span></span>|<span data-ttu-id="0ccad-140">字符串</span><span class="sxs-lookup"><span data-stu-id="0ccad-140">String</span></span>|<span data-ttu-id="0ccad-141">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0ccad-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="0ccad-142">displayName</span><span class="sxs-lookup"><span data-stu-id="0ccad-142">displayName</span></span>|<span data-ttu-id="0ccad-143">字符串</span><span class="sxs-lookup"><span data-stu-id="0ccad-143">String</span></span>|<span data-ttu-id="0ccad-144">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="0ccad-144">Name of the device management script.</span></span>|
|<span data-ttu-id="0ccad-145">说明</span><span class="sxs-lookup"><span data-stu-id="0ccad-145">description</span></span>|<span data-ttu-id="0ccad-146">String</span><span class="sxs-lookup"><span data-stu-id="0ccad-146">String</span></span>|<span data-ttu-id="0ccad-147">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="0ccad-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="0ccad-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ccad-148">createdDateTime</span></span>|<span data-ttu-id="0ccad-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ccad-149">DateTimeOffset</span></span>|<span data-ttu-id="0ccad-150">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0ccad-150">The date and time the device management script was created.</span></span> <span data-ttu-id="0ccad-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0ccad-151">This property is read-only.</span></span>|
|<span data-ttu-id="0ccad-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ccad-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0ccad-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ccad-153">DateTimeOffset</span></span>|<span data-ttu-id="0ccad-154">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0ccad-154">The date and time the device management script was last modified.</span></span> <span data-ttu-id="0ccad-155">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0ccad-155">This property is read-only.</span></span>|
|<span data-ttu-id="0ccad-156">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="0ccad-156">runAsAccount</span></span>|[<span data-ttu-id="0ccad-157">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="0ccad-157">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="0ccad-158">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="0ccad-158">Indicates the type of execution context.</span></span> <span data-ttu-id="0ccad-159">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="0ccad-159">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="0ccad-160">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="0ccad-160">enforceSignatureCheck</span></span>|<span data-ttu-id="0ccad-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ccad-161">Boolean</span></span>|<span data-ttu-id="0ccad-162">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="0ccad-162">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="0ccad-163">fileName</span><span class="sxs-lookup"><span data-stu-id="0ccad-163">fileName</span></span>|<span data-ttu-id="0ccad-164">String</span><span class="sxs-lookup"><span data-stu-id="0ccad-164">String</span></span>|<span data-ttu-id="0ccad-165">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="0ccad-165">Script file name.</span></span>|
|<span data-ttu-id="0ccad-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ccad-166">roleScopeTagIds</span></span>|<span data-ttu-id="0ccad-167">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0ccad-167">String collection</span></span>|<span data-ttu-id="0ccad-168">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="0ccad-168">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="0ccad-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="0ccad-169">runAs32Bit</span></span>|<span data-ttu-id="0ccad-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ccad-170">Boolean</span></span>|<span data-ttu-id="0ccad-171">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="0ccad-171">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="0ccad-172">响应</span><span class="sxs-lookup"><span data-stu-id="0ccad-172">Response</span></span>
<span data-ttu-id="0ccad-173">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ccad-173">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ccad-174">示例</span><span class="sxs-lookup"><span data-stu-id="0ccad-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ccad-175">请求</span><span class="sxs-lookup"><span data-stu-id="0ccad-175">Request</span></span>
<span data-ttu-id="0ccad-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ccad-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
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

### <a name="response"></a><span data-ttu-id="0ccad-177">响应</span><span class="sxs-lookup"><span data-stu-id="0ccad-177">Response</span></span>
<span data-ttu-id="0ccad-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ccad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






