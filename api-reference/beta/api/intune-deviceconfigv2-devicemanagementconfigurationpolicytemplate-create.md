---
title: 创建 deviceManagementConfigurationPolicyTemplate
description: 创建新的 deviceManagementConfigurationPolicyTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbbcabc3d531505ef53aab117cec7e8b6e8e594f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665693"
---
# <a name="create-devicemanagementconfigurationpolicytemplate"></a><span data-ttu-id="fb486-103">创建 deviceManagementConfigurationPolicyTemplate</span><span class="sxs-lookup"><span data-stu-id="fb486-103">Create deviceManagementConfigurationPolicyTemplate</span></span>

<span data-ttu-id="fb486-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb486-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb486-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb486-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb486-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb486-107">创建新的 [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb486-107">Create a new [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb486-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb486-108">Prerequisites</span></span>
<span data-ttu-id="fb486-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb486-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb486-111">Permission type</span></span>|<span data-ttu-id="fb486-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb486-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb486-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb486-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb486-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb486-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb486-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb486-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb486-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb486-116">Not supported.</span></span>|
|<span data-ttu-id="fb486-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb486-117">Application</span></span>|<span data-ttu-id="fb486-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb486-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb486-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb486-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicyTemplates
```

## <a name="request-headers"></a><span data-ttu-id="fb486-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb486-120">Request headers</span></span>
|<span data-ttu-id="fb486-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb486-121">Header</span></span>|<span data-ttu-id="fb486-122">值</span><span class="sxs-lookup"><span data-stu-id="fb486-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb486-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb486-123">Authorization</span></span>|<span data-ttu-id="fb486-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb486-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb486-125">接受</span><span class="sxs-lookup"><span data-stu-id="fb486-125">Accept</span></span>|<span data-ttu-id="fb486-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb486-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb486-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb486-127">Request body</span></span>
<span data-ttu-id="fb486-128">在请求正文中，提供 deviceManagementConfigurationPolicyTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb486-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicyTemplate object.</span></span>

<span data-ttu-id="fb486-129">下表显示创建 deviceManagementConfigurationPolicyTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb486-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicyTemplate.</span></span>

|<span data-ttu-id="fb486-130">属性</span><span class="sxs-lookup"><span data-stu-id="fb486-130">Property</span></span>|<span data-ttu-id="fb486-131">类型</span><span class="sxs-lookup"><span data-stu-id="fb486-131">Type</span></span>|<span data-ttu-id="fb486-132">说明</span><span class="sxs-lookup"><span data-stu-id="fb486-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb486-133">id</span><span class="sxs-lookup"><span data-stu-id="fb486-133">id</span></span>|<span data-ttu-id="fb486-134">String</span><span class="sxs-lookup"><span data-stu-id="fb486-134">String</span></span>|<span data-ttu-id="fb486-135">由 BaseId 和 Version 组成的模板文档的键。</span><span class="sxs-lookup"><span data-stu-id="fb486-135">Key of the template document, composed of BaseId and Version.</span></span> <span data-ttu-id="fb486-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="fb486-136">Automatically generated.</span></span>|
|<span data-ttu-id="fb486-137">baseId</span><span class="sxs-lookup"><span data-stu-id="fb486-137">baseId</span></span>|<span data-ttu-id="fb486-138">String</span><span class="sxs-lookup"><span data-stu-id="fb486-138">String</span></span>|<span data-ttu-id="fb486-139">模板基本标识符</span><span class="sxs-lookup"><span data-stu-id="fb486-139">Template base identifier</span></span>|
|<span data-ttu-id="fb486-140">version</span><span class="sxs-lookup"><span data-stu-id="fb486-140">version</span></span>|<span data-ttu-id="fb486-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fb486-141">Int32</span></span>|<span data-ttu-id="fb486-142">模板版本。</span><span class="sxs-lookup"><span data-stu-id="fb486-142">Template version.</span></span> <span data-ttu-id="fb486-143">有效值为 1 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="fb486-143">Valid values 1 to 2147483647.</span></span> <span data-ttu-id="fb486-144">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fb486-144">This property is read-only.</span></span>|
|<span data-ttu-id="fb486-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fb486-145">displayName</span></span>|<span data-ttu-id="fb486-146">String</span><span class="sxs-lookup"><span data-stu-id="fb486-146">String</span></span>|<span data-ttu-id="fb486-147">模板显示名称</span><span class="sxs-lookup"><span data-stu-id="fb486-147">Template display name</span></span>|
|<span data-ttu-id="fb486-148">说明</span><span class="sxs-lookup"><span data-stu-id="fb486-148">description</span></span>|<span data-ttu-id="fb486-149">String</span><span class="sxs-lookup"><span data-stu-id="fb486-149">String</span></span>|<span data-ttu-id="fb486-150">模板说明</span><span class="sxs-lookup"><span data-stu-id="fb486-150">Template description</span></span>|
|<span data-ttu-id="fb486-151">displayVersion</span><span class="sxs-lookup"><span data-stu-id="fb486-151">displayVersion</span></span>|<span data-ttu-id="fb486-152">String</span><span class="sxs-lookup"><span data-stu-id="fb486-152">String</span></span>|<span data-ttu-id="fb486-153">模板版本说明</span><span class="sxs-lookup"><span data-stu-id="fb486-153">Description of template version</span></span>|
|<span data-ttu-id="fb486-154">lifecycleState</span><span class="sxs-lookup"><span data-stu-id="fb486-154">lifecycleState</span></span>|[<span data-ttu-id="fb486-155">deviceManagementTemplateLifecycleState</span><span class="sxs-lookup"><span data-stu-id="fb486-155">deviceManagementTemplateLifecycleState</span></span>](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|<span data-ttu-id="fb486-156">指示模板的当前生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="fb486-156">Indicate current lifecycle state of template.</span></span> <span data-ttu-id="fb486-157">可取值为：`invalid`、`draft`、`active`、`superseded`、`deprecated`、`retired`。</span><span class="sxs-lookup"><span data-stu-id="fb486-157">Possible values are: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.</span></span>|
|<span data-ttu-id="fb486-158">平台</span><span class="sxs-lookup"><span data-stu-id="fb486-158">platforms</span></span>|[<span data-ttu-id="fb486-159">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="fb486-159">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="fb486-160">此模板的平台。</span><span class="sxs-lookup"><span data-stu-id="fb486-160">Platforms for this template.</span></span> <span data-ttu-id="fb486-161">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="fb486-161">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="fb486-162">technologies</span><span class="sxs-lookup"><span data-stu-id="fb486-162">technologies</span></span>|[<span data-ttu-id="fb486-163">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="fb486-163">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="fb486-164">此模板的技术。</span><span class="sxs-lookup"><span data-stu-id="fb486-164">Technologies for this template.</span></span> <span data-ttu-id="fb486-165">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`。</span><span class="sxs-lookup"><span data-stu-id="fb486-165">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="fb486-166">templateFamily</span><span class="sxs-lookup"><span data-stu-id="fb486-166">templateFamily</span></span>|[<span data-ttu-id="fb486-167">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="fb486-167">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="fb486-168">TemplateFamily 此模板。</span><span class="sxs-lookup"><span data-stu-id="fb486-168">TemplateFamily for this template.</span></span> <span data-ttu-id="fb486-169">可取值为：`none`、`endpointSecurityAntivirus`、`endpointSecurityDiskEncryption`、`endpointSecurityFirewall`、`endpointSecurityEndpointDetectionAndResponse`、`endpointSecurityAttackSurfaceReduction`、`endpointSecurityAccountProtection`、`endpointSecurityApplicationControl`。</span><span class="sxs-lookup"><span data-stu-id="fb486-169">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="fb486-170">allowUnmanagedSettings</span><span class="sxs-lookup"><span data-stu-id="fb486-170">allowUnmanagedSettings</span></span>|<span data-ttu-id="fb486-171">布尔值</span><span class="sxs-lookup"><span data-stu-id="fb486-171">Boolean</span></span>|<span data-ttu-id="fb486-172">允许非托管设置模板</span><span class="sxs-lookup"><span data-stu-id="fb486-172">Allow unmanaged setting templates</span></span>|
|<span data-ttu-id="fb486-173">settingTemplateCount</span><span class="sxs-lookup"><span data-stu-id="fb486-173">settingTemplateCount</span></span>|<span data-ttu-id="fb486-174">Int32</span><span class="sxs-lookup"><span data-stu-id="fb486-174">Int32</span></span>|<span data-ttu-id="fb486-175">设置模板的数量。</span><span class="sxs-lookup"><span data-stu-id="fb486-175">Number of setting templates.</span></span> <span data-ttu-id="fb486-176">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="fb486-176">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="fb486-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fb486-177">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="fb486-178">响应</span><span class="sxs-lookup"><span data-stu-id="fb486-178">Response</span></span>
<span data-ttu-id="fb486-179">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb486-179">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb486-180">示例</span><span class="sxs-lookup"><span data-stu-id="fb486-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb486-181">请求</span><span class="sxs-lookup"><span data-stu-id="fb486-181">Request</span></span>
<span data-ttu-id="fb486-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb486-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```

### <a name="response"></a><span data-ttu-id="fb486-183">响应</span><span class="sxs-lookup"><span data-stu-id="fb486-183">Response</span></span>
<span data-ttu-id="fb486-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb486-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```




