---
title: 更新 deviceComplianceScript
description: 更新 deviceComplianceScript 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 116dc79a5c7c7f34d6cf2b168d9012c0dbf488b8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150596"
---
# <a name="update-devicecompliancescript"></a><span data-ttu-id="74f6b-103">更新 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="74f6b-103">Update deviceComplianceScript</span></span>

<span data-ttu-id="74f6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74f6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74f6b-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74f6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74f6b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74f6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74f6b-107">更新 [deviceComplianceScript 对象](../resources/intune-devices-devicecompliancescript.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="74f6b-107">Update the properties of a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74f6b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="74f6b-108">Prerequisites</span></span>
<span data-ttu-id="74f6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74f6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74f6b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74f6b-111">Permission type</span></span>|<span data-ttu-id="74f6b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74f6b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74f6b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74f6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74f6b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f6b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="74f6b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74f6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74f6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74f6b-116">Not supported.</span></span>|
|<span data-ttu-id="74f6b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="74f6b-117">Application</span></span>|<span data-ttu-id="74f6b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f6b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74f6b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74f6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="74f6b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74f6b-120">Request headers</span></span>
|<span data-ttu-id="74f6b-121">标头</span><span class="sxs-lookup"><span data-stu-id="74f6b-121">Header</span></span>|<span data-ttu-id="74f6b-122">值</span><span class="sxs-lookup"><span data-stu-id="74f6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74f6b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74f6b-123">Authorization</span></span>|<span data-ttu-id="74f6b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74f6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74f6b-125">接受</span><span class="sxs-lookup"><span data-stu-id="74f6b-125">Accept</span></span>|<span data-ttu-id="74f6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74f6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74f6b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="74f6b-127">Request body</span></span>
<span data-ttu-id="74f6b-128">在请求正文中，提供 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74f6b-128">In the request body, supply a JSON representation for the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

<span data-ttu-id="74f6b-129">下表显示创建 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74f6b-129">The following table shows the properties that are required when you create the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).</span></span>

|<span data-ttu-id="74f6b-130">属性</span><span class="sxs-lookup"><span data-stu-id="74f6b-130">Property</span></span>|<span data-ttu-id="74f6b-131">类型</span><span class="sxs-lookup"><span data-stu-id="74f6b-131">Type</span></span>|<span data-ttu-id="74f6b-132">说明</span><span class="sxs-lookup"><span data-stu-id="74f6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f6b-133">id</span><span class="sxs-lookup"><span data-stu-id="74f6b-133">id</span></span>|<span data-ttu-id="74f6b-134">String</span><span class="sxs-lookup"><span data-stu-id="74f6b-134">String</span></span>|<span data-ttu-id="74f6b-135">设备合规性脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="74f6b-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="74f6b-136">发布者</span><span class="sxs-lookup"><span data-stu-id="74f6b-136">publisher</span></span>|<span data-ttu-id="74f6b-137">String</span><span class="sxs-lookup"><span data-stu-id="74f6b-137">String</span></span>|<span data-ttu-id="74f6b-138">设备合规性脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="74f6b-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="74f6b-139">version</span><span class="sxs-lookup"><span data-stu-id="74f6b-139">version</span></span>|<span data-ttu-id="74f6b-140">String</span><span class="sxs-lookup"><span data-stu-id="74f6b-140">String</span></span>|<span data-ttu-id="74f6b-141">设备合规性脚本的版本</span><span class="sxs-lookup"><span data-stu-id="74f6b-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="74f6b-142">displayName</span><span class="sxs-lookup"><span data-stu-id="74f6b-142">displayName</span></span>|<span data-ttu-id="74f6b-143">String</span><span class="sxs-lookup"><span data-stu-id="74f6b-143">String</span></span>|<span data-ttu-id="74f6b-144">设备合规性脚本的名称</span><span class="sxs-lookup"><span data-stu-id="74f6b-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="74f6b-145">说明</span><span class="sxs-lookup"><span data-stu-id="74f6b-145">description</span></span>|<span data-ttu-id="74f6b-146">String</span><span class="sxs-lookup"><span data-stu-id="74f6b-146">String</span></span>|<span data-ttu-id="74f6b-147">设备合规性脚本的说明</span><span class="sxs-lookup"><span data-stu-id="74f6b-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="74f6b-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="74f6b-148">detectionScriptContent</span></span>|<span data-ttu-id="74f6b-149">Binary</span><span class="sxs-lookup"><span data-stu-id="74f6b-149">Binary</span></span>|<span data-ttu-id="74f6b-150">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="74f6b-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="74f6b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74f6b-151">createdDateTime</span></span>|<span data-ttu-id="74f6b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f6b-152">DateTimeOffset</span></span>|<span data-ttu-id="74f6b-153">创建设备合规性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="74f6b-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="74f6b-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="74f6b-154">This property is read-only.</span></span>|
|<span data-ttu-id="74f6b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74f6b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="74f6b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f6b-156">DateTimeOffset</span></span>|<span data-ttu-id="74f6b-157">修改设备合规性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="74f6b-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="74f6b-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="74f6b-158">This property is read-only.</span></span>|
|<span data-ttu-id="74f6b-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="74f6b-159">runAsAccount</span></span>|[<span data-ttu-id="74f6b-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="74f6b-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="74f6b-161">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="74f6b-161">Indicates the type of execution context.</span></span> <span data-ttu-id="74f6b-162">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="74f6b-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="74f6b-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="74f6b-163">enforceSignatureCheck</span></span>|<span data-ttu-id="74f6b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="74f6b-164">Boolean</span></span>|<span data-ttu-id="74f6b-165">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="74f6b-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="74f6b-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="74f6b-166">runAs32Bit</span></span>|<span data-ttu-id="74f6b-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="74f6b-167">Boolean</span></span>|<span data-ttu-id="74f6b-168">指示 PowerShell 脚本 () 32 位运行</span><span class="sxs-lookup"><span data-stu-id="74f6b-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="74f6b-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="74f6b-169">roleScopeTagIds</span></span>|<span data-ttu-id="74f6b-170">String collection</span><span class="sxs-lookup"><span data-stu-id="74f6b-170">String collection</span></span>|<span data-ttu-id="74f6b-171">设备合规性脚本的范围标记标识列表</span><span class="sxs-lookup"><span data-stu-id="74f6b-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="74f6b-172">响应</span><span class="sxs-lookup"><span data-stu-id="74f6b-172">Response</span></span>
<span data-ttu-id="74f6b-173">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74f6b-173">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74f6b-174">示例</span><span class="sxs-lookup"><span data-stu-id="74f6b-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="74f6b-175">请求</span><span class="sxs-lookup"><span data-stu-id="74f6b-175">Request</span></span>
<span data-ttu-id="74f6b-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74f6b-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
Content-type: application/json
Content-length: 420

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="74f6b-177">响应</span><span class="sxs-lookup"><span data-stu-id="74f6b-177">Response</span></span>
<span data-ttu-id="74f6b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74f6b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "14e72a7b-2a7b-14e7-7b2a-e7147b2ae714",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




