---
title: 更新 deviceHealthScript
description: 更新 deviceHealthScript 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a3eb34d13008c4dcf572f3418928215ea435761
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146277"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="761df-103">更新 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="761df-103">Update deviceHealthScript</span></span>

<span data-ttu-id="761df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="761df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="761df-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="761df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="761df-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="761df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="761df-107">更新 [deviceHealthScript 对象](../resources/intune-devices-devicehealthscript.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="761df-107">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="761df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="761df-108">Prerequisites</span></span>
<span data-ttu-id="761df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="761df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="761df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="761df-111">Permission type</span></span>|<span data-ttu-id="761df-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="761df-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="761df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="761df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="761df-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="761df-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="761df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="761df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="761df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="761df-116">Not supported.</span></span>|
|<span data-ttu-id="761df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="761df-117">Application</span></span>|<span data-ttu-id="761df-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="761df-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="761df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="761df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="761df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="761df-120">Request headers</span></span>
|<span data-ttu-id="761df-121">标头</span><span class="sxs-lookup"><span data-stu-id="761df-121">Header</span></span>|<span data-ttu-id="761df-122">值</span><span class="sxs-lookup"><span data-stu-id="761df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="761df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="761df-123">Authorization</span></span>|<span data-ttu-id="761df-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="761df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="761df-125">接受</span><span class="sxs-lookup"><span data-stu-id="761df-125">Accept</span></span>|<span data-ttu-id="761df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="761df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="761df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="761df-127">Request body</span></span>
<span data-ttu-id="761df-128">在请求正文中，提供 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="761df-128">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="761df-129">下表显示创建 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="761df-129">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="761df-130">属性</span><span class="sxs-lookup"><span data-stu-id="761df-130">Property</span></span>|<span data-ttu-id="761df-131">类型</span><span class="sxs-lookup"><span data-stu-id="761df-131">Type</span></span>|<span data-ttu-id="761df-132">说明</span><span class="sxs-lookup"><span data-stu-id="761df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="761df-133">id</span><span class="sxs-lookup"><span data-stu-id="761df-133">id</span></span>|<span data-ttu-id="761df-134">String</span><span class="sxs-lookup"><span data-stu-id="761df-134">String</span></span>|<span data-ttu-id="761df-135">设备运行状况脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="761df-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="761df-136">发布者</span><span class="sxs-lookup"><span data-stu-id="761df-136">publisher</span></span>|<span data-ttu-id="761df-137">String</span><span class="sxs-lookup"><span data-stu-id="761df-137">String</span></span>|<span data-ttu-id="761df-138">设备运行状况脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="761df-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="761df-139">version</span><span class="sxs-lookup"><span data-stu-id="761df-139">version</span></span>|<span data-ttu-id="761df-140">String</span><span class="sxs-lookup"><span data-stu-id="761df-140">String</span></span>|<span data-ttu-id="761df-141">设备运行状况脚本的版本</span><span class="sxs-lookup"><span data-stu-id="761df-141">Version of the device health script</span></span>|
|<span data-ttu-id="761df-142">displayName</span><span class="sxs-lookup"><span data-stu-id="761df-142">displayName</span></span>|<span data-ttu-id="761df-143">String</span><span class="sxs-lookup"><span data-stu-id="761df-143">String</span></span>|<span data-ttu-id="761df-144">设备运行状况脚本的名称</span><span class="sxs-lookup"><span data-stu-id="761df-144">Name of the device health script</span></span>|
|<span data-ttu-id="761df-145">说明</span><span class="sxs-lookup"><span data-stu-id="761df-145">description</span></span>|<span data-ttu-id="761df-146">String</span><span class="sxs-lookup"><span data-stu-id="761df-146">String</span></span>|<span data-ttu-id="761df-147">设备运行状况脚本的说明</span><span class="sxs-lookup"><span data-stu-id="761df-147">Description of the device health script</span></span>|
|<span data-ttu-id="761df-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="761df-148">detectionScriptContent</span></span>|<span data-ttu-id="761df-149">Binary</span><span class="sxs-lookup"><span data-stu-id="761df-149">Binary</span></span>|<span data-ttu-id="761df-150">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="761df-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="761df-151">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="761df-151">remediationScriptContent</span></span>|<span data-ttu-id="761df-152">Binary</span><span class="sxs-lookup"><span data-stu-id="761df-152">Binary</span></span>|<span data-ttu-id="761df-153">修正 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="761df-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="761df-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="761df-154">createdDateTime</span></span>|<span data-ttu-id="761df-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="761df-155">DateTimeOffset</span></span>|<span data-ttu-id="761df-156">创建设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="761df-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="761df-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="761df-157">This property is read-only.</span></span>|
|<span data-ttu-id="761df-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="761df-158">lastModifiedDateTime</span></span>|<span data-ttu-id="761df-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="761df-159">DateTimeOffset</span></span>|<span data-ttu-id="761df-160">修改设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="761df-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="761df-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="761df-161">This property is read-only.</span></span>|
|<span data-ttu-id="761df-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="761df-162">runAsAccount</span></span>|[<span data-ttu-id="761df-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="761df-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="761df-164">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="761df-164">Indicates the type of execution context.</span></span> <span data-ttu-id="761df-165">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="761df-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="761df-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="761df-166">enforceSignatureCheck</span></span>|<span data-ttu-id="761df-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="761df-167">Boolean</span></span>|<span data-ttu-id="761df-168">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="761df-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="761df-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="761df-169">runAs32Bit</span></span>|<span data-ttu-id="761df-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="761df-170">Boolean</span></span>|<span data-ttu-id="761df-171">指示 PowerShell 脚本 () 32 位运行</span><span class="sxs-lookup"><span data-stu-id="761df-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="761df-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="761df-172">roleScopeTagIds</span></span>|<span data-ttu-id="761df-173">String collection</span><span class="sxs-lookup"><span data-stu-id="761df-173">String collection</span></span>|<span data-ttu-id="761df-174">设备运行状况脚本的范围标记标识列表</span><span class="sxs-lookup"><span data-stu-id="761df-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="761df-175">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="761df-175">isGlobalScript</span></span>|<span data-ttu-id="761df-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="761df-176">Boolean</span></span>|<span data-ttu-id="761df-177">确定这是否为 Microsoft 专有脚本。</span><span class="sxs-lookup"><span data-stu-id="761df-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="761df-178">专有脚本是只读的</span><span class="sxs-lookup"><span data-stu-id="761df-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="761df-179">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="761df-179">highestAvailableVersion</span></span>|<span data-ttu-id="761df-180">String</span><span class="sxs-lookup"><span data-stu-id="761df-180">String</span></span>|<span data-ttu-id="761df-181">Microsoft 专有脚本的最高可用版本</span><span class="sxs-lookup"><span data-stu-id="761df-181">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="761df-182">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="761df-182">detectionScriptParameters</span></span>|<span data-ttu-id="761df-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) 集合</span><span class="sxs-lookup"><span data-stu-id="761df-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="761df-184">ComplexType DetectionScriptParameters 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="761df-184">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="761df-185">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="761df-185">remediationScriptParameters</span></span>|<span data-ttu-id="761df-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) 集合</span><span class="sxs-lookup"><span data-stu-id="761df-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="761df-187">ComplexType RemediationScriptParameters 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="761df-187">List of ComplexType RemediationScriptParameters objects.</span></span>|



## <a name="response"></a><span data-ttu-id="761df-188">响应</span><span class="sxs-lookup"><span data-stu-id="761df-188">Response</span></span>
<span data-ttu-id="761df-189">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="761df-189">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="761df-190">示例</span><span class="sxs-lookup"><span data-stu-id="761df-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="761df-191">请求</span><span class="sxs-lookup"><span data-stu-id="761df-191">Request</span></span>
<span data-ttu-id="761df-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="761df-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-type: application/json
Content-length: 1221

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
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="761df-193">响应</span><span class="sxs-lookup"><span data-stu-id="761df-193">Response</span></span>
<span data-ttu-id="761df-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="761df-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1393

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
  "highestAvailableVersion": "Highest Available Version value",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ]
}
```




