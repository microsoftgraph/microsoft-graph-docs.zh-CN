---
title: 更新 deviceComplianceScript
description: 更新 deviceComplianceScript 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88187ad5f3ea66202823c074b85a5336078246df
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792476"
---
# <a name="update-devicecompliancescript"></a><span data-ttu-id="daf31-103">更新 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="daf31-103">Update deviceComplianceScript</span></span>

<span data-ttu-id="daf31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daf31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daf31-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="daf31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daf31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="daf31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf31-107">更新[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="daf31-107">Update the properties of a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daf31-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="daf31-108">Prerequisites</span></span>
<span data-ttu-id="daf31-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="daf31-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="daf31-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daf31-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daf31-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="daf31-111">Permission type</span></span>|<span data-ttu-id="daf31-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="daf31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daf31-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="daf31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="daf31-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf31-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="daf31-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="daf31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daf31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="daf31-116">Not supported.</span></span>|
|<span data-ttu-id="daf31-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="daf31-117">Application</span></span>|<span data-ttu-id="daf31-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf31-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="daf31-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="daf31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="daf31-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="daf31-120">Request headers</span></span>
|<span data-ttu-id="daf31-121">标头</span><span class="sxs-lookup"><span data-stu-id="daf31-121">Header</span></span>|<span data-ttu-id="daf31-122">值</span><span class="sxs-lookup"><span data-stu-id="daf31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daf31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="daf31-123">Authorization</span></span>|<span data-ttu-id="daf31-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="daf31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daf31-125">接受</span><span class="sxs-lookup"><span data-stu-id="daf31-125">Accept</span></span>|<span data-ttu-id="daf31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="daf31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daf31-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="daf31-127">Request body</span></span>
<span data-ttu-id="daf31-128">在请求正文中，提供[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="daf31-128">In the request body, supply a JSON representation for the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

<span data-ttu-id="daf31-129">下表显示创建[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="daf31-129">The following table shows the properties that are required when you create the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).</span></span>

|<span data-ttu-id="daf31-130">属性</span><span class="sxs-lookup"><span data-stu-id="daf31-130">Property</span></span>|<span data-ttu-id="daf31-131">类型</span><span class="sxs-lookup"><span data-stu-id="daf31-131">Type</span></span>|<span data-ttu-id="daf31-132">说明</span><span class="sxs-lookup"><span data-stu-id="daf31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf31-133">id</span><span class="sxs-lookup"><span data-stu-id="daf31-133">id</span></span>|<span data-ttu-id="daf31-134">字符串</span><span class="sxs-lookup"><span data-stu-id="daf31-134">String</span></span>|<span data-ttu-id="daf31-135">设备符合性脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="daf31-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="daf31-136">发布者</span><span class="sxs-lookup"><span data-stu-id="daf31-136">publisher</span></span>|<span data-ttu-id="daf31-137">String</span><span class="sxs-lookup"><span data-stu-id="daf31-137">String</span></span>|<span data-ttu-id="daf31-138">设备合规性脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="daf31-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="daf31-139">version</span><span class="sxs-lookup"><span data-stu-id="daf31-139">version</span></span>|<span data-ttu-id="daf31-140">String</span><span class="sxs-lookup"><span data-stu-id="daf31-140">String</span></span>|<span data-ttu-id="daf31-141">设备合规性脚本的版本</span><span class="sxs-lookup"><span data-stu-id="daf31-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="daf31-142">displayName</span><span class="sxs-lookup"><span data-stu-id="daf31-142">displayName</span></span>|<span data-ttu-id="daf31-143">字符串</span><span class="sxs-lookup"><span data-stu-id="daf31-143">String</span></span>|<span data-ttu-id="daf31-144">设备合规性脚本的名称</span><span class="sxs-lookup"><span data-stu-id="daf31-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="daf31-145">说明</span><span class="sxs-lookup"><span data-stu-id="daf31-145">description</span></span>|<span data-ttu-id="daf31-146">String</span><span class="sxs-lookup"><span data-stu-id="daf31-146">String</span></span>|<span data-ttu-id="daf31-147">设备合规性脚本的说明</span><span class="sxs-lookup"><span data-stu-id="daf31-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="daf31-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="daf31-148">detectionScriptContent</span></span>|<span data-ttu-id="daf31-149">Binary</span><span class="sxs-lookup"><span data-stu-id="daf31-149">Binary</span></span>|<span data-ttu-id="daf31-150">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="daf31-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="daf31-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="daf31-151">createdDateTime</span></span>|<span data-ttu-id="daf31-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daf31-152">DateTimeOffset</span></span>|<span data-ttu-id="daf31-153">创建设备符合性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="daf31-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="daf31-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="daf31-154">This property is read-only.</span></span>|
|<span data-ttu-id="daf31-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="daf31-155">lastModifiedDateTime</span></span>|<span data-ttu-id="daf31-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="daf31-156">DateTimeOffset</span></span>|<span data-ttu-id="daf31-157">修改设备符合性脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="daf31-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="daf31-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="daf31-158">This property is read-only.</span></span>|
|<span data-ttu-id="daf31-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="daf31-159">runAsAccount</span></span>|[<span data-ttu-id="daf31-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="daf31-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="daf31-161">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="daf31-161">Indicates the type of execution context.</span></span> <span data-ttu-id="daf31-162">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="daf31-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="daf31-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="daf31-163">enforceSignatureCheck</span></span>|<span data-ttu-id="daf31-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="daf31-164">Boolean</span></span>|<span data-ttu-id="daf31-165">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="daf31-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="daf31-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="daf31-166">runAs32Bit</span></span>|<span data-ttu-id="daf31-167">布尔值</span><span class="sxs-lookup"><span data-stu-id="daf31-167">Boolean</span></span>|<span data-ttu-id="daf31-168">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="daf31-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="daf31-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="daf31-169">roleScopeTagIds</span></span>|<span data-ttu-id="daf31-170">String collection</span><span class="sxs-lookup"><span data-stu-id="daf31-170">String collection</span></span>|<span data-ttu-id="daf31-171">设备符合性脚本的作用域标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="daf31-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="daf31-172">响应</span><span class="sxs-lookup"><span data-stu-id="daf31-172">Response</span></span>
<span data-ttu-id="daf31-173">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="daf31-173">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daf31-174">示例</span><span class="sxs-lookup"><span data-stu-id="daf31-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="daf31-175">请求</span><span class="sxs-lookup"><span data-stu-id="daf31-175">Request</span></span>
<span data-ttu-id="daf31-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="daf31-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="daf31-177">响应</span><span class="sxs-lookup"><span data-stu-id="daf31-177">Response</span></span>
<span data-ttu-id="daf31-178">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="daf31-178">Here is an example of the response.</span></span> <span data-ttu-id="daf31-179">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="daf31-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="daf31-180">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="daf31-180">All of the properties will be returned from an actual call.</span></span>
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



