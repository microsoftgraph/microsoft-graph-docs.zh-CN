---
title: 更新 deviceHealthScript
description: 更新 deviceHealthScript 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ae6e8b7c7fe90656d69e66e62d6fe09e366b5f7a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945121"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="38a57-103">更新 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="38a57-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="38a57-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38a57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38a57-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38a57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a57-106">更新[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38a57-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38a57-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="38a57-107">Prerequisites</span></span>
<span data-ttu-id="38a57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38a57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38a57-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38a57-110">Permission type</span></span>|<span data-ttu-id="38a57-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38a57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38a57-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38a57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38a57-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a57-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="38a57-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38a57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38a57-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38a57-115">Not supported.</span></span>|
|<span data-ttu-id="38a57-116">Application</span><span class="sxs-lookup"><span data-stu-id="38a57-116">Application</span></span>|<span data-ttu-id="38a57-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a57-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38a57-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38a57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="38a57-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38a57-119">Request headers</span></span>
|<span data-ttu-id="38a57-120">标头</span><span class="sxs-lookup"><span data-stu-id="38a57-120">Header</span></span>|<span data-ttu-id="38a57-121">值</span><span class="sxs-lookup"><span data-stu-id="38a57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38a57-122">授权</span><span class="sxs-lookup"><span data-stu-id="38a57-122">Authorization</span></span>|<span data-ttu-id="38a57-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38a57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38a57-124">接受</span><span class="sxs-lookup"><span data-stu-id="38a57-124">Accept</span></span>|<span data-ttu-id="38a57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38a57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38a57-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="38a57-126">Request body</span></span>
<span data-ttu-id="38a57-127">在请求正文中，提供[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38a57-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="38a57-128">下表显示创建[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38a57-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="38a57-129">属性</span><span class="sxs-lookup"><span data-stu-id="38a57-129">Property</span></span>|<span data-ttu-id="38a57-130">类型</span><span class="sxs-lookup"><span data-stu-id="38a57-130">Type</span></span>|<span data-ttu-id="38a57-131">说明</span><span class="sxs-lookup"><span data-stu-id="38a57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a57-132">id</span><span class="sxs-lookup"><span data-stu-id="38a57-132">id</span></span>|<span data-ttu-id="38a57-133">字符串</span><span class="sxs-lookup"><span data-stu-id="38a57-133">String</span></span>|<span data-ttu-id="38a57-134">设备运行状况脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="38a57-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="38a57-135">发布者</span><span class="sxs-lookup"><span data-stu-id="38a57-135">publisher</span></span>|<span data-ttu-id="38a57-136">字符串</span><span class="sxs-lookup"><span data-stu-id="38a57-136">String</span></span>|<span data-ttu-id="38a57-137">设备运行状况脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="38a57-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="38a57-138">version</span><span class="sxs-lookup"><span data-stu-id="38a57-138">version</span></span>|<span data-ttu-id="38a57-139">String</span><span class="sxs-lookup"><span data-stu-id="38a57-139">String</span></span>|<span data-ttu-id="38a57-140">设备运行状况脚本的版本</span><span class="sxs-lookup"><span data-stu-id="38a57-140">Version of the device health script</span></span>|
|<span data-ttu-id="38a57-141">displayName</span><span class="sxs-lookup"><span data-stu-id="38a57-141">displayName</span></span>|<span data-ttu-id="38a57-142">字符串</span><span class="sxs-lookup"><span data-stu-id="38a57-142">String</span></span>|<span data-ttu-id="38a57-143">设备运行状况脚本的名称</span><span class="sxs-lookup"><span data-stu-id="38a57-143">Name of the device health script</span></span>|
|<span data-ttu-id="38a57-144">说明</span><span class="sxs-lookup"><span data-stu-id="38a57-144">description</span></span>|<span data-ttu-id="38a57-145">String</span><span class="sxs-lookup"><span data-stu-id="38a57-145">String</span></span>|<span data-ttu-id="38a57-146">设备运行状况脚本的说明</span><span class="sxs-lookup"><span data-stu-id="38a57-146">Description of the device health script</span></span>|
|<span data-ttu-id="38a57-147">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="38a57-147">detectionScriptContent</span></span>|<span data-ttu-id="38a57-148">Binary</span><span class="sxs-lookup"><span data-stu-id="38a57-148">Binary</span></span>|<span data-ttu-id="38a57-149">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="38a57-149">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="38a57-150">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="38a57-150">remediationScriptContent</span></span>|<span data-ttu-id="38a57-151">Binary</span><span class="sxs-lookup"><span data-stu-id="38a57-151">Binary</span></span>|<span data-ttu-id="38a57-152">修正 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="38a57-152">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="38a57-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38a57-153">createdDateTime</span></span>|<span data-ttu-id="38a57-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38a57-154">DateTimeOffset</span></span>|<span data-ttu-id="38a57-155">设备运行状况脚本的创建时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="38a57-155">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="38a57-156">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="38a57-156">This property is read-only.</span></span>|
|<span data-ttu-id="38a57-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38a57-157">lastModifiedDateTime</span></span>|<span data-ttu-id="38a57-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38a57-158">DateTimeOffset</span></span>|<span data-ttu-id="38a57-159">修改设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="38a57-159">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="38a57-160">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="38a57-160">This property is read-only.</span></span>|
|<span data-ttu-id="38a57-161">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="38a57-161">runAsAccount</span></span>|[<span data-ttu-id="38a57-162">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="38a57-162">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="38a57-163">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="38a57-163">Indicates the type of execution context.</span></span> <span data-ttu-id="38a57-164">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="38a57-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="38a57-165">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="38a57-165">enforceSignatureCheck</span></span>|<span data-ttu-id="38a57-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a57-166">Boolean</span></span>|<span data-ttu-id="38a57-167">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="38a57-167">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="38a57-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="38a57-168">runAs32Bit</span></span>|<span data-ttu-id="38a57-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a57-169">Boolean</span></span>|<span data-ttu-id="38a57-170">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="38a57-170">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="38a57-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38a57-171">roleScopeTagIds</span></span>|<span data-ttu-id="38a57-172">String collection</span><span class="sxs-lookup"><span data-stu-id="38a57-172">String collection</span></span>|<span data-ttu-id="38a57-173">设备运行状况脚本的范围标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="38a57-173">List of Scope Tag IDs for the device health script</span></span>|



## <a name="response"></a><span data-ttu-id="38a57-174">响应</span><span class="sxs-lookup"><span data-stu-id="38a57-174">Response</span></span>
<span data-ttu-id="38a57-175">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38a57-175">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38a57-176">示例</span><span class="sxs-lookup"><span data-stu-id="38a57-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="38a57-177">请求</span><span class="sxs-lookup"><span data-stu-id="38a57-177">Request</span></span>
<span data-ttu-id="38a57-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38a57-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="38a57-179">响应</span><span class="sxs-lookup"><span data-stu-id="38a57-179">Response</span></span>
<span data-ttu-id="38a57-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38a57-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 655

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
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





