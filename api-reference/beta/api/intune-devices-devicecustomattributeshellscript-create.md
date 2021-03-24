---
title: 创建 deviceCustomAttributeShellScript
description: 创建新的 deviceCustomAttributeShellScript 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7db71c2c35aaf514a893749a0f6aaf1565c460b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146417"
---
# <a name="create-devicecustomattributeshellscript"></a><span data-ttu-id="db6c1-103">创建 deviceCustomAttributeShellScript</span><span class="sxs-lookup"><span data-stu-id="db6c1-103">Create deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="db6c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db6c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db6c1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db6c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db6c1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db6c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db6c1-107">创建新的 [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db6c1-107">Create a new [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db6c1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="db6c1-108">Prerequisites</span></span>
<span data-ttu-id="db6c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db6c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db6c1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="db6c1-111">Permission type</span></span>|<span data-ttu-id="db6c1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db6c1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db6c1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db6c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db6c1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db6c1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="db6c1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db6c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db6c1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db6c1-116">Not supported.</span></span>|
|<span data-ttu-id="db6c1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="db6c1-117">Application</span></span>|<span data-ttu-id="db6c1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db6c1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db6c1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db6c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCustomAttributeShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="db6c1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db6c1-120">Request headers</span></span>
|<span data-ttu-id="db6c1-121">标头</span><span class="sxs-lookup"><span data-stu-id="db6c1-121">Header</span></span>|<span data-ttu-id="db6c1-122">值</span><span class="sxs-lookup"><span data-stu-id="db6c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db6c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db6c1-123">Authorization</span></span>|<span data-ttu-id="db6c1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db6c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db6c1-125">接受</span><span class="sxs-lookup"><span data-stu-id="db6c1-125">Accept</span></span>|<span data-ttu-id="db6c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db6c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db6c1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="db6c1-127">Request body</span></span>
<span data-ttu-id="db6c1-128">在请求正文中，提供 deviceCustomAttributeShellScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db6c1-128">In the request body, supply a JSON representation for the deviceCustomAttributeShellScript object.</span></span>

<span data-ttu-id="db6c1-129">下表显示创建 deviceCustomAttributeShellScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db6c1-129">The following table shows the properties that are required when you create the deviceCustomAttributeShellScript.</span></span>

