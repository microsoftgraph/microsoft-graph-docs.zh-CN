---
title: 创建 deviceManagementScript
description: 创建新的 deviceManagementScript 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 370e0663907f7c45e63b306480d876fd2acce458
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791326"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="8ea9d-103">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="8ea9d-103">Create deviceManagementScript</span></span>

<span data-ttu-id="8ea9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ea9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ea9d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ea9d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ea9d-107">创建新的[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ea9d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ea9d-108">Prerequisites</span></span>
<span data-ttu-id="8ea9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ea9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ea9d-111">Permission type</span></span>|<span data-ttu-id="8ea9d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8ea9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ea9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ea9d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8ea9d-114">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="8ea9d-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8ea9d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ea9d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8ea9d-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="8ea9d-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8ea9d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ea9d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ea9d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ea9d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ea9d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-119">Not supported.</span></span>|
|<span data-ttu-id="8ea9d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ea9d-120">Application</span></span>||
| <span data-ttu-id="8ea9d-121">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="8ea9d-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8ea9d-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ea9d-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8ea9d-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="8ea9d-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8ea9d-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ea9d-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ea9d-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ea9d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="8ea9d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ea9d-126">Request headers</span></span>
|<span data-ttu-id="8ea9d-127">标头</span><span class="sxs-lookup"><span data-stu-id="8ea9d-127">Header</span></span>|<span data-ttu-id="8ea9d-128">值</span><span class="sxs-lookup"><span data-stu-id="8ea9d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ea9d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ea9d-129">Authorization</span></span>|<span data-ttu-id="8ea9d-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ea9d-131">接受</span><span class="sxs-lookup"><span data-stu-id="8ea9d-131">Accept</span></span>|<span data-ttu-id="8ea9d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8ea9d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ea9d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ea9d-133">Request body</span></span>
<span data-ttu-id="8ea9d-134">在请求正文中，提供 deviceManagementScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="8ea9d-135">下表显示创建 deviceManagementScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="8ea9d-136">属性</span><span class="sxs-lookup"><span data-stu-id="8ea9d-136">Property</span></span>|<span data-ttu-id="8ea9d-137">类型</span><span class="sxs-lookup"><span data-stu-id="8ea9d-137">Type</span></span>|<span data-ttu-id="8ea9d-138">说明</span><span class="sxs-lookup"><span data-stu-id="8ea9d-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ea9d-139">id</span><span class="sxs-lookup"><span data-stu-id="8ea9d-139">id</span></span>|<span data-ttu-id="8ea9d-140">字符串</span><span class="sxs-lookup"><span data-stu-id="8ea9d-140">String</span></span>|<span data-ttu-id="8ea9d-141">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="8ea9d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8ea9d-142">displayName</span></span>|<span data-ttu-id="8ea9d-143">字符串</span><span class="sxs-lookup"><span data-stu-id="8ea9d-143">String</span></span>|<span data-ttu-id="8ea9d-144">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-144">Name of the device management script.</span></span>|
|<span data-ttu-id="8ea9d-145">说明</span><span class="sxs-lookup"><span data-stu-id="8ea9d-145">description</span></span>|<span data-ttu-id="8ea9d-146">String</span><span class="sxs-lookup"><span data-stu-id="8ea9d-146">String</span></span>|<span data-ttu-id="8ea9d-147">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="8ea9d-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="8ea9d-148">runSchedule</span></span>|<span data-ttu-id="8ea9d-149">runSchedule</span><span class="sxs-lookup"><span data-stu-id="8ea9d-149">runSchedule</span></span>|<span data-ttu-id="8ea9d-150">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-150">The interval for script to run.</span></span> <span data-ttu-id="8ea9d-151">如果未定义，脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="8ea9d-151">If not defined the script will run once</span></span>|
|<span data-ttu-id="8ea9d-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="8ea9d-152">scriptContent</span></span>|<span data-ttu-id="8ea9d-153">Binary</span><span class="sxs-lookup"><span data-stu-id="8ea9d-153">Binary</span></span>|<span data-ttu-id="8ea9d-154">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-154">The script content.</span></span>|
|<span data-ttu-id="8ea9d-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ea9d-155">createdDateTime</span></span>|<span data-ttu-id="8ea9d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ea9d-156">DateTimeOffset</span></span>|<span data-ttu-id="8ea9d-157">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-157">The date and time the device management script was created.</span></span> <span data-ttu-id="8ea9d-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-158">This property is read-only.</span></span>|
|<span data-ttu-id="8ea9d-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ea9d-159">lastModifiedDateTime</span></span>|<span data-ttu-id="8ea9d-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ea9d-160">DateTimeOffset</span></span>|<span data-ttu-id="8ea9d-161">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="8ea9d-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-162">This property is read-only.</span></span>|
|<span data-ttu-id="8ea9d-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="8ea9d-163">runAsAccount</span></span>|[<span data-ttu-id="8ea9d-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="8ea9d-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="8ea9d-165">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-165">Indicates the type of execution context.</span></span> <span data-ttu-id="8ea9d-166">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="8ea9d-167">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="8ea9d-167">enforceSignatureCheck</span></span>|<span data-ttu-id="8ea9d-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="8ea9d-168">Boolean</span></span>|<span data-ttu-id="8ea9d-169">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-169">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="8ea9d-170">fileName</span><span class="sxs-lookup"><span data-stu-id="8ea9d-170">fileName</span></span>|<span data-ttu-id="8ea9d-171">String</span><span class="sxs-lookup"><span data-stu-id="8ea9d-171">String</span></span>|<span data-ttu-id="8ea9d-172">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-172">Script file name.</span></span>|
|<span data-ttu-id="8ea9d-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ea9d-173">roleScopeTagIds</span></span>|<span data-ttu-id="8ea9d-174">String collection</span><span class="sxs-lookup"><span data-stu-id="8ea9d-174">String collection</span></span>|<span data-ttu-id="8ea9d-175">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="8ea9d-176">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="8ea9d-176">runAs32Bit</span></span>|<span data-ttu-id="8ea9d-177">布尔值</span><span class="sxs-lookup"><span data-stu-id="8ea9d-177">Boolean</span></span>|<span data-ttu-id="8ea9d-178">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="8ea9d-178">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="8ea9d-179">响应</span><span class="sxs-lookup"><span data-stu-id="8ea9d-179">Response</span></span>
<span data-ttu-id="8ea9d-180">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-180">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ea9d-181">示例</span><span class="sxs-lookup"><span data-stu-id="8ea9d-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ea9d-182">请求</span><span class="sxs-lookup"><span data-stu-id="8ea9d-182">Request</span></span>
<span data-ttu-id="8ea9d-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
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

### <a name="response"></a><span data-ttu-id="8ea9d-184">响应</span><span class="sxs-lookup"><span data-stu-id="8ea9d-184">Response</span></span>
<span data-ttu-id="8ea9d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ea9d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






