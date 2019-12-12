---
title: 更新 deviceShellScript
description: 更新 deviceShellScript 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6296caa1a6f9bf1db185bd16810f2733a30e943
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944839"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="12388-103">更新 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="12388-103">Update deviceShellScript</span></span>

> <span data-ttu-id="12388-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12388-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12388-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12388-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12388-106">更新[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12388-106">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12388-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="12388-107">Prerequisites</span></span>
<span data-ttu-id="12388-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12388-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12388-110">Permission type</span></span>|<span data-ttu-id="12388-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12388-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12388-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12388-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12388-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12388-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12388-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12388-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12388-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12388-115">Not supported.</span></span>|
|<span data-ttu-id="12388-116">Application</span><span class="sxs-lookup"><span data-stu-id="12388-116">Application</span></span>|<span data-ttu-id="12388-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12388-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12388-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12388-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="12388-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12388-119">Request headers</span></span>
|<span data-ttu-id="12388-120">标头</span><span class="sxs-lookup"><span data-stu-id="12388-120">Header</span></span>|<span data-ttu-id="12388-121">值</span><span class="sxs-lookup"><span data-stu-id="12388-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12388-122">授权</span><span class="sxs-lookup"><span data-stu-id="12388-122">Authorization</span></span>|<span data-ttu-id="12388-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12388-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12388-124">接受</span><span class="sxs-lookup"><span data-stu-id="12388-124">Accept</span></span>|<span data-ttu-id="12388-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12388-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12388-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12388-126">Request body</span></span>
<span data-ttu-id="12388-127">在请求正文中，提供[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12388-127">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="12388-128">下表显示创建[deviceShellScript](../resources/intune-devices-deviceshellscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12388-128">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="12388-129">属性</span><span class="sxs-lookup"><span data-stu-id="12388-129">Property</span></span>|<span data-ttu-id="12388-130">类型</span><span class="sxs-lookup"><span data-stu-id="12388-130">Type</span></span>|<span data-ttu-id="12388-131">说明</span><span class="sxs-lookup"><span data-stu-id="12388-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12388-132">id</span><span class="sxs-lookup"><span data-stu-id="12388-132">id</span></span>|<span data-ttu-id="12388-133">字符串</span><span class="sxs-lookup"><span data-stu-id="12388-133">String</span></span>|<span data-ttu-id="12388-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12388-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="12388-135">displayName</span><span class="sxs-lookup"><span data-stu-id="12388-135">displayName</span></span>|<span data-ttu-id="12388-136">字符串</span><span class="sxs-lookup"><span data-stu-id="12388-136">String</span></span>|<span data-ttu-id="12388-137">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="12388-137">Name of the device management script.</span></span>|
|<span data-ttu-id="12388-138">说明</span><span class="sxs-lookup"><span data-stu-id="12388-138">description</span></span>|<span data-ttu-id="12388-139">String</span><span class="sxs-lookup"><span data-stu-id="12388-139">String</span></span>|<span data-ttu-id="12388-140">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="12388-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="12388-141">scriptContent</span><span class="sxs-lookup"><span data-stu-id="12388-141">scriptContent</span></span>|<span data-ttu-id="12388-142">Binary</span><span class="sxs-lookup"><span data-stu-id="12388-142">Binary</span></span>|<span data-ttu-id="12388-143">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="12388-143">The script content.</span></span>|
|<span data-ttu-id="12388-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12388-144">createdDateTime</span></span>|<span data-ttu-id="12388-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12388-145">DateTimeOffset</span></span>|<span data-ttu-id="12388-146">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12388-146">The date and time the device management script was created.</span></span> <span data-ttu-id="12388-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="12388-147">This property is read-only.</span></span>|
|<span data-ttu-id="12388-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12388-148">lastModifiedDateTime</span></span>|<span data-ttu-id="12388-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12388-149">DateTimeOffset</span></span>|<span data-ttu-id="12388-150">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12388-150">The date and time the device management script was last modified.</span></span> <span data-ttu-id="12388-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="12388-151">This property is read-only.</span></span>|
|<span data-ttu-id="12388-152">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="12388-152">runAsAccount</span></span>|[<span data-ttu-id="12388-153">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="12388-153">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="12388-154">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="12388-154">Indicates the type of execution context.</span></span> <span data-ttu-id="12388-155">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="12388-155">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="12388-156">fileName</span><span class="sxs-lookup"><span data-stu-id="12388-156">fileName</span></span>|<span data-ttu-id="12388-157">String</span><span class="sxs-lookup"><span data-stu-id="12388-157">String</span></span>|<span data-ttu-id="12388-158">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="12388-158">Script file name.</span></span>|
|<span data-ttu-id="12388-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12388-159">roleScopeTagIds</span></span>|<span data-ttu-id="12388-160">String collection</span><span class="sxs-lookup"><span data-stu-id="12388-160">String collection</span></span>|<span data-ttu-id="12388-161">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="12388-161">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="12388-162">响应</span><span class="sxs-lookup"><span data-stu-id="12388-162">Response</span></span>
<span data-ttu-id="12388-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="12388-163">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12388-164">示例</span><span class="sxs-lookup"><span data-stu-id="12388-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="12388-165">请求</span><span class="sxs-lookup"><span data-stu-id="12388-165">Request</span></span>
<span data-ttu-id="12388-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12388-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
Content-type: application/json
Content-length: 305

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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

### <a name="response"></a><span data-ttu-id="12388-167">响应</span><span class="sxs-lookup"><span data-stu-id="12388-167">Response</span></span>
<span data-ttu-id="12388-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12388-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 477

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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





