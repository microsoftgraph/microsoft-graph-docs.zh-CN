---
title: 更新 deviceShellScript
description: 更新 deviceShellScript 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9e3c2da2008b5e44f4b13449abd6b63251fe08f
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034746"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="2d13e-103">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="2d13e-103">Update deviceShellScript</span></span>

> <span data-ttu-id="2d13e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d13e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d13e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d13e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d13e-106">更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2d13e-106">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d13e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d13e-107">Prerequisites</span></span>
<span data-ttu-id="2d13e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d13e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d13e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d13e-110">Permission type</span></span>|<span data-ttu-id="2d13e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d13e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d13e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d13e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d13e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d13e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2d13e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d13e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d13e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d13e-115">Not supported.</span></span>|
|<span data-ttu-id="2d13e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d13e-116">Application</span></span>|<span data-ttu-id="2d13e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d13e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d13e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d13e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="2d13e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d13e-119">Request headers</span></span>
|<span data-ttu-id="2d13e-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d13e-120">Header</span></span>|<span data-ttu-id="2d13e-121">值</span><span class="sxs-lookup"><span data-stu-id="2d13e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d13e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d13e-122">Authorization</span></span>|<span data-ttu-id="2d13e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d13e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d13e-124">接受</span><span class="sxs-lookup"><span data-stu-id="2d13e-124">Accept</span></span>|<span data-ttu-id="2d13e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d13e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d13e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d13e-126">Request body</span></span>
<span data-ttu-id="2d13e-127">在请求正文中，提供[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d13e-127">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="2d13e-128">下表显示创建[deviceShellScript](../resources/intune-devices-deviceshellscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d13e-128">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="2d13e-129">属性</span><span class="sxs-lookup"><span data-stu-id="2d13e-129">Property</span></span>|<span data-ttu-id="2d13e-130">类型</span><span class="sxs-lookup"><span data-stu-id="2d13e-130">Type</span></span>|<span data-ttu-id="2d13e-131">Description</span><span class="sxs-lookup"><span data-stu-id="2d13e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d13e-132">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="2d13e-132">executionFrequency</span></span>|<span data-ttu-id="2d13e-133">持续时间</span><span class="sxs-lookup"><span data-stu-id="2d13e-133">Duration</span></span>|<span data-ttu-id="2d13e-134">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="2d13e-134">The interval for script to run.</span></span> <span data-ttu-id="2d13e-135">如果未定义，则脚本将运行一次。</span><span class="sxs-lookup"><span data-stu-id="2d13e-135">If not defined, the script runs once.</span></span>|
|<span data-ttu-id="2d13e-136">retryCount</span><span class="sxs-lookup"><span data-stu-id="2d13e-136">retryCount</span></span>|<span data-ttu-id="2d13e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2d13e-137">Int32</span></span>|<span data-ttu-id="2d13e-138">脚本失败时重试脚本的次数。</span><span class="sxs-lookup"><span data-stu-id="2d13e-138">The number of times for the script to be retried if it fails.</span></span>|
|<span data-ttu-id="2d13e-139">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="2d13e-139">blockExecutionNotifications</span></span>|<span data-ttu-id="2d13e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d13e-140">Boolean</span></span>|<span data-ttu-id="2d13e-141">指示在脚本运行时是否通知用户。</span><span class="sxs-lookup"><span data-stu-id="2d13e-141">Indicates whether the user is notified when a script runs.</span></span>|
|<span data-ttu-id="2d13e-142">id</span><span class="sxs-lookup"><span data-stu-id="2d13e-142">id</span></span>|<span data-ttu-id="2d13e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="2d13e-143">String</span></span>|<span data-ttu-id="2d13e-144">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2d13e-144">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="2d13e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2d13e-145">displayName</span></span>|<span data-ttu-id="2d13e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="2d13e-146">String</span></span>|<span data-ttu-id="2d13e-147">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="2d13e-147">The name of the device management script.</span></span>|
|<span data-ttu-id="2d13e-148">description</span><span class="sxs-lookup"><span data-stu-id="2d13e-148">description</span></span>|<span data-ttu-id="2d13e-149">String</span><span class="sxs-lookup"><span data-stu-id="2d13e-149">String</span></span>|<span data-ttu-id="2d13e-150">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="2d13e-150">Optional description for the device management script.</span></span>|
|<span data-ttu-id="2d13e-151">scriptContent</span><span class="sxs-lookup"><span data-stu-id="2d13e-151">scriptContent</span></span>|<span data-ttu-id="2d13e-152">Binary</span><span class="sxs-lookup"><span data-stu-id="2d13e-152">Binary</span></span>|<span data-ttu-id="2d13e-153">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="2d13e-153">The script content.</span></span>|
|<span data-ttu-id="2d13e-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d13e-154">createdDateTime</span></span>|<span data-ttu-id="2d13e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d13e-155">DateTimeOffset</span></span>|<span data-ttu-id="2d13e-156">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2d13e-156">The date and time the device management script was created.</span></span> <span data-ttu-id="2d13e-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2d13e-157">This property is read-only.</span></span>|
|<span data-ttu-id="2d13e-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d13e-158">lastModifiedDateTime</span></span>|<span data-ttu-id="2d13e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d13e-159">DateTimeOffset</span></span>|<span data-ttu-id="2d13e-160">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2d13e-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="2d13e-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2d13e-161">This property is read-only.</span></span>|
|<span data-ttu-id="2d13e-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="2d13e-162">runAsAccount</span></span>|[<span data-ttu-id="2d13e-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="2d13e-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="2d13e-164">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="2d13e-164">Indicates the type of execution context.</span></span> <span data-ttu-id="2d13e-165">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="2d13e-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="2d13e-166">fileName</span><span class="sxs-lookup"><span data-stu-id="2d13e-166">fileName</span></span>|<span data-ttu-id="2d13e-167">String</span><span class="sxs-lookup"><span data-stu-id="2d13e-167">String</span></span>|<span data-ttu-id="2d13e-168">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="2d13e-168">The script file name.</span></span>|
|<span data-ttu-id="2d13e-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d13e-169">roleScopeTagIds</span></span>|<span data-ttu-id="2d13e-170">String 集合</span><span class="sxs-lookup"><span data-stu-id="2d13e-170">String collection</span></span>|<span data-ttu-id="2d13e-171">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="2d13e-171">The list of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2d13e-172">响应</span><span class="sxs-lookup"><span data-stu-id="2d13e-172">Response</span></span>
<span data-ttu-id="2d13e-173">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d13e-173">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d13e-174">示例</span><span class="sxs-lookup"><span data-stu-id="2d13e-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d13e-175">请求</span><span class="sxs-lookup"><span data-stu-id="2d13e-175">Request</span></span>
<span data-ttu-id="2d13e-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d13e-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
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

### <a name="response"></a><span data-ttu-id="2d13e-177">响应</span><span class="sxs-lookup"><span data-stu-id="2d13e-177">Response</span></span>
<span data-ttu-id="2d13e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d13e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



