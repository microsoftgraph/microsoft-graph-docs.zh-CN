---
title: 更新 deviceManagementScript
description: 更新 deviceManagementScript 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8cb1b6978922f99ae357cabe7fbc6d19a58fa2a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959038"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="f4406-103">更新 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="f4406-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="f4406-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4406-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4406-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4406-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4406-106">更新[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4406-106">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4406-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4406-107">Prerequisites</span></span>
<span data-ttu-id="f4406-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4406-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4406-110">Permission type</span></span>|<span data-ttu-id="f4406-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4406-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4406-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4406-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4406-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4406-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4406-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4406-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4406-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4406-115">Not supported.</span></span>|
|<span data-ttu-id="f4406-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4406-116">Application</span></span>|<span data-ttu-id="f4406-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4406-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4406-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4406-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="f4406-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4406-119">Request headers</span></span>
|<span data-ttu-id="f4406-120">标头</span><span class="sxs-lookup"><span data-stu-id="f4406-120">Header</span></span>|<span data-ttu-id="f4406-121">值</span><span class="sxs-lookup"><span data-stu-id="f4406-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4406-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4406-122">Authorization</span></span>|<span data-ttu-id="f4406-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4406-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4406-124">接受</span><span class="sxs-lookup"><span data-stu-id="f4406-124">Accept</span></span>|<span data-ttu-id="f4406-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4406-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4406-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4406-126">Request body</span></span>
<span data-ttu-id="f4406-127">在请求正文中, 提供[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4406-127">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="f4406-128">下表显示创建[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4406-128">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="f4406-129">属性</span><span class="sxs-lookup"><span data-stu-id="f4406-129">Property</span></span>|<span data-ttu-id="f4406-130">类型</span><span class="sxs-lookup"><span data-stu-id="f4406-130">Type</span></span>|<span data-ttu-id="f4406-131">说明</span><span class="sxs-lookup"><span data-stu-id="f4406-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4406-132">id</span><span class="sxs-lookup"><span data-stu-id="f4406-132">id</span></span>|<span data-ttu-id="f4406-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f4406-133">String</span></span>|<span data-ttu-id="f4406-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4406-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="f4406-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f4406-135">displayName</span></span>|<span data-ttu-id="f4406-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f4406-136">String</span></span>|<span data-ttu-id="f4406-137">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="f4406-137">Name of the device management script.</span></span>|
|<span data-ttu-id="f4406-138">说明</span><span class="sxs-lookup"><span data-stu-id="f4406-138">description</span></span>|<span data-ttu-id="f4406-139">String</span><span class="sxs-lookup"><span data-stu-id="f4406-139">String</span></span>|<span data-ttu-id="f4406-140">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="f4406-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="f4406-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="f4406-141">runSchedule</span></span>|[<span data-ttu-id="f4406-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="f4406-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="f4406-143">脚本运行的间隔。</span><span class="sxs-lookup"><span data-stu-id="f4406-143">The interval for script to run.</span></span> <span data-ttu-id="f4406-144">如果未定义, 脚本将运行一次</span><span class="sxs-lookup"><span data-stu-id="f4406-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="f4406-145">scriptContent</span><span class="sxs-lookup"><span data-stu-id="f4406-145">scriptContent</span></span>|<span data-ttu-id="f4406-146">Binary</span><span class="sxs-lookup"><span data-stu-id="f4406-146">Binary</span></span>|<span data-ttu-id="f4406-147">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="f4406-147">The script content.</span></span>|
|<span data-ttu-id="f4406-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4406-148">createdDateTime</span></span>|<span data-ttu-id="f4406-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4406-149">DateTimeOffset</span></span>|<span data-ttu-id="f4406-150">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f4406-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="f4406-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4406-151">lastModifiedDateTime</span></span>|<span data-ttu-id="f4406-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4406-152">DateTimeOffset</span></span>|<span data-ttu-id="f4406-153">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f4406-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="f4406-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f4406-154">runAsAccount</span></span>|[<span data-ttu-id="f4406-155">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f4406-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f4406-156">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="f4406-156">Indicates the type of execution context.</span></span> <span data-ttu-id="f4406-157">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f4406-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="f4406-158">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="f4406-158">enforceSignatureCheck</span></span>|<span data-ttu-id="f4406-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4406-159">Boolean</span></span>|<span data-ttu-id="f4406-160">指示是否需要检查脚本签名。</span><span class="sxs-lookup"><span data-stu-id="f4406-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="f4406-161">fileName</span><span class="sxs-lookup"><span data-stu-id="f4406-161">fileName</span></span>|<span data-ttu-id="f4406-162">String</span><span class="sxs-lookup"><span data-stu-id="f4406-162">String</span></span>|<span data-ttu-id="f4406-163">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="f4406-163">Script file name.</span></span>|
|<span data-ttu-id="f4406-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4406-164">roleScopeTagIds</span></span>|<span data-ttu-id="f4406-165">String collection</span><span class="sxs-lookup"><span data-stu-id="f4406-165">String collection</span></span>|<span data-ttu-id="f4406-166">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="f4406-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="f4406-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="f4406-167">runAs32Bit</span></span>|<span data-ttu-id="f4406-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4406-168">Boolean</span></span>|<span data-ttu-id="f4406-169">一个指示 PowerShell 脚本是否应作为32位运行的值</span><span class="sxs-lookup"><span data-stu-id="f4406-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="f4406-170">响应</span><span class="sxs-lookup"><span data-stu-id="f4406-170">Response</span></span>
<span data-ttu-id="f4406-171">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4406-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4406-172">示例</span><span class="sxs-lookup"><span data-stu-id="f4406-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4406-173">请求</span><span class="sxs-lookup"><span data-stu-id="f4406-173">Request</span></span>
<span data-ttu-id="f4406-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4406-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4406-175">响应</span><span class="sxs-lookup"><span data-stu-id="f4406-175">Response</span></span>
<span data-ttu-id="f4406-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4406-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





