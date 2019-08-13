---
title: 创建 deviceManagementScript
description: 创建新的 deviceManagementScript 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e83d34f519093dbc6e7b70a2cda385be7426d2c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310540"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="4549a-103">创建 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="4549a-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="4549a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4549a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4549a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4549a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4549a-106">创建新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4549a-106">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4549a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4549a-107">Prerequisites</span></span>
<span data-ttu-id="4549a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4549a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4549a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4549a-110">Permission type</span></span>|<span data-ttu-id="4549a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4549a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4549a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4549a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4549a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4549a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4549a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4549a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4549a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4549a-115">Not supported.</span></span>|
|<span data-ttu-id="4549a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4549a-116">Application</span></span>|<span data-ttu-id="4549a-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4549a-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4549a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4549a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="4549a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4549a-119">Request headers</span></span>
|<span data-ttu-id="4549a-120">标头</span><span class="sxs-lookup"><span data-stu-id="4549a-120">Header</span></span>|<span data-ttu-id="4549a-121">值</span><span class="sxs-lookup"><span data-stu-id="4549a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4549a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4549a-122">Authorization</span></span>|<span data-ttu-id="4549a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4549a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4549a-124">接受</span><span class="sxs-lookup"><span data-stu-id="4549a-124">Accept</span></span>|<span data-ttu-id="4549a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4549a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4549a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4549a-126">Request body</span></span>
<span data-ttu-id="4549a-127">在请求正文中, 提供 deviceManagementScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4549a-127">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="4549a-128">下表显示创建 deviceManagementScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4549a-128">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="4549a-129">属性</span><span class="sxs-lookup"><span data-stu-id="4549a-129">Property</span></span>|<span data-ttu-id="4549a-130">类型</span><span class="sxs-lookup"><span data-stu-id="4549a-130">Type</span></span>|<span data-ttu-id="4549a-131">说明</span><span class="sxs-lookup"><span data-stu-id="4549a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4549a-132">id</span><span class="sxs-lookup"><span data-stu-id="4549a-132">id</span></span>|<span data-ttu-id="4549a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4549a-133">String</span></span>|<span data-ttu-id="4549a-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4549a-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="4549a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4549a-135">displayName</span></span>|<span data-ttu-id="4549a-136">字符串</span><span class="sxs-lookup"><span data-stu-id="4549a-136">String</span></span>|<span data-ttu-id="4549a-137">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="4549a-137">Name of the device management script.</span></span>|
|<span data-ttu-id="4549a-138">说明</span><span class="sxs-lookup"><span data-stu-id="4549a-138">description</span></span>|<span data-ttu-id="4549a-139">String</span><span class="sxs-lookup"><span data-stu-id="4549a-139">String</span></span>|<span data-ttu-id="4549a-140">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="4549a-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="4549a-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="4549a-141">runSchedule</span></span>|[<span data-ttu-id="4549a-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="4549a-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="4549a-143">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="4549a-143">The interval for script to run.</span></span> <span data-ttu-id="4549a-144">如果未定义, 脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="4549a-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="4549a-145">scriptContent</span><span class="sxs-lookup"><span data-stu-id="4549a-145">scriptContent</span></span>|<span data-ttu-id="4549a-146">Binary</span><span class="sxs-lookup"><span data-stu-id="4549a-146">Binary</span></span>|<span data-ttu-id="4549a-147">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="4549a-147">The script content.</span></span>|
|<span data-ttu-id="4549a-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4549a-148">createdDateTime</span></span>|<span data-ttu-id="4549a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4549a-149">DateTimeOffset</span></span>|<span data-ttu-id="4549a-150">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4549a-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="4549a-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4549a-151">lastModifiedDateTime</span></span>|<span data-ttu-id="4549a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4549a-152">DateTimeOffset</span></span>|<span data-ttu-id="4549a-153">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4549a-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="4549a-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="4549a-154">runAsAccount</span></span>|[<span data-ttu-id="4549a-155">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="4549a-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="4549a-156">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="4549a-156">Indicates the type of execution context.</span></span> <span data-ttu-id="4549a-157">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="4549a-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="4549a-158">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="4549a-158">enforceSignatureCheck</span></span>|<span data-ttu-id="4549a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="4549a-159">Boolean</span></span>|<span data-ttu-id="4549a-160">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="4549a-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="4549a-161">fileName</span><span class="sxs-lookup"><span data-stu-id="4549a-161">fileName</span></span>|<span data-ttu-id="4549a-162">String</span><span class="sxs-lookup"><span data-stu-id="4549a-162">String</span></span>|<span data-ttu-id="4549a-163">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="4549a-163">Script file name.</span></span>|
|<span data-ttu-id="4549a-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4549a-164">roleScopeTagIds</span></span>|<span data-ttu-id="4549a-165">String collection</span><span class="sxs-lookup"><span data-stu-id="4549a-165">String collection</span></span>|<span data-ttu-id="4549a-166">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="4549a-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="4549a-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="4549a-167">runAs32Bit</span></span>|<span data-ttu-id="4549a-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4549a-168">Boolean</span></span>|<span data-ttu-id="4549a-169">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="4549a-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="4549a-170">响应</span><span class="sxs-lookup"><span data-stu-id="4549a-170">Response</span></span>
<span data-ttu-id="4549a-171">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4549a-171">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4549a-172">示例</span><span class="sxs-lookup"><span data-stu-id="4549a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4549a-173">请求</span><span class="sxs-lookup"><span data-stu-id="4549a-173">Request</span></span>
<span data-ttu-id="4549a-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4549a-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4549a-175">响应</span><span class="sxs-lookup"><span data-stu-id="4549a-175">Response</span></span>
<span data-ttu-id="4549a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4549a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






