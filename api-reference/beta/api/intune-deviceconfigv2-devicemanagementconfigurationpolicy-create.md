---
title: 创建 deviceManagementConfigurationPolicy
description: 创建新的 deviceManagementConfigurationPolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c6ead094999f2ff21d63fde2469a459072f6b83
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666125"
---
# <a name="create-devicemanagementconfigurationpolicy"></a><span data-ttu-id="78e5d-103">创建 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="78e5d-103">Create deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="78e5d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78e5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78e5d-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78e5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e5d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78e5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e5d-107">创建新的 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78e5d-107">Create a new [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78e5d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="78e5d-108">Prerequisites</span></span>
<span data-ttu-id="78e5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78e5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e5d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="78e5d-111">Permission type</span></span>|<span data-ttu-id="78e5d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78e5d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e5d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78e5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78e5d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e5d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78e5d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78e5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e5d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="78e5d-116">Not supported.</span></span>|
|<span data-ttu-id="78e5d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="78e5d-117">Application</span></span>|<span data-ttu-id="78e5d-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e5d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e5d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78e5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="78e5d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="78e5d-120">Request headers</span></span>
|<span data-ttu-id="78e5d-121">标头</span><span class="sxs-lookup"><span data-stu-id="78e5d-121">Header</span></span>|<span data-ttu-id="78e5d-122">值</span><span class="sxs-lookup"><span data-stu-id="78e5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78e5d-123">Authorization</span></span>|<span data-ttu-id="78e5d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78e5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e5d-125">接受</span><span class="sxs-lookup"><span data-stu-id="78e5d-125">Accept</span></span>|<span data-ttu-id="78e5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78e5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e5d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="78e5d-127">Request body</span></span>
<span data-ttu-id="78e5d-128">在请求正文中，提供 deviceManagementConfigurationPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78e5d-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicy object.</span></span>

<span data-ttu-id="78e5d-129">下表显示创建 deviceManagementConfigurationPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="78e5d-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicy.</span></span>

