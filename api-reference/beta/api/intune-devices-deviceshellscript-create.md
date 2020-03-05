---
title: 创建 deviceShellScript
description: 创建新的 deviceShellScript 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 662d0be06b4a714a271e12b1e813aa09f5c76187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469158"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="f0b60-103">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f0b60-103">Create deviceShellScript</span></span>

<span data-ttu-id="f0b60-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0b60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0b60-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0b60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0b60-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0b60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0b60-107">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0b60-107">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0b60-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0b60-108">Prerequisites</span></span>
<span data-ttu-id="f0b60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0b60-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0b60-111">Permission type</span></span>|<span data-ttu-id="f0b60-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0b60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0b60-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0b60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0b60-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0b60-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f0b60-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0b60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0b60-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0b60-116">Not supported.</span></span>|
|<span data-ttu-id="f0b60-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0b60-117">Application</span></span>|<span data-ttu-id="f0b60-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0b60-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0b60-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0b60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="f0b60-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0b60-120">Request headers</span></span>
|<span data-ttu-id="f0b60-121">标头</span><span class="sxs-lookup"><span data-stu-id="f0b60-121">Header</span></span>|<span data-ttu-id="f0b60-122">值</span><span class="sxs-lookup"><span data-stu-id="f0b60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0b60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0b60-123">Authorization</span></span>|<span data-ttu-id="f0b60-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0b60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0b60-125">接受</span><span class="sxs-lookup"><span data-stu-id="f0b60-125">Accept</span></span>|<span data-ttu-id="f0b60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0b60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0b60-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0b60-127">Request body</span></span>
<span data-ttu-id="f0b60-128">在请求正文中，提供 deviceShellScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0b60-128">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="f0b60-129">下表显示创建 deviceShellScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f0b60-129">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="f0b60-130">属性</span><span class="sxs-lookup"><span data-stu-id="f0b60-130">Property</span></span>|<span data-ttu-id="f0b60-131">类型</span><span class="sxs-lookup"><span data-stu-id="f0b60-131">Type</span></span>|<span data-ttu-id="f0b60-132">说明</span><span class="sxs-lookup"><span data-stu-id="f0b60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b60-133">id</span><span class="sxs-lookup"><span data-stu-id="f0b60-133">id</span></span>|<span data-ttu-id="f0b60-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f0b60-134">String</span></span>|<span data-ttu-id="f0b60-135">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f0b60-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="f0b60-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f0b60-136">displayName</span></span>|<span data-ttu-id="f0b60-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f0b60-137">String</span></span>|<span data-ttu-id="f0b60-138">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="f0b60-138">Name of the device management script.</span></span>|
|<span data-ttu-id="f0b60-139">说明</span><span class="sxs-lookup"><span data-stu-id="f0b60-139">description</span></span>|<span data-ttu-id="f0b60-140">String</span><span class="sxs-lookup"><span data-stu-id="f0b60-140">String</span></span>|<span data-ttu-id="f0b60-141">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="f0b60-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="f0b60-142">scriptContent</span><span class="sxs-lookup"><span data-stu-id="f0b60-142">scriptContent</span></span>|<span data-ttu-id="f0b60-143">Binary</span><span class="sxs-lookup"><span data-stu-id="f0b60-143">Binary</span></span>|<span data-ttu-id="f0b60-144">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="f0b60-144">The script content.</span></span>|
|<span data-ttu-id="f0b60-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0b60-145">createdDateTime</span></span>|<span data-ttu-id="f0b60-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0b60-146">DateTimeOffset</span></span>|<span data-ttu-id="f0b60-147">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f0b60-147">The date and time the device management script was created.</span></span> <span data-ttu-id="f0b60-148">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f0b60-148">This property is read-only.</span></span>|
|<span data-ttu-id="f0b60-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0b60-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f0b60-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0b60-150">DateTimeOffset</span></span>|<span data-ttu-id="f0b60-151">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f0b60-151">The date and time the device management script was last modified.</span></span> <span data-ttu-id="f0b60-152">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f0b60-152">This property is read-only.</span></span>|
|<span data-ttu-id="f0b60-153">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f0b60-153">runAsAccount</span></span>|[<span data-ttu-id="f0b60-154">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f0b60-154">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f0b60-155">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="f0b60-155">Indicates the type of execution context.</span></span> <span data-ttu-id="f0b60-156">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f0b60-156">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="f0b60-157">fileName</span><span class="sxs-lookup"><span data-stu-id="f0b60-157">fileName</span></span>|<span data-ttu-id="f0b60-158">String</span><span class="sxs-lookup"><span data-stu-id="f0b60-158">String</span></span>|<span data-ttu-id="f0b60-159">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="f0b60-159">Script file name.</span></span>|
|<span data-ttu-id="f0b60-160">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0b60-160">roleScopeTagIds</span></span>|<span data-ttu-id="f0b60-161">String 集合</span><span class="sxs-lookup"><span data-stu-id="f0b60-161">String collection</span></span>|<span data-ttu-id="f0b60-162">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="f0b60-162">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="f0b60-163">响应</span><span class="sxs-lookup"><span data-stu-id="f0b60-163">Response</span></span>
<span data-ttu-id="f0b60-164">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0b60-164">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0b60-165">示例</span><span class="sxs-lookup"><span data-stu-id="f0b60-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0b60-166">请求</span><span class="sxs-lookup"><span data-stu-id="f0b60-166">Request</span></span>
<span data-ttu-id="f0b60-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0b60-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
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

### <a name="response"></a><span data-ttu-id="f0b60-168">响应</span><span class="sxs-lookup"><span data-stu-id="f0b60-168">Response</span></span>
<span data-ttu-id="f0b60-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0b60-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





