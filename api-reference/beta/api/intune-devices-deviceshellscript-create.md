---
title: 创建 deviceShellScript
description: 创建新的 deviceShellScript 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e2777d766335d0d8ddade5eba1ea889b535113
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944860"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="6186e-103">创建 deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="6186e-103">Create deviceShellScript</span></span>

> <span data-ttu-id="6186e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6186e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6186e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6186e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6186e-106">创建新的[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6186e-106">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6186e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6186e-107">Prerequisites</span></span>
<span data-ttu-id="6186e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6186e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6186e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6186e-110">Permission type</span></span>|<span data-ttu-id="6186e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6186e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6186e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6186e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6186e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6186e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6186e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6186e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6186e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6186e-115">Not supported.</span></span>|
|<span data-ttu-id="6186e-116">Application</span><span class="sxs-lookup"><span data-stu-id="6186e-116">Application</span></span>|<span data-ttu-id="6186e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6186e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6186e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6186e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="6186e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6186e-119">Request headers</span></span>
|<span data-ttu-id="6186e-120">标头</span><span class="sxs-lookup"><span data-stu-id="6186e-120">Header</span></span>|<span data-ttu-id="6186e-121">值</span><span class="sxs-lookup"><span data-stu-id="6186e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6186e-122">授权</span><span class="sxs-lookup"><span data-stu-id="6186e-122">Authorization</span></span>|<span data-ttu-id="6186e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6186e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6186e-124">接受</span><span class="sxs-lookup"><span data-stu-id="6186e-124">Accept</span></span>|<span data-ttu-id="6186e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6186e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6186e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6186e-126">Request body</span></span>
<span data-ttu-id="6186e-127">在请求正文中，提供 deviceShellScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6186e-127">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="6186e-128">下表显示创建 deviceShellScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6186e-128">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="6186e-129">属性</span><span class="sxs-lookup"><span data-stu-id="6186e-129">Property</span></span>|<span data-ttu-id="6186e-130">类型</span><span class="sxs-lookup"><span data-stu-id="6186e-130">Type</span></span>|<span data-ttu-id="6186e-131">说明</span><span class="sxs-lookup"><span data-stu-id="6186e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6186e-132">id</span><span class="sxs-lookup"><span data-stu-id="6186e-132">id</span></span>|<span data-ttu-id="6186e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6186e-133">String</span></span>|<span data-ttu-id="6186e-134">设备管理脚本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6186e-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="6186e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6186e-135">displayName</span></span>|<span data-ttu-id="6186e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="6186e-136">String</span></span>|<span data-ttu-id="6186e-137">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="6186e-137">Name of the device management script.</span></span>|
|<span data-ttu-id="6186e-138">说明</span><span class="sxs-lookup"><span data-stu-id="6186e-138">description</span></span>|<span data-ttu-id="6186e-139">String</span><span class="sxs-lookup"><span data-stu-id="6186e-139">String</span></span>|<span data-ttu-id="6186e-140">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="6186e-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="6186e-141">scriptContent</span><span class="sxs-lookup"><span data-stu-id="6186e-141">scriptContent</span></span>|<span data-ttu-id="6186e-142">Binary</span><span class="sxs-lookup"><span data-stu-id="6186e-142">Binary</span></span>|<span data-ttu-id="6186e-143">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="6186e-143">The script content.</span></span>|
|<span data-ttu-id="6186e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6186e-144">createdDateTime</span></span>|<span data-ttu-id="6186e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6186e-145">DateTimeOffset</span></span>|<span data-ttu-id="6186e-146">设备管理脚本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6186e-146">The date and time the device management script was created.</span></span> <span data-ttu-id="6186e-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6186e-147">This property is read-only.</span></span>|
|<span data-ttu-id="6186e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6186e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6186e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6186e-149">DateTimeOffset</span></span>|<span data-ttu-id="6186e-150">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6186e-150">The date and time the device management script was last modified.</span></span> <span data-ttu-id="6186e-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6186e-151">This property is read-only.</span></span>|
|<span data-ttu-id="6186e-152">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6186e-152">runAsAccount</span></span>|[<span data-ttu-id="6186e-153">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="6186e-153">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6186e-154">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="6186e-154">Indicates the type of execution context.</span></span> <span data-ttu-id="6186e-155">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="6186e-155">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="6186e-156">fileName</span><span class="sxs-lookup"><span data-stu-id="6186e-156">fileName</span></span>|<span data-ttu-id="6186e-157">String</span><span class="sxs-lookup"><span data-stu-id="6186e-157">String</span></span>|<span data-ttu-id="6186e-158">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="6186e-158">Script file name.</span></span>|
|<span data-ttu-id="6186e-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6186e-159">roleScopeTagIds</span></span>|<span data-ttu-id="6186e-160">String collection</span><span class="sxs-lookup"><span data-stu-id="6186e-160">String collection</span></span>|<span data-ttu-id="6186e-161">此 PowerShellScript 实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="6186e-161">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="6186e-162">响应</span><span class="sxs-lookup"><span data-stu-id="6186e-162">Response</span></span>
<span data-ttu-id="6186e-163">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceShellScript](../resources/intune-devices-deviceshellscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6186e-163">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6186e-164">示例</span><span class="sxs-lookup"><span data-stu-id="6186e-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="6186e-165">请求</span><span class="sxs-lookup"><span data-stu-id="6186e-165">Request</span></span>
<span data-ttu-id="6186e-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6186e-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6186e-167">响应</span><span class="sxs-lookup"><span data-stu-id="6186e-167">Response</span></span>
<span data-ttu-id="6186e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6186e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