|<span data-ttu-id="78e5d-130">属性</span><span class="sxs-lookup"><span data-stu-id="78e5d-130">Property</span></span>|<span data-ttu-id="78e5d-131">类型</span><span class="sxs-lookup"><span data-stu-id="78e5d-131">Type</span></span>|<span data-ttu-id="78e5d-132">说明</span><span class="sxs-lookup"><span data-stu-id="78e5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e5d-133">id</span><span class="sxs-lookup"><span data-stu-id="78e5d-133">id</span></span>|<span data-ttu-id="78e5d-134">String</span><span class="sxs-lookup"><span data-stu-id="78e5d-134">String</span></span>|<span data-ttu-id="78e5d-135">策略文档的键。</span><span class="sxs-lookup"><span data-stu-id="78e5d-135">Key of the policy document.</span></span> <span data-ttu-id="78e5d-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="78e5d-136">Automatically generated.</span></span>|
|<span data-ttu-id="78e5d-137">name</span><span class="sxs-lookup"><span data-stu-id="78e5d-137">name</span></span>|<span data-ttu-id="78e5d-138">String</span><span class="sxs-lookup"><span data-stu-id="78e5d-138">String</span></span>|<span data-ttu-id="78e5d-139">策略名称</span><span class="sxs-lookup"><span data-stu-id="78e5d-139">Policy name</span></span>|
|<span data-ttu-id="78e5d-140">说明</span><span class="sxs-lookup"><span data-stu-id="78e5d-140">description</span></span>|<span data-ttu-id="78e5d-141">String</span><span class="sxs-lookup"><span data-stu-id="78e5d-141">String</span></span>|<span data-ttu-id="78e5d-142">策略说明</span><span class="sxs-lookup"><span data-stu-id="78e5d-142">Policy description</span></span>|
|<span data-ttu-id="78e5d-143">平台</span><span class="sxs-lookup"><span data-stu-id="78e5d-143">platforms</span></span>|[<span data-ttu-id="78e5d-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="78e5d-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="78e5d-145">此策略的平台。</span><span class="sxs-lookup"><span data-stu-id="78e5d-145">Platforms for this policy.</span></span> <span data-ttu-id="78e5d-146">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="78e5d-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="78e5d-147">technologies</span><span class="sxs-lookup"><span data-stu-id="78e5d-147">technologies</span></span>|[<span data-ttu-id="78e5d-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="78e5d-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="78e5d-149">此策略的技术。</span><span class="sxs-lookup"><span data-stu-id="78e5d-149">Technologies for this policy.</span></span> <span data-ttu-id="78e5d-150">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`。</span><span class="sxs-lookup"><span data-stu-id="78e5d-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="78e5d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78e5d-151">createdDateTime</span></span>|<span data-ttu-id="78e5d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e5d-152">DateTimeOffset</span></span>|<span data-ttu-id="78e5d-153">策略创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78e5d-153">Policy creation date and time.</span></span> <span data-ttu-id="78e5d-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="78e5d-154">This property is read-only.</span></span>|
|<span data-ttu-id="78e5d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78e5d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="78e5d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e5d-156">DateTimeOffset</span></span>|<span data-ttu-id="78e5d-157">策略上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="78e5d-157">Policy last modification date and time.</span></span> <span data-ttu-id="78e5d-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="78e5d-158">This property is read-only.</span></span>|
|<span data-ttu-id="78e5d-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="78e5d-159">settingCount</span></span>|<span data-ttu-id="78e5d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="78e5d-160">Int32</span></span>|<span data-ttu-id="78e5d-161">设置数。</span><span class="sxs-lookup"><span data-stu-id="78e5d-161">Number of settings.</span></span> <span data-ttu-id="78e5d-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="78e5d-162">This property is read-only.</span></span>|
|<span data-ttu-id="78e5d-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="78e5d-163">creationSource</span></span>|<span data-ttu-id="78e5d-164">String</span><span class="sxs-lookup"><span data-stu-id="78e5d-164">String</span></span>|<span data-ttu-id="78e5d-165">策略创建源</span><span class="sxs-lookup"><span data-stu-id="78e5d-165">Policy creation source</span></span>|
|<span data-ttu-id="78e5d-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="78e5d-166">roleScopeTagIds</span></span>|<span data-ttu-id="78e5d-167">String collection</span><span class="sxs-lookup"><span data-stu-id="78e5d-167">String collection</span></span>|<span data-ttu-id="78e5d-168">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="78e5d-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="78e5d-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="78e5d-169">isAssigned</span></span>|<span data-ttu-id="78e5d-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="78e5d-170">Boolean</span></span>|<span data-ttu-id="78e5d-171">策略分配状态。</span><span class="sxs-lookup"><span data-stu-id="78e5d-171">Policy assignment status.</span></span> <span data-ttu-id="78e5d-172">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="78e5d-172">This property is read-only.</span></span>|
|<span data-ttu-id="78e5d-173">templateReference</span><span class="sxs-lookup"><span data-stu-id="78e5d-173">templateReference</span></span>|[<span data-ttu-id="78e5d-174">deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="78e5d-174">deviceManagementConfigurationPolicyTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplatereference.md)|<span data-ttu-id="78e5d-175">模板参考信息</span><span class="sxs-lookup"><span data-stu-id="78e5d-175">Template reference information</span></span>|



## <a name="response"></a><span data-ttu-id="78e5d-176">响应</span><span class="sxs-lookup"><span data-stu-id="78e5d-176">Response</span></span>
<span data-ttu-id="78e5d-177">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78e5d-177">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e5d-178">示例</span><span class="sxs-lookup"><span data-stu-id="78e5d-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="78e5d-179">请求</span><span class="sxs-lookup"><span data-stu-id="78e5d-179">Request</span></span>
<span data-ttu-id="78e5d-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78e5d-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies
Content-type: application/json
Content-length: 685

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "Template Id value",
    "templateFamily": "endpointSecurityAntivirus",
    "templateDisplayName": "Template Display Name value",
    "templateDisplayVersion": "Template Display Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="78e5d-181">响应</span><span class="sxs-lookup"><span data-stu-id="78e5d-181">Response</span></span>
<span data-ttu-id="78e5d-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78e5d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 857

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true,
  "templateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
    "templateId": "Template Id value",
    "templateFamily": "endpointSecurityAntivirus",
    "templateDisplayName": "Template Display Name value",
    "templateDisplayVersion": "Template Display Version value"
  }
}
```




