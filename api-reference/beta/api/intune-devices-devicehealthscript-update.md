---
title: 更新 deviceHealthScript
description: 更新 deviceHealthScript 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ec2609c17259dcfb04e06aa115be0fe99e33c20
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062061"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="35747-103">更新 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="35747-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="35747-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35747-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35747-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35747-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35747-106">更新[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35747-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35747-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="35747-107">Prerequisites</span></span>
<span data-ttu-id="35747-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35747-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="35747-110">Permission type</span></span>|<span data-ttu-id="35747-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35747-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35747-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35747-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35747-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35747-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="35747-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35747-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35747-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="35747-115">Not supported.</span></span>|
|<span data-ttu-id="35747-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="35747-116">Application</span></span>|<span data-ttu-id="35747-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35747-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35747-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35747-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="35747-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="35747-119">Request headers</span></span>
|<span data-ttu-id="35747-120">标头</span><span class="sxs-lookup"><span data-stu-id="35747-120">Header</span></span>|<span data-ttu-id="35747-121">值</span><span class="sxs-lookup"><span data-stu-id="35747-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35747-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35747-122">Authorization</span></span>|<span data-ttu-id="35747-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35747-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35747-124">接受</span><span class="sxs-lookup"><span data-stu-id="35747-124">Accept</span></span>|<span data-ttu-id="35747-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35747-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35747-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="35747-126">Request body</span></span>
<span data-ttu-id="35747-127">在请求正文中，提供[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35747-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="35747-128">下表显示创建[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35747-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="35747-129">属性</span><span class="sxs-lookup"><span data-stu-id="35747-129">Property</span></span>|<span data-ttu-id="35747-130">类型</span><span class="sxs-lookup"><span data-stu-id="35747-130">Type</span></span>|<span data-ttu-id="35747-131">说明</span><span class="sxs-lookup"><span data-stu-id="35747-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35747-132">id</span><span class="sxs-lookup"><span data-stu-id="35747-132">id</span></span>|<span data-ttu-id="35747-133">字符串</span><span class="sxs-lookup"><span data-stu-id="35747-133">String</span></span>|<span data-ttu-id="35747-134">设备运行状况脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="35747-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="35747-135">发布者</span><span class="sxs-lookup"><span data-stu-id="35747-135">publisher</span></span>|<span data-ttu-id="35747-136">String</span><span class="sxs-lookup"><span data-stu-id="35747-136">String</span></span>|<span data-ttu-id="35747-137">设备运行状况脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="35747-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="35747-138">displayName</span><span class="sxs-lookup"><span data-stu-id="35747-138">displayName</span></span>|<span data-ttu-id="35747-139">字符串</span><span class="sxs-lookup"><span data-stu-id="35747-139">String</span></span>|<span data-ttu-id="35747-140">设备运行状况脚本的名称</span><span class="sxs-lookup"><span data-stu-id="35747-140">Name of the device health script</span></span>|
|<span data-ttu-id="35747-141">description</span><span class="sxs-lookup"><span data-stu-id="35747-141">description</span></span>|<span data-ttu-id="35747-142">String</span><span class="sxs-lookup"><span data-stu-id="35747-142">String</span></span>|<span data-ttu-id="35747-143">设备运行状况脚本的说明</span><span class="sxs-lookup"><span data-stu-id="35747-143">Description of the device health script</span></span>|
|<span data-ttu-id="35747-144">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="35747-144">detectionScriptContent</span></span>|<span data-ttu-id="35747-145">Binary</span><span class="sxs-lookup"><span data-stu-id="35747-145">Binary</span></span>|<span data-ttu-id="35747-146">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="35747-146">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="35747-147">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="35747-147">remediationScriptContent</span></span>|<span data-ttu-id="35747-148">Binary</span><span class="sxs-lookup"><span data-stu-id="35747-148">Binary</span></span>|<span data-ttu-id="35747-149">修正 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="35747-149">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="35747-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35747-150">createdDateTime</span></span>|<span data-ttu-id="35747-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35747-151">DateTimeOffset</span></span>|<span data-ttu-id="35747-152">设备运行状况脚本的创建时间的时间戳。</span><span class="sxs-lookup"><span data-stu-id="35747-152">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="35747-153">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="35747-153">This property is read-only.</span></span>|
|<span data-ttu-id="35747-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35747-154">lastModifiedDateTime</span></span>|<span data-ttu-id="35747-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35747-155">DateTimeOffset</span></span>|<span data-ttu-id="35747-156">修改设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="35747-156">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="35747-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="35747-157">This property is read-only.</span></span>|
|<span data-ttu-id="35747-158">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="35747-158">runAsAccount</span></span>|[<span data-ttu-id="35747-159">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="35747-159">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="35747-160">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="35747-160">Indicates the type of execution context.</span></span> <span data-ttu-id="35747-161">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="35747-161">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="35747-162">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="35747-162">enforceSignatureCheck</span></span>|<span data-ttu-id="35747-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="35747-163">Boolean</span></span>|<span data-ttu-id="35747-164">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="35747-164">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="35747-165">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="35747-165">runAs32Bit</span></span>|<span data-ttu-id="35747-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="35747-166">Boolean</span></span>|<span data-ttu-id="35747-167">指示 PowerShell 脚本是否应作为32位运行</span><span class="sxs-lookup"><span data-stu-id="35747-167">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="35747-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35747-168">roleScopeTagIds</span></span>|<span data-ttu-id="35747-169">String 集合</span><span class="sxs-lookup"><span data-stu-id="35747-169">String collection</span></span>|<span data-ttu-id="35747-170">设备运行状况脚本的范围标记 Id 列表</span><span class="sxs-lookup"><span data-stu-id="35747-170">List of Scope Tag IDs for the device health script</span></span>|



## <a name="response"></a><span data-ttu-id="35747-171">响应</span><span class="sxs-lookup"><span data-stu-id="35747-171">Response</span></span>
<span data-ttu-id="35747-172">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35747-172">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35747-173">示例</span><span class="sxs-lookup"><span data-stu-id="35747-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="35747-174">请求</span><span class="sxs-lookup"><span data-stu-id="35747-174">Request</span></span>
<span data-ttu-id="35747-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35747-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-type: application/json
Content-length: 575

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
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

### <a name="response"></a><span data-ttu-id="35747-176">响应</span><span class="sxs-lookup"><span data-stu-id="35747-176">Response</span></span>
<span data-ttu-id="35747-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35747-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 747

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
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
}
```




