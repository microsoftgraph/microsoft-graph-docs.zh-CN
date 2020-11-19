---
title: 更新 deviceShellScript
description: 更新 deviceShellScript 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2791932af6b9c9e4963dd5fa1da66a32876c1541
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228510"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="c3560-103">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="c3560-103">Update deviceShellScript</span></span>

<span data-ttu-id="c3560-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3560-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3560-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3560-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3560-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3560-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3560-107">更新 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3560-107">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3560-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3560-108">Prerequisites</span></span>
<span data-ttu-id="c3560-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3560-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3560-111">Permission type</span></span>|<span data-ttu-id="c3560-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3560-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3560-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3560-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3560-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3560-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c3560-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3560-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3560-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3560-116">Not supported.</span></span>|
|<span data-ttu-id="c3560-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3560-117">Application</span></span>|<span data-ttu-id="c3560-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3560-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3560-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3560-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="c3560-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3560-120">Request headers</span></span>
|<span data-ttu-id="c3560-121">标头</span><span class="sxs-lookup"><span data-stu-id="c3560-121">Header</span></span>|<span data-ttu-id="c3560-122">值</span><span class="sxs-lookup"><span data-stu-id="c3560-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3560-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3560-123">Authorization</span></span>|<span data-ttu-id="c3560-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3560-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3560-125">接受</span><span class="sxs-lookup"><span data-stu-id="c3560-125">Accept</span></span>|<span data-ttu-id="c3560-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3560-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3560-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3560-127">Request body</span></span>
<span data-ttu-id="c3560-128">在请求正文中，提供 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3560-128">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="c3560-129">下表显示创建 [deviceShellScript](../resources/intune-devices-deviceshellscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3560-129">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="c3560-130">属性</span><span class="sxs-lookup"><span data-stu-id="c3560-130">Property</span></span>|<span data-ttu-id="c3560-131">类型</span><span class="sxs-lookup"><span data-stu-id="c3560-131">Type</span></span>|<span data-ttu-id="c3560-132">说明</span><span class="sxs-lookup"><span data-stu-id="c3560-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3560-133">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="c3560-133">executionFrequency</span></span>|<span data-ttu-id="c3560-134">持续时间</span><span class="sxs-lookup"><span data-stu-id="c3560-134">Duration</span></span>|<span data-ttu-id="c3560-135">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="c3560-135">The interval for script to run.</span></span> <span data-ttu-id="c3560-136">如果未定义，脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="c3560-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="c3560-137">retryCount</span><span class="sxs-lookup"><span data-stu-id="c3560-137">retryCount</span></span>|<span data-ttu-id="c3560-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c3560-138">Int32</span></span>|<span data-ttu-id="c3560-139">脚本失败时将重试脚本的次数</span><span class="sxs-lookup"><span data-stu-id="c3560-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="c3560-140">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="c3560-140">blockExecutionNotifications</span></span>|<span data-ttu-id="c3560-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3560-141">Boolean</span></span>|<span data-ttu-id="c3560-142">不通知用户正在执行的脚本</span><span class="sxs-lookup"><span data-stu-id="c3560-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="c3560-143">id</span><span class="sxs-lookup"><span data-stu-id="c3560-143">id</span></span>|<span data-ttu-id="c3560-144">String</span><span class="sxs-lookup"><span data-stu-id="c3560-144">String</span></span>|<span data-ttu-id="c3560-145">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c3560-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="c3560-146">displayName</span><span class="sxs-lookup"><span data-stu-id="c3560-146">displayName</span></span>|<span data-ttu-id="c3560-147">String</span><span class="sxs-lookup"><span data-stu-id="c3560-147">String</span></span>|<span data-ttu-id="c3560-148">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="c3560-148">Name of the device management script.</span></span>|
|<span data-ttu-id="c3560-149">description</span><span class="sxs-lookup"><span data-stu-id="c3560-149">description</span></span>|<span data-ttu-id="c3560-150">String</span><span class="sxs-lookup"><span data-stu-id="c3560-150">String</span></span>|<span data-ttu-id="c3560-151">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="c3560-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="c3560-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="c3560-152">scriptContent</span></span>|<span data-ttu-id="c3560-153">Binary</span><span class="sxs-lookup"><span data-stu-id="c3560-153">Binary</span></span>|<span data-ttu-id="c3560-154">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="c3560-154">The script content.</span></span>|
|<span data-ttu-id="c3560-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3560-155">createdDateTime</span></span>|<span data-ttu-id="c3560-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3560-156">DateTimeOffset</span></span>|<span data-ttu-id="c3560-157">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c3560-157">The date and time the device management script was created.</span></span> <span data-ttu-id="c3560-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c3560-158">This property is read-only.</span></span>|
|<span data-ttu-id="c3560-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3560-159">lastModifiedDateTime</span></span>|<span data-ttu-id="c3560-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3560-160">DateTimeOffset</span></span>|<span data-ttu-id="c3560-161">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c3560-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="c3560-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c3560-162">This property is read-only.</span></span>|
|<span data-ttu-id="c3560-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c3560-163">runAsAccount</span></span>|[<span data-ttu-id="c3560-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c3560-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c3560-165">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="c3560-165">Indicates the type of execution context.</span></span> <span data-ttu-id="c3560-166">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="c3560-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c3560-167">fileName</span><span class="sxs-lookup"><span data-stu-id="c3560-167">fileName</span></span>|<span data-ttu-id="c3560-168">String</span><span class="sxs-lookup"><span data-stu-id="c3560-168">String</span></span>|<span data-ttu-id="c3560-169">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="c3560-169">Script file name.</span></span>|
|<span data-ttu-id="c3560-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3560-170">roleScopeTagIds</span></span>|<span data-ttu-id="c3560-171">String 集合</span><span class="sxs-lookup"><span data-stu-id="c3560-171">String collection</span></span>|<span data-ttu-id="c3560-172">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="c3560-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c3560-173">响应</span><span class="sxs-lookup"><span data-stu-id="c3560-173">Response</span></span>
<span data-ttu-id="c3560-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceShellScript](../resources/intune-devices-deviceshellscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3560-174">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3560-175">示例</span><span class="sxs-lookup"><span data-stu-id="c3560-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3560-176">请求</span><span class="sxs-lookup"><span data-stu-id="c3560-176">Request</span></span>
<span data-ttu-id="c3560-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3560-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3560-178">响应</span><span class="sxs-lookup"><span data-stu-id="c3560-178">Response</span></span>
<span data-ttu-id="c3560-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3560-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




