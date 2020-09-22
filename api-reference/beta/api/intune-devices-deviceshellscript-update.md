---
title: 更新 deviceShellScript
description: 更新 deviceShellScript 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbb9e91eb2e02ae39ad77db8c5ade78656c778e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090576"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="7896c-103">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="7896c-103">Update deviceShellScript</span></span>

<span data-ttu-id="7896c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7896c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7896c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7896c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7896c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7896c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7896c-107">更新 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7896c-107">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7896c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7896c-108">Prerequisites</span></span>
<span data-ttu-id="7896c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7896c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7896c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7896c-111">Permission type</span></span>|<span data-ttu-id="7896c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7896c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7896c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7896c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7896c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7896c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7896c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7896c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7896c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7896c-116">Not supported.</span></span>|
|<span data-ttu-id="7896c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7896c-117">Application</span></span>|<span data-ttu-id="7896c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7896c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7896c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7896c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="7896c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7896c-120">Request headers</span></span>
|<span data-ttu-id="7896c-121">标头</span><span class="sxs-lookup"><span data-stu-id="7896c-121">Header</span></span>|<span data-ttu-id="7896c-122">值</span><span class="sxs-lookup"><span data-stu-id="7896c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7896c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7896c-123">Authorization</span></span>|<span data-ttu-id="7896c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7896c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7896c-125">接受</span><span class="sxs-lookup"><span data-stu-id="7896c-125">Accept</span></span>|<span data-ttu-id="7896c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7896c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7896c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7896c-127">Request body</span></span>
<span data-ttu-id="7896c-128">在请求正文中，提供 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7896c-128">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="7896c-129">下表显示创建 [deviceShellScript](../resources/intune-devices-deviceshellscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7896c-129">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="7896c-130">属性</span><span class="sxs-lookup"><span data-stu-id="7896c-130">Property</span></span>|<span data-ttu-id="7896c-131">类型</span><span class="sxs-lookup"><span data-stu-id="7896c-131">Type</span></span>|<span data-ttu-id="7896c-132">说明</span><span class="sxs-lookup"><span data-stu-id="7896c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7896c-133">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="7896c-133">executionFrequency</span></span>|<span data-ttu-id="7896c-134">持续时间</span><span class="sxs-lookup"><span data-stu-id="7896c-134">Duration</span></span>|<span data-ttu-id="7896c-135">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="7896c-135">The interval for script to run.</span></span> <span data-ttu-id="7896c-136">如果未定义，脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="7896c-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="7896c-137">retryCount</span><span class="sxs-lookup"><span data-stu-id="7896c-137">retryCount</span></span>|<span data-ttu-id="7896c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7896c-138">Int32</span></span>|<span data-ttu-id="7896c-139">脚本失败时将重试脚本的次数</span><span class="sxs-lookup"><span data-stu-id="7896c-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="7896c-140">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="7896c-140">blockExecutionNotifications</span></span>|<span data-ttu-id="7896c-141">布尔</span><span class="sxs-lookup"><span data-stu-id="7896c-141">Boolean</span></span>|<span data-ttu-id="7896c-142">不通知用户正在执行的脚本</span><span class="sxs-lookup"><span data-stu-id="7896c-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="7896c-143">id</span><span class="sxs-lookup"><span data-stu-id="7896c-143">id</span></span>|<span data-ttu-id="7896c-144">字符串</span><span class="sxs-lookup"><span data-stu-id="7896c-144">String</span></span>|<span data-ttu-id="7896c-145">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7896c-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="7896c-146">displayName</span><span class="sxs-lookup"><span data-stu-id="7896c-146">displayName</span></span>|<span data-ttu-id="7896c-147">字符串</span><span class="sxs-lookup"><span data-stu-id="7896c-147">String</span></span>|<span data-ttu-id="7896c-148">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="7896c-148">Name of the device management script.</span></span>|
|<span data-ttu-id="7896c-149">说明</span><span class="sxs-lookup"><span data-stu-id="7896c-149">description</span></span>|<span data-ttu-id="7896c-150">字符串</span><span class="sxs-lookup"><span data-stu-id="7896c-150">String</span></span>|<span data-ttu-id="7896c-151">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="7896c-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="7896c-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="7896c-152">scriptContent</span></span>|<span data-ttu-id="7896c-153">Binary</span><span class="sxs-lookup"><span data-stu-id="7896c-153">Binary</span></span>|<span data-ttu-id="7896c-154">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="7896c-154">The script content.</span></span>|
|<span data-ttu-id="7896c-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7896c-155">createdDateTime</span></span>|<span data-ttu-id="7896c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7896c-156">DateTimeOffset</span></span>|<span data-ttu-id="7896c-157">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7896c-157">The date and time the device management script was created.</span></span> <span data-ttu-id="7896c-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7896c-158">This property is read-only.</span></span>|
|<span data-ttu-id="7896c-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7896c-159">lastModifiedDateTime</span></span>|<span data-ttu-id="7896c-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7896c-160">DateTimeOffset</span></span>|<span data-ttu-id="7896c-161">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7896c-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="7896c-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7896c-162">This property is read-only.</span></span>|
|<span data-ttu-id="7896c-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="7896c-163">runAsAccount</span></span>|[<span data-ttu-id="7896c-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="7896c-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="7896c-165">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="7896c-165">Indicates the type of execution context.</span></span> <span data-ttu-id="7896c-166">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="7896c-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="7896c-167">fileName</span><span class="sxs-lookup"><span data-stu-id="7896c-167">fileName</span></span>|<span data-ttu-id="7896c-168">String</span><span class="sxs-lookup"><span data-stu-id="7896c-168">String</span></span>|<span data-ttu-id="7896c-169">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="7896c-169">Script file name.</span></span>|
|<span data-ttu-id="7896c-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7896c-170">roleScopeTagIds</span></span>|<span data-ttu-id="7896c-171">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7896c-171">String collection</span></span>|<span data-ttu-id="7896c-172">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="7896c-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="7896c-173">响应</span><span class="sxs-lookup"><span data-stu-id="7896c-173">Response</span></span>
<span data-ttu-id="7896c-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7896c-174">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7896c-175">示例</span><span class="sxs-lookup"><span data-stu-id="7896c-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="7896c-176">请求</span><span class="sxs-lookup"><span data-stu-id="7896c-176">Request</span></span>
<span data-ttu-id="7896c-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7896c-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7896c-178">响应</span><span class="sxs-lookup"><span data-stu-id="7896c-178">Response</span></span>
<span data-ttu-id="7896c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7896c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






