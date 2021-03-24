---
title: 创建 deviceHealthScript
description: 创建新的 deviceHealthScript 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb2fc4cde6aeffd30950e08c7a9183348388aa7b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146389"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="f097d-103">创建 deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="f097d-103">Create deviceHealthScript</span></span>

<span data-ttu-id="f097d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f097d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f097d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f097d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f097d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f097d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f097d-107">创建新的 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f097d-107">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f097d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f097d-108">Prerequisites</span></span>
<span data-ttu-id="f097d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f097d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f097d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f097d-111">Permission type</span></span>|<span data-ttu-id="f097d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f097d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f097d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f097d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f097d-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f097d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f097d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f097d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f097d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f097d-116">Not supported.</span></span>|
|<span data-ttu-id="f097d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f097d-117">Application</span></span>|<span data-ttu-id="f097d-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f097d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f097d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f097d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="f097d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f097d-120">Request headers</span></span>
|<span data-ttu-id="f097d-121">标头</span><span class="sxs-lookup"><span data-stu-id="f097d-121">Header</span></span>|<span data-ttu-id="f097d-122">值</span><span class="sxs-lookup"><span data-stu-id="f097d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f097d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f097d-123">Authorization</span></span>|<span data-ttu-id="f097d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f097d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f097d-125">接受</span><span class="sxs-lookup"><span data-stu-id="f097d-125">Accept</span></span>|<span data-ttu-id="f097d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f097d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f097d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f097d-127">Request body</span></span>
<span data-ttu-id="f097d-128">在请求正文中，提供 deviceHealthScript 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f097d-128">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="f097d-129">下表显示创建 deviceHealthScript 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f097d-129">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="f097d-130">属性</span><span class="sxs-lookup"><span data-stu-id="f097d-130">Property</span></span>|<span data-ttu-id="f097d-131">类型</span><span class="sxs-lookup"><span data-stu-id="f097d-131">Type</span></span>|<span data-ttu-id="f097d-132">说明</span><span class="sxs-lookup"><span data-stu-id="f097d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f097d-133">id</span><span class="sxs-lookup"><span data-stu-id="f097d-133">id</span></span>|<span data-ttu-id="f097d-134">String</span><span class="sxs-lookup"><span data-stu-id="f097d-134">String</span></span>|<span data-ttu-id="f097d-135">设备运行状况脚本的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f097d-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="f097d-136">发布者</span><span class="sxs-lookup"><span data-stu-id="f097d-136">publisher</span></span>|<span data-ttu-id="f097d-137">String</span><span class="sxs-lookup"><span data-stu-id="f097d-137">String</span></span>|<span data-ttu-id="f097d-138">设备运行状况脚本发布者的名称</span><span class="sxs-lookup"><span data-stu-id="f097d-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="f097d-139">version</span><span class="sxs-lookup"><span data-stu-id="f097d-139">version</span></span>|<span data-ttu-id="f097d-140">String</span><span class="sxs-lookup"><span data-stu-id="f097d-140">String</span></span>|<span data-ttu-id="f097d-141">设备运行状况脚本的版本</span><span class="sxs-lookup"><span data-stu-id="f097d-141">Version of the device health script</span></span>|
|<span data-ttu-id="f097d-142">displayName</span><span class="sxs-lookup"><span data-stu-id="f097d-142">displayName</span></span>|<span data-ttu-id="f097d-143">String</span><span class="sxs-lookup"><span data-stu-id="f097d-143">String</span></span>|<span data-ttu-id="f097d-144">设备运行状况脚本的名称</span><span class="sxs-lookup"><span data-stu-id="f097d-144">Name of the device health script</span></span>|
|<span data-ttu-id="f097d-145">说明</span><span class="sxs-lookup"><span data-stu-id="f097d-145">description</span></span>|<span data-ttu-id="f097d-146">String</span><span class="sxs-lookup"><span data-stu-id="f097d-146">String</span></span>|<span data-ttu-id="f097d-147">设备运行状况脚本的说明</span><span class="sxs-lookup"><span data-stu-id="f097d-147">Description of the device health script</span></span>|
|<span data-ttu-id="f097d-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="f097d-148">detectionScriptContent</span></span>|<span data-ttu-id="f097d-149">Binary</span><span class="sxs-lookup"><span data-stu-id="f097d-149">Binary</span></span>|<span data-ttu-id="f097d-150">检测 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="f097d-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="f097d-151">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="f097d-151">remediationScriptContent</span></span>|<span data-ttu-id="f097d-152">Binary</span><span class="sxs-lookup"><span data-stu-id="f097d-152">Binary</span></span>|<span data-ttu-id="f097d-153">修正 powershell 脚本的全部内容</span><span class="sxs-lookup"><span data-stu-id="f097d-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="f097d-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f097d-154">createdDateTime</span></span>|<span data-ttu-id="f097d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f097d-155">DateTimeOffset</span></span>|<span data-ttu-id="f097d-156">创建设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="f097d-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="f097d-157">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f097d-157">This property is read-only.</span></span>|
|<span data-ttu-id="f097d-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f097d-158">lastModifiedDateTime</span></span>|<span data-ttu-id="f097d-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f097d-159">DateTimeOffset</span></span>|<span data-ttu-id="f097d-160">修改设备运行状况脚本的时间戳。</span><span class="sxs-lookup"><span data-stu-id="f097d-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="f097d-161">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f097d-161">This property is read-only.</span></span>|
|<span data-ttu-id="f097d-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f097d-162">runAsAccount</span></span>|[<span data-ttu-id="f097d-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f097d-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f097d-164">指示执行上下文的类型。</span><span class="sxs-lookup"><span data-stu-id="f097d-164">Indicates the type of execution context.</span></span> <span data-ttu-id="f097d-165">可取值为：`system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f097d-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="f097d-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="f097d-166">enforceSignatureCheck</span></span>|<span data-ttu-id="f097d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f097d-167">Boolean</span></span>|<span data-ttu-id="f097d-168">指示是否需要检查脚本签名</span><span class="sxs-lookup"><span data-stu-id="f097d-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="f097d-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="f097d-169">runAs32Bit</span></span>|<span data-ttu-id="f097d-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f097d-170">Boolean</span></span>|<span data-ttu-id="f097d-171">指示 PowerShell 脚本 () 32 位运行</span><span class="sxs-lookup"><span data-stu-id="f097d-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="f097d-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f097d-172">roleScopeTagIds</span></span>|<span data-ttu-id="f097d-173">String collection</span><span class="sxs-lookup"><span data-stu-id="f097d-173">String collection</span></span>|<span data-ttu-id="f097d-174">设备运行状况脚本的范围标记标识列表</span><span class="sxs-lookup"><span data-stu-id="f097d-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="f097d-175">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="f097d-175">isGlobalScript</span></span>|<span data-ttu-id="f097d-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f097d-176">Boolean</span></span>|<span data-ttu-id="f097d-177">确定这是否为 Microsoft 专有脚本。</span><span class="sxs-lookup"><span data-stu-id="f097d-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="f097d-178">专有脚本是只读的</span><span class="sxs-lookup"><span data-stu-id="f097d-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="f097d-179">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="f097d-179">highestAvailableVersion</span></span>|<span data-ttu-id="f097d-180">String</span><span class="sxs-lookup"><span data-stu-id="f097d-180">String</span></span>|<span data-ttu-id="f097d-181">Microsoft 专有脚本的最高可用版本</span><span class="sxs-lookup"><span data-stu-id="f097d-181">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="f097d-182">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="f097d-182">detectionScriptParameters</span></span>|<span data-ttu-id="f097d-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f097d-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="f097d-184">ComplexType DetectionScriptParameters 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f097d-184">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="f097d-185">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="f097d-185">remediationScriptParameters</span></span>|<span data-ttu-id="f097d-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f097d-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="f097d-187">ComplexType RemediationScriptParameters 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f097d-187">List of ComplexType RemediationScriptParameters objects.</span></span>|



## <a name="response"></a><span data-ttu-id="f097d-188">响应</span><span class="sxs-lookup"><span data-stu-id="f097d-188">Response</span></span>
<span data-ttu-id="f097d-189">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f097d-189">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f097d-190">示例</span><span class="sxs-lookup"><span data-stu-id="f097d-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="f097d-191">请求</span><span class="sxs-lookup"><span data-stu-id="f097d-191">Request</span></span>
<span data-ttu-id="f097d-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f097d-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
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

### <a name="response"></a><span data-ttu-id="f097d-193">响应</span><span class="sxs-lookup"><span data-stu-id="f097d-193">Response</span></span>
<span data-ttu-id="f097d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f097d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




