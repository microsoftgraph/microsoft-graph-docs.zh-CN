---
title: 更新 deviceManagementConfigurationPolicyTemplate
description: 更新 deviceManagementConfigurationPolicyTemplate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c3856862b0706c4eb30340d76c35275eb797e68
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665689"
---
# <a name="update-devicemanagementconfigurationpolicytemplate"></a><span data-ttu-id="05c07-103">更新 deviceManagementConfigurationPolicyTemplate</span><span class="sxs-lookup"><span data-stu-id="05c07-103">Update deviceManagementConfigurationPolicyTemplate</span></span>

<span data-ttu-id="05c07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05c07-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05c07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05c07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05c07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c07-107">更新 [deviceManagementConfigurationPolicyTemplate 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="05c07-107">Update the properties of a [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05c07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="05c07-108">Prerequisites</span></span>
<span data-ttu-id="05c07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05c07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="05c07-111">Permission type</span></span>|<span data-ttu-id="05c07-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05c07-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05c07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05c07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05c07-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c07-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05c07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05c07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05c07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05c07-116">Not supported.</span></span>|
|<span data-ttu-id="05c07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="05c07-117">Application</span></span>|<span data-ttu-id="05c07-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c07-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05c07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05c07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="05c07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05c07-120">Request headers</span></span>
|<span data-ttu-id="05c07-121">标头</span><span class="sxs-lookup"><span data-stu-id="05c07-121">Header</span></span>|<span data-ttu-id="05c07-122">值</span><span class="sxs-lookup"><span data-stu-id="05c07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05c07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05c07-123">Authorization</span></span>|<span data-ttu-id="05c07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05c07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05c07-125">接受</span><span class="sxs-lookup"><span data-stu-id="05c07-125">Accept</span></span>|<span data-ttu-id="05c07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05c07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05c07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05c07-127">Request body</span></span>
<span data-ttu-id="05c07-128">在请求正文中，提供 [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05c07-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object.</span></span>

<span data-ttu-id="05c07-129">下表显示创建 [deviceManagementConfigurationPolicyTemplate 时所需的属性](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="05c07-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md).</span></span>

|<span data-ttu-id="05c07-130">属性</span><span class="sxs-lookup"><span data-stu-id="05c07-130">Property</span></span>|<span data-ttu-id="05c07-131">类型</span><span class="sxs-lookup"><span data-stu-id="05c07-131">Type</span></span>|<span data-ttu-id="05c07-132">说明</span><span class="sxs-lookup"><span data-stu-id="05c07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05c07-133">id</span><span class="sxs-lookup"><span data-stu-id="05c07-133">id</span></span>|<span data-ttu-id="05c07-134">String</span><span class="sxs-lookup"><span data-stu-id="05c07-134">String</span></span>|<span data-ttu-id="05c07-135">由 BaseId 和 Version 组成的模板文档的键。</span><span class="sxs-lookup"><span data-stu-id="05c07-135">Key of the template document, composed of BaseId and Version.</span></span> <span data-ttu-id="05c07-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="05c07-136">Automatically generated.</span></span>|
|<span data-ttu-id="05c07-137">baseId</span><span class="sxs-lookup"><span data-stu-id="05c07-137">baseId</span></span>|<span data-ttu-id="05c07-138">String</span><span class="sxs-lookup"><span data-stu-id="05c07-138">String</span></span>|<span data-ttu-id="05c07-139">模板基本标识符</span><span class="sxs-lookup"><span data-stu-id="05c07-139">Template base identifier</span></span>|
|<span data-ttu-id="05c07-140">version</span><span class="sxs-lookup"><span data-stu-id="05c07-140">version</span></span>|<span data-ttu-id="05c07-141">Int32</span><span class="sxs-lookup"><span data-stu-id="05c07-141">Int32</span></span>|<span data-ttu-id="05c07-142">模板版本。</span><span class="sxs-lookup"><span data-stu-id="05c07-142">Template version.</span></span> <span data-ttu-id="05c07-143">有效值为 1 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="05c07-143">Valid values 1 to 2147483647.</span></span> <span data-ttu-id="05c07-144">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="05c07-144">This property is read-only.</span></span>|
|<span data-ttu-id="05c07-145">displayName</span><span class="sxs-lookup"><span data-stu-id="05c07-145">displayName</span></span>|<span data-ttu-id="05c07-146">String</span><span class="sxs-lookup"><span data-stu-id="05c07-146">String</span></span>|<span data-ttu-id="05c07-147">模板显示名称</span><span class="sxs-lookup"><span data-stu-id="05c07-147">Template display name</span></span>|
|<span data-ttu-id="05c07-148">说明</span><span class="sxs-lookup"><span data-stu-id="05c07-148">description</span></span>|<span data-ttu-id="05c07-149">String</span><span class="sxs-lookup"><span data-stu-id="05c07-149">String</span></span>|<span data-ttu-id="05c07-150">模板说明</span><span class="sxs-lookup"><span data-stu-id="05c07-150">Template description</span></span>|
|<span data-ttu-id="05c07-151">displayVersion</span><span class="sxs-lookup"><span data-stu-id="05c07-151">displayVersion</span></span>|<span data-ttu-id="05c07-152">String</span><span class="sxs-lookup"><span data-stu-id="05c07-152">String</span></span>|<span data-ttu-id="05c07-153">模板版本说明</span><span class="sxs-lookup"><span data-stu-id="05c07-153">Description of template version</span></span>|
|<span data-ttu-id="05c07-154">lifecycleState</span><span class="sxs-lookup"><span data-stu-id="05c07-154">lifecycleState</span></span>|[<span data-ttu-id="05c07-155">deviceManagementTemplateLifecycleState</span><span class="sxs-lookup"><span data-stu-id="05c07-155">deviceManagementTemplateLifecycleState</span></span>](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|<span data-ttu-id="05c07-156">指示模板的当前生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="05c07-156">Indicate current lifecycle state of template.</span></span> <span data-ttu-id="05c07-157">可取值为：`invalid`、`draft`、`active`、`superseded`、`deprecated`、`retired`。</span><span class="sxs-lookup"><span data-stu-id="05c07-157">Possible values are: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.</span></span>|
|<span data-ttu-id="05c07-158">平台</span><span class="sxs-lookup"><span data-stu-id="05c07-158">platforms</span></span>|[<span data-ttu-id="05c07-159">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="05c07-159">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="05c07-160">此模板的平台。</span><span class="sxs-lookup"><span data-stu-id="05c07-160">Platforms for this template.</span></span> <span data-ttu-id="05c07-161">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="05c07-161">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="05c07-162">technologies</span><span class="sxs-lookup"><span data-stu-id="05c07-162">technologies</span></span>|[<span data-ttu-id="05c07-163">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="05c07-163">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="05c07-164">此模板的技术。</span><span class="sxs-lookup"><span data-stu-id="05c07-164">Technologies for this template.</span></span> <span data-ttu-id="05c07-165">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`。</span><span class="sxs-lookup"><span data-stu-id="05c07-165">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="05c07-166">templateFamily</span><span class="sxs-lookup"><span data-stu-id="05c07-166">templateFamily</span></span>|[<span data-ttu-id="05c07-167">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="05c07-167">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="05c07-168">TemplateFamily 此模板。</span><span class="sxs-lookup"><span data-stu-id="05c07-168">TemplateFamily for this template.</span></span> <span data-ttu-id="05c07-169">可取值为：`none`、`endpointSecurityAntivirus`、`endpointSecurityDiskEncryption`、`endpointSecurityFirewall`、`endpointSecurityEndpointDetectionAndResponse`、`endpointSecurityAttackSurfaceReduction`、`endpointSecurityAccountProtection`、`endpointSecurityApplicationControl`。</span><span class="sxs-lookup"><span data-stu-id="05c07-169">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="05c07-170">allowUnmanagedSettings</span><span class="sxs-lookup"><span data-stu-id="05c07-170">allowUnmanagedSettings</span></span>|<span data-ttu-id="05c07-171">布尔值</span><span class="sxs-lookup"><span data-stu-id="05c07-171">Boolean</span></span>|<span data-ttu-id="05c07-172">允许非托管设置模板</span><span class="sxs-lookup"><span data-stu-id="05c07-172">Allow unmanaged setting templates</span></span>|
|<span data-ttu-id="05c07-173">settingTemplateCount</span><span class="sxs-lookup"><span data-stu-id="05c07-173">settingTemplateCount</span></span>|<span data-ttu-id="05c07-174">Int32</span><span class="sxs-lookup"><span data-stu-id="05c07-174">Int32</span></span>|<span data-ttu-id="05c07-175">设置模板的数量。</span><span class="sxs-lookup"><span data-stu-id="05c07-175">Number of setting templates.</span></span> <span data-ttu-id="05c07-176">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="05c07-176">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="05c07-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="05c07-177">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="05c07-178">响应</span><span class="sxs-lookup"><span data-stu-id="05c07-178">Response</span></span>
<span data-ttu-id="05c07-179">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05c07-179">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05c07-180">示例</span><span class="sxs-lookup"><span data-stu-id="05c07-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="05c07-181">请求</span><span class="sxs-lookup"><span data-stu-id="05c07-181">Request</span></span>
<span data-ttu-id="05c07-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05c07-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}
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

### <a name="response"></a><span data-ttu-id="05c07-183">响应</span><span class="sxs-lookup"><span data-stu-id="05c07-183">Response</span></span>
<span data-ttu-id="05c07-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05c07-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




