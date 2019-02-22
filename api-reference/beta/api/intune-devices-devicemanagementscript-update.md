---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fafb11f61f6e98eba90de9054550e673b6d6cbdd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141788"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="90a3b-103">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="90a3b-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="90a3b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90a3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90a3b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90a3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90a3b-106">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="90a3b-106">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90a3b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="90a3b-107">Prerequisites</span></span>
<span data-ttu-id="90a3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="90a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90a3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="90a3b-110">Permission type</span></span>|<span data-ttu-id="90a3b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90a3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90a3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90a3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90a3b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90a3b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90a3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90a3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90a3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90a3b-115">Not supported.</span></span>|
|<span data-ttu-id="90a3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="90a3b-116">Application</span></span>|<span data-ttu-id="90a3b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="90a3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90a3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90a3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="90a3b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="90a3b-119">Request headers</span></span>
|<span data-ttu-id="90a3b-120">标头</span><span class="sxs-lookup"><span data-stu-id="90a3b-120">Header</span></span>|<span data-ttu-id="90a3b-121">值</span><span class="sxs-lookup"><span data-stu-id="90a3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90a3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90a3b-122">Authorization</span></span>|<span data-ttu-id="90a3b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90a3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90a3b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90a3b-124">Accept</span></span>|<span data-ttu-id="90a3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90a3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90a3b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90a3b-126">Request body</span></span>
<span data-ttu-id="90a3b-127">在请求正文中, 提供[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90a3b-127">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="90a3b-128">下表显示创建[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90a3b-128">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="90a3b-129">属性</span><span class="sxs-lookup"><span data-stu-id="90a3b-129">Property</span></span>|<span data-ttu-id="90a3b-130">类型</span><span class="sxs-lookup"><span data-stu-id="90a3b-130">Type</span></span>|<span data-ttu-id="90a3b-131">说明</span><span class="sxs-lookup"><span data-stu-id="90a3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90a3b-132">id</span><span class="sxs-lookup"><span data-stu-id="90a3b-132">id</span></span>|<span data-ttu-id="90a3b-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="90a3b-133">String</span></span>|<span data-ttu-id="90a3b-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="90a3b-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="90a3b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="90a3b-135">displayName</span></span>|<span data-ttu-id="90a3b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="90a3b-136">String</span></span>|<span data-ttu-id="90a3b-137">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="90a3b-137">Name of the device management script.</span></span>|
|<span data-ttu-id="90a3b-138">说明</span><span class="sxs-lookup"><span data-stu-id="90a3b-138">description</span></span>|<span data-ttu-id="90a3b-139">字符串</span><span class="sxs-lookup"><span data-stu-id="90a3b-139">String</span></span>|<span data-ttu-id="90a3b-140">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="90a3b-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="90a3b-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="90a3b-141">runSchedule</span></span>|[<span data-ttu-id="90a3b-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="90a3b-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="90a3b-143">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="90a3b-143">The interval for script to run.</span></span> <span data-ttu-id="90a3b-144">如果未定义, 脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="90a3b-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="90a3b-145">scriptContent</span><span class="sxs-lookup"><span data-stu-id="90a3b-145">scriptContent</span></span>|<span data-ttu-id="90a3b-146">Binary</span><span class="sxs-lookup"><span data-stu-id="90a3b-146">Binary</span></span>|<span data-ttu-id="90a3b-147">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="90a3b-147">The script content.</span></span>|
|<span data-ttu-id="90a3b-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90a3b-148">createdDateTime</span></span>|<span data-ttu-id="90a3b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a3b-149">DateTimeOffset</span></span>|<span data-ttu-id="90a3b-150">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90a3b-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="90a3b-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90a3b-151">lastModifiedDateTime</span></span>|<span data-ttu-id="90a3b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a3b-152">DateTimeOffset</span></span>|<span data-ttu-id="90a3b-153">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90a3b-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="90a3b-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="90a3b-154">runAsAccount</span></span>|[<span data-ttu-id="90a3b-155">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="90a3b-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="90a3b-156">指示设备管理脚本在其中运行的执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="90a3b-156">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="90a3b-157">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="90a3b-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="90a3b-158">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="90a3b-158">enforceSignatureCheck</span></span>|<span data-ttu-id="90a3b-159">布尔</span><span class="sxs-lookup"><span data-stu-id="90a3b-159">Boolean</span></span>|<span data-ttu-id="90a3b-160">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="90a3b-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="90a3b-161">fileName</span><span class="sxs-lookup"><span data-stu-id="90a3b-161">fileName</span></span>|<span data-ttu-id="90a3b-162">String</span><span class="sxs-lookup"><span data-stu-id="90a3b-162">String</span></span>|<span data-ttu-id="90a3b-163">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="90a3b-163">Script file name.</span></span>|
|<span data-ttu-id="90a3b-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90a3b-164">roleScopeTagIds</span></span>|<span data-ttu-id="90a3b-165">String collection</span><span class="sxs-lookup"><span data-stu-id="90a3b-165">String collection</span></span>|<span data-ttu-id="90a3b-166">此 PowerShellScript 实例的范围标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="90a3b-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="90a3b-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="90a3b-167">runAs32Bit</span></span>|<span data-ttu-id="90a3b-168">布尔</span><span class="sxs-lookup"><span data-stu-id="90a3b-168">Boolean</span></span>|<span data-ttu-id="90a3b-169">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="90a3b-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="90a3b-170">响应</span><span class="sxs-lookup"><span data-stu-id="90a3b-170">Response</span></span>
<span data-ttu-id="90a3b-171">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90a3b-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90a3b-172">示例</span><span class="sxs-lookup"><span data-stu-id="90a3b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="90a3b-173">请求</span><span class="sxs-lookup"><span data-stu-id="90a3b-173">Request</span></span>
<span data-ttu-id="90a3b-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90a3b-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90a3b-175">响应</span><span class="sxs-lookup"><span data-stu-id="90a3b-175">Response</span></span>
<span data-ttu-id="90a3b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90a3b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