|<span data-ttu-id="db6c1-130">属性</span><span class="sxs-lookup"><span data-stu-id="db6c1-130">Property</span></span>|<span data-ttu-id="db6c1-131">类型</span><span class="sxs-lookup"><span data-stu-id="db6c1-131">Type</span></span>|<span data-ttu-id="db6c1-132">说明</span><span class="sxs-lookup"><span data-stu-id="db6c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db6c1-133">id</span><span class="sxs-lookup"><span data-stu-id="db6c1-133">id</span></span>|<span data-ttu-id="db6c1-134">String</span><span class="sxs-lookup"><span data-stu-id="db6c1-134">String</span></span>|<span data-ttu-id="db6c1-135">自定义属性实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="db6c1-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="db6c1-136">customAttributeName</span><span class="sxs-lookup"><span data-stu-id="db6c1-136">customAttributeName</span></span>|<span data-ttu-id="db6c1-137">String</span><span class="sxs-lookup"><span data-stu-id="db6c1-137">String</span></span>|<span data-ttu-id="db6c1-138">自定义属性的名称。</span><span class="sxs-lookup"><span data-stu-id="db6c1-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="db6c1-139">customAttributeType</span><span class="sxs-lookup"><span data-stu-id="db6c1-139">customAttributeType</span></span>|[<span data-ttu-id="db6c1-140">deviceCustomAttributeValueType</span><span class="sxs-lookup"><span data-stu-id="db6c1-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="db6c1-141">自定义属性的值的预期类型。</span><span class="sxs-lookup"><span data-stu-id="db6c1-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="db6c1-142">可取值为：`integer`、`string`、`dateTime`。</span><span class="sxs-lookup"><span data-stu-id="db6c1-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="db6c1-143">displayName</span><span class="sxs-lookup"><span data-stu-id="db6c1-143">displayName</span></span>|<span data-ttu-id="db6c1-144">String</span><span class="sxs-lookup"><span data-stu-id="db6c1-144">String</span></span>|<span data-ttu-id="db6c1-145">设备管理脚本的名称。</span><span class="sxs-lookup"><span data-stu-id="db6c1-145">Name of the device management script.</span></span>|
|<span data-ttu-id="db6c1-146">说明</span><span class="sxs-lookup"><span data-stu-id="db6c1-146">description</span></span>|<span data-ttu-id="db6c1-147">String</span><span class="sxs-lookup"><span data-stu-id="db6c1-147">String</span></span>|<span data-ttu-id="db6c1-148">设备管理脚本的可选说明。</span><span class="sxs-lookup"><span data-stu-id="db6c1-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="db6c1-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="db6c1-149">scriptContent</span></span>|<span data-ttu-id="db6c1-150">Binary</span><span class="sxs-lookup"><span data-stu-id="db6c1-150">Binary</span></span>|<span data-ttu-id="db6c1-151">脚本内容。</span><span class="sxs-lookup"><span data-stu-id="db6c1-151">The script content.</span></span>|
|<span data-ttu-id="db6c1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db6c1-152">createdDateTime</span></span>|<span data-ttu-id="db6c1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db6c1-153">DateTimeOffset</span></span>|<span data-ttu-id="db6c1-154">创建设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="db6c1-154">The date and time the device management script was created.</span></span> <span data-ttu-id="db6c1-155">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="db6c1-155">This property is read-only.</span></span>|
|<span data-ttu-id="db6c1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db6c1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="db6c1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db6c1-157">DateTimeOffset</span></span>|<span data-ttu-id="db6c1-158">上次修改设备管理脚本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="db6c1-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="db6c1-159">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="db6c1-159">This property is read-only.</span></span>|
|<span data-ttu-id="db6c1-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="db6c1-160">runAsAccount</span></span>|[<span data-ttu-id="db6c1-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="db6c1-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="db6c1-162">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="db6c1-162">Indicates the type of execution context.</span></span> <span data-ttu-id="db6c1-163">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="db6c1-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="db6c1-164">fileName</span><span class="sxs-lookup"><span data-stu-id="db6c1-164">fileName</span></span>|<span data-ttu-id="db6c1-165">String</span><span class="sxs-lookup"><span data-stu-id="db6c1-165">String</span></span>|<span data-ttu-id="db6c1-166">脚本文件名。</span><span class="sxs-lookup"><span data-stu-id="db6c1-166">Script file name.</span></span>|
|<span data-ttu-id="db6c1-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db6c1-167">roleScopeTagIds</span></span>|<span data-ttu-id="db6c1-168">String collection</span><span class="sxs-lookup"><span data-stu-id="db6c1-168">String collection</span></span>|<span data-ttu-id="db6c1-169">此 PowerShellScript 实例的范围标记标识列表。</span><span class="sxs-lookup"><span data-stu-id="db6c1-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="db6c1-170">响应</span><span class="sxs-lookup"><span data-stu-id="db6c1-170">Response</span></span>
<span data-ttu-id="db6c1-171">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db6c1-171">If successful, this method returns a `201 Created` response code and a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db6c1-172">示例</span><span class="sxs-lookup"><span data-stu-id="db6c1-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="db6c1-173">请求</span><span class="sxs-lookup"><span data-stu-id="db6c1-173">Request</span></span>
<span data-ttu-id="db6c1-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db6c1-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "customAttributeName": "Custom Attribute Name value",
  "customAttributeType": "string",
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

### <a name="response"></a><span data-ttu-id="db6c1-175">响应</span><span class="sxs-lookup"><span data-stu-id="db6c1-175">Response</span></span>
<span data-ttu-id="db6c1-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db6c1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "id": "929d921b-921b-929d-1b92-9d921b929d92",
  "customAttributeName": "Custom Attribute Name value",
  "customAttributeType": "string",
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




