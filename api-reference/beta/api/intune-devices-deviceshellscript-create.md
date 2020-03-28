---
title: 创建 deviceShellScript
description: 创建新的 deviceShellScript 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f310a1b2b83effda2af1a2a73406325f78a06f3d
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034753"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="ff639-103">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="ff639-103">Create deviceShellScript</span></span>

> <span data-ttu-id="ff639-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff639-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff639-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff639-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff639-106">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff639-106">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff639-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff639-107">Prerequisites</span></span>
<span data-ttu-id="ff639-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff639-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff639-110">Permission type</span></span>|<span data-ttu-id="ff639-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff639-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff639-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff639-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff639-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff639-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ff639-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff639-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff639-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff639-115">Not supported.</span></span>|
|<span data-ttu-id="ff639-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff639-116">Application</span></span>|<span data-ttu-id="ff639-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff639-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff639-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff639-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="ff639-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff639-119">Request headers</span></span>
|<span data-ttu-id="ff639-120">标头</span><span class="sxs-lookup"><span data-stu-id="ff639-120">Header</span></span>|<span data-ttu-id="ff639-121">值</span><span class="sxs-lookup"><span data-stu-id="ff639-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff639-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff639-122">Authorization</span></span>|<span data-ttu-id="ff639-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff639-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff639-124">接受</span><span class="sxs-lookup"><span data-stu-id="ff639-124">Accept</span></span>|<span data-ttu-id="ff639-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff639-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff639-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff639-126">Request body</span></span>
<span data-ttu-id="ff639-127">在请求正文中，提供 deviceShellScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff639-127">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="ff639-128">下表显示创建 deviceShellScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ff639-128">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="ff639-129">属性</span><span class="sxs-lookup"><span data-stu-id="ff639-129">Property</span></span>|<span data-ttu-id="ff639-130">类型</span><span class="sxs-lookup"><span data-stu-id="ff639-130">Type</span></span>|<span data-ttu-id="ff639-131">Description</span><span class="sxs-lookup"><span data-stu-id="ff639-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff639-132">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="ff639-132">executionFrequency</span></span>|<span data-ttu-id="ff639-133">持续时间</span><span class="sxs-lookup"><span data-stu-id="ff639-133">Duration</span></span>|<span data-ttu-id="ff639-134">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="ff639-134">The interval for the script to run.</span></span> <span data-ttu-id="ff639-135">如果未定义，则脚本将运行一次。</span><span class="sxs-lookup"><span data-stu-id="ff639-135">If not defined, the script runs once.</span></span>|
|<span data-ttu-id="ff639-136">retryCount</span><span class="sxs-lookup"><span data-stu-id="ff639-136">retryCount</span></span>|<span data-ttu-id="ff639-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ff639-137">Int32</span></span>| <span data-ttu-id="ff639-138">脚本失败时重试脚本的次数。</span><span class="sxs-lookup"><span data-stu-id="ff639-138">The number of times for the script to be retried if it fails.</span></span> |
|<span data-ttu-id="ff639-139">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="ff639-139">blockExecutionNotifications</span></span>|<span data-ttu-id="ff639-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff639-140">Boolean</span></span>|<span data-ttu-id="ff639-141">指示在执行脚本时是否通知用户。</span><span class="sxs-lookup"><span data-stu-id="ff639-141">Indicates whether the user is notified when a script is being executed.</span></span>|
|<span data-ttu-id="ff639-142">id</span><span class="sxs-lookup"><span data-stu-id="ff639-142">id</span></span>|<span data-ttu-id="ff639-143">字符串</span><span class="sxs-lookup"><span data-stu-id="ff639-143">String</span></span>|<span data-ttu-id="ff639-144">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ff639-144">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="ff639-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ff639-145">displayName</span></span>|<span data-ttu-id="ff639-146">字符串</span><span class="sxs-lookup"><span data-stu-id="ff639-146">String</span></span>|<span data-ttu-id="ff639-147">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="ff639-147">Name of the device management script.</span></span>|
|<span data-ttu-id="ff639-148">description</span><span class="sxs-lookup"><span data-stu-id="ff639-148">description</span></span>|<span data-ttu-id="ff639-149">String</span><span class="sxs-lookup"><span data-stu-id="ff639-149">String</span></span>|<span data-ttu-id="ff639-150">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="ff639-150">Optional description for the device management script.</span></span>|
|<span data-ttu-id="ff639-151">scriptContent</span><span class="sxs-lookup"><span data-stu-id="ff639-151">scriptContent</span></span>|<span data-ttu-id="ff639-152">Binary</span><span class="sxs-lookup"><span data-stu-id="ff639-152">Binary</span></span>|<span data-ttu-id="ff639-153">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="ff639-153">The script content.</span></span>|
|<span data-ttu-id="ff639-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff639-154">createdDateTime</span></span>|<span data-ttu-id="ff639-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff639-155">DateTimeOffset</span></span>|<span data-ttu-id="ff639-156">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff639-156">The date and time the device management script was created.</span></span> <span data-ttu-id="ff639-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ff639-157">This property is read-only.</span></span>|
|<span data-ttu-id="ff639-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff639-158">lastModifiedDateTime</span></span>|<span data-ttu-id="ff639-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff639-159">DateTimeOffset</span></span>|<span data-ttu-id="ff639-160">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff639-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="ff639-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ff639-161">This property is read-only.</span></span>|
|<span data-ttu-id="ff639-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="ff639-162">runAsAccount</span></span>|[<span data-ttu-id="ff639-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="ff639-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="ff639-164">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="ff639-164">Indicates the type of execution context.</span></span> <span data-ttu-id="ff639-165">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="ff639-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="ff639-166">fileName</span><span class="sxs-lookup"><span data-stu-id="ff639-166">fileName</span></span>|<span data-ttu-id="ff639-167">String</span><span class="sxs-lookup"><span data-stu-id="ff639-167">String</span></span>|<span data-ttu-id="ff639-168">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="ff639-168">The script file name.</span></span>|
|<span data-ttu-id="ff639-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff639-169">roleScopeTagIds</span></span>|<span data-ttu-id="ff639-170">String 集合</span><span class="sxs-lookup"><span data-stu-id="ff639-170">String collection</span></span>|<span data-ttu-id="ff639-171">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="ff639-171">The list of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="ff639-172">响应</span><span class="sxs-lookup"><span data-stu-id="ff639-172">Response</span></span>
<span data-ttu-id="ff639-173">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff639-173">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff639-174">示例</span><span class="sxs-lookup"><span data-stu-id="ff639-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff639-175">请求</span><span class="sxs-lookup"><span data-stu-id="ff639-175">Request</span></span>
<span data-ttu-id="ff639-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff639-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ff639-177">响应</span><span class="sxs-lookup"><span data-stu-id="ff639-177">Response</span></span>
<span data-ttu-id="ff639-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff639-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "id": "ca9e0ad8-0ad8-ca9e-d80a-9ecad80a9eca",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



