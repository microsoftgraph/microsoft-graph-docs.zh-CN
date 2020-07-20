---
title: 创建 deviceComplianceScript
description: 创建新的 deviceComplianceScript 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbd57133d102a6c0e8d7e28e275388cb13ecbee8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792504"
---
# <a name="create-devicecompliancescript"></a><span data-ttu-id="99f15-103">创建 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="99f15-103">Create deviceComplianceScript</span></span>

<span data-ttu-id="99f15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99f15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99f15-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99f15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99f15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99f15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99f15-107">创建新的[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="99f15-107">Create a new [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99f15-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="99f15-108">Prerequisites</span></span>
<span data-ttu-id="99f15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99f15-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99f15-111">Permission type</span></span>|<span data-ttu-id="99f15-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99f15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99f15-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99f15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99f15-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99f15-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99f15-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99f15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99f15-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99f15-116">Not supported.</span></span>|
|<span data-ttu-id="99f15-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="99f15-117">Application</span></span>|<span data-ttu-id="99f15-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99f15-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99f15-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99f15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="99f15-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99f15-120">Request headers</span></span>
|<span data-ttu-id="99f15-121">标头</span><span class="sxs-lookup"><span data-stu-id="99f15-121">Header</span></span>|<span data-ttu-id="99f15-122">值</span><span class="sxs-lookup"><span data-stu-id="99f15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99f15-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99f15-123">Authorization</span></span>|<span data-ttu-id="99f15-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99f15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99f15-125">接受</span><span class="sxs-lookup"><span data-stu-id="99f15-125">Accept</span></span>|<span data-ttu-id="99f15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99f15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99f15-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="99f15-127">Request body</span></span>
<span data-ttu-id="99f15-128">在请求正文中，提供 deviceComplianceScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99f15-128">In the request body, supply a JSON representation for the deviceComplianceScript object.</span></span>

<span data-ttu-id="99f15-129">下表显示创建 deviceComplianceScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="99f15-129">The following table shows the properties that are required when you create the deviceComplianceScript.</span></span>

|<span data-ttu-id="99f15-130">属性</span><span class="sxs-lookup"><span data-stu-id="99f15-130">Property</span></span>|<span data-ttu-id="99f15-131">类型</span><span class="sxs-lookup"><span data-stu-id="99f15-131">Type</span></span>|<span data-ttu-id="99f15-132">说明</span><span class="sxs-lookup"><span data-stu-id="99f15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99f15-133">id</span><span class="sxs-lookup"><span data-stu-id="99f15-133">id</span></span>|<span data-ttu-id="99f15-134">字符串</span><span class="sxs-lookup"><span data-stu-id="99f15-134">String</span></span>|<span data-ttu-id="99f15-135">设备符合性脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="99f15-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="99f15-136">发布者</span><span class="sxs-lookup"><span data-stu-id="99f15-136">publisher</span></span>|<span data-ttu-id="99f15-137">String</span><span class="sxs-lookup"><span data-stu-id="99f15-137">String</span></span>|<span data-ttu-id="99f15-138">设备合规性脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="99f15-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="99f15-139">version</span><span class="sxs-lookup"><span data-stu-id="99f15-139">version</span></span>|<span data-ttu-id="99f15-140">String</span><span class="sxs-lookup"><span data-stu-id="99f15-140">String</span></span>|<span data-ttu-id="99f15-141">设备合规性脚本的版本</span><span class="sxs-lookup"><span data-stu-id="99f15-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="99f15-142">displayName</span><span class="sxs-lookup"><span data-stu-id="99f15-142">displayName</span></span>|<span data-ttu-id="99f15-143">字符串</span><span class="sxs-lookup"><span data-stu-id="99f15-143">String</span></span>|<span data-ttu-id="99f15-144">设备合规性脚本的名称</span><span class="sxs-lookup"><span data-stu-id="99f15-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="99f15-145">说明</span><span class="sxs-lookup"><span data-stu-id="99f15-145">description</span></span>|<span data-ttu-id="99f15-146">String</span><span class="sxs-lookup"><span data-stu-id="99f15-146">String</span></span>|<span data-ttu-id="99f15-147">设备合规性脚本的说明</span><span class="sxs-lookup"><span data-stu-id="99f15-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="99f15-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="99f15-148">detectionScriptContent</span></span>|<span data-ttu-id="99f15-149">Binary</span><span class="sxs-lookup"><span data-stu-id="99f15-149">Binary</span></span>|<span data-ttu-id="99f15-150">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="99f15-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="99f15-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99f15-151">createdDateTime</span></span>|<span data-ttu-id="99f15-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99f15-152">DateTimeOffset</span></span>|<span data-ttu-id="99f15-153">创建设备符合性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="99f15-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="99f15-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="99f15-154">This property is read-only.</span></span>|
|<span data-ttu-id="99f15-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99f15-155">lastModifiedDateTime</span></span>|<span data-ttu-id="99f15-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99f15-156">DateTimeOffset</span></span>|<span data-ttu-id="99f15-157">修改设备符合性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="99f15-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="99f15-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="99f15-158">This property is read-only.</span></span>|
|<span data-ttu-id="99f15-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="99f15-159">runAsAccount</span></span>|[<span data-ttu-id="99f15-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="99f15-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="99f15-161">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="99f15-161">Indicates the type of execution context.</span></span> <span data-ttu-id="99f15-162">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="99f15-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="99f15-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="99f15-163">enforceSignatureCheck</span></span>|<span data-ttu-id="99f15-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="99f15-164">Boolean</span></span>|<span data-ttu-id="99f15-165">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="99f15-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="99f15-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="99f15-166">runAs32Bit</span></span>|<span data-ttu-id="99f15-167">布尔值</span><span class="sxs-lookup"><span data-stu-id="99f15-167">Boolean</span></span>|<span data-ttu-id="99f15-168">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="99f15-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="99f15-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99f15-169">roleScopeTagIds</span></span>|<span data-ttu-id="99f15-170">String collection</span><span class="sxs-lookup"><span data-stu-id="99f15-170">String collection</span></span>|<span data-ttu-id="99f15-171">设备符合性脚本的作用域标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="99f15-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="99f15-172">响应</span><span class="sxs-lookup"><span data-stu-id="99f15-172">Response</span></span>
<span data-ttu-id="99f15-173">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="99f15-173">If successful, this method returns a `201 Created` response code and a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99f15-174">示例</span><span class="sxs-lookup"><span data-stu-id="99f15-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="99f15-175">请求</span><span class="sxs-lookup"><span data-stu-id="99f15-175">Request</span></span>
<span data-ttu-id="99f15-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99f15-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
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

### <a name="response"></a><span data-ttu-id="99f15-177">响应</span><span class="sxs-lookup"><span data-stu-id="99f15-177">Response</span></span>
<span data-ttu-id="99f15-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99f15-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



