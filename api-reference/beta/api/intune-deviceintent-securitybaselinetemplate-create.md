---
title: 创建 securityBaselineTemplate
description: 创建新的 securityBaselineTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c56758ab2f1cc75149fb63aa77a83a67873d0fb7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154502"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="9bd22-103">创建 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="9bd22-103">Create securityBaselineTemplate</span></span>

<span data-ttu-id="9bd22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bd22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bd22-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9bd22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bd22-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9bd22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bd22-107">创建新的 [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bd22-107">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bd22-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9bd22-108">Prerequisites</span></span>
<span data-ttu-id="9bd22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bd22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd22-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bd22-111">Permission type</span></span>|<span data-ttu-id="9bd22-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bd22-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bd22-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bd22-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bd22-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bd22-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bd22-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bd22-116">Not supported.</span></span>|
|<span data-ttu-id="9bd22-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bd22-117">Application</span></span>|<span data-ttu-id="9bd22-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bd22-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bd22-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bd22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="9bd22-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bd22-120">Request headers</span></span>
|<span data-ttu-id="9bd22-121">标头</span><span class="sxs-lookup"><span data-stu-id="9bd22-121">Header</span></span>|<span data-ttu-id="9bd22-122">值</span><span class="sxs-lookup"><span data-stu-id="9bd22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bd22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd22-123">Authorization</span></span>|<span data-ttu-id="9bd22-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9bd22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bd22-125">接受</span><span class="sxs-lookup"><span data-stu-id="9bd22-125">Accept</span></span>|<span data-ttu-id="9bd22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bd22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bd22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bd22-127">Request body</span></span>
<span data-ttu-id="9bd22-128">在请求正文中，提供 securityBaselineTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bd22-128">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="9bd22-129">下表显示创建 securityBaselineTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9bd22-129">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="9bd22-130">属性</span><span class="sxs-lookup"><span data-stu-id="9bd22-130">Property</span></span>|<span data-ttu-id="9bd22-131">类型</span><span class="sxs-lookup"><span data-stu-id="9bd22-131">Type</span></span>|<span data-ttu-id="9bd22-132">说明</span><span class="sxs-lookup"><span data-stu-id="9bd22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bd22-133">id</span><span class="sxs-lookup"><span data-stu-id="9bd22-133">id</span></span>|<span data-ttu-id="9bd22-134">String</span><span class="sxs-lookup"><span data-stu-id="9bd22-134">String</span></span>|<span data-ttu-id="9bd22-135">模板 ID 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9bd22-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="9bd22-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9bd22-136">displayName</span></span>|<span data-ttu-id="9bd22-137">String</span><span class="sxs-lookup"><span data-stu-id="9bd22-137">String</span></span>|<span data-ttu-id="9bd22-138">模板的模板显示名称继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9bd22-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="9bd22-139">说明</span><span class="sxs-lookup"><span data-stu-id="9bd22-139">description</span></span>|<span data-ttu-id="9bd22-140">String</span><span class="sxs-lookup"><span data-stu-id="9bd22-140">String</span></span>|<span data-ttu-id="9bd22-141">模板的说明 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9bd22-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="9bd22-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="9bd22-142">versionInfo</span></span>|<span data-ttu-id="9bd22-143">String</span><span class="sxs-lookup"><span data-stu-id="9bd22-143">String</span></span>|<span data-ttu-id="9bd22-144">模板的版本信息 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9bd22-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="9bd22-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="9bd22-145">isDeprecated</span></span>|<span data-ttu-id="9bd22-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd22-146">Boolean</span></span>|<span data-ttu-id="9bd22-147">模板是否被弃用。</span><span class="sxs-lookup"><span data-stu-id="9bd22-147">The template is deprecated or not.</span></span> <span data-ttu-id="9bd22-148">无法从已弃用模板创建意图。</span><span class="sxs-lookup"><span data-stu-id="9bd22-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="9bd22-149">继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9bd22-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="9bd22-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="9bd22-150">intentCount</span></span>|<span data-ttu-id="9bd22-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9bd22-151">Int32</span></span>|<span data-ttu-id="9bd22-152">从此模板创建的意图数。</span><span class="sxs-lookup"><span data-stu-id="9bd22-152">Number of Intents created from this template.</span></span> <span data-ttu-id="9bd22-153">继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9bd22-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="9bd22-154">templateType</span><span class="sxs-lookup"><span data-stu-id="9bd22-154">templateType</span></span>|[<span data-ttu-id="9bd22-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="9bd22-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="9bd22-156">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="9bd22-156">The template's type.</span></span> <span data-ttu-id="9bd22-157">继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="9bd22-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="9bd22-158">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`、`deviceConfigurationForOffice365`、`cloudPC`、`firewallSharedSettings`。</span><span class="sxs-lookup"><span data-stu-id="9bd22-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="9bd22-159">platformType</span><span class="sxs-lookup"><span data-stu-id="9bd22-159">platformType</span></span>|[<span data-ttu-id="9bd22-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="9bd22-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="9bd22-161">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="9bd22-161">The template's platform.</span></span> <span data-ttu-id="9bd22-162">继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="9bd22-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="9bd22-163">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="9bd22-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="9bd22-164">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="9bd22-164">templateSubtype</span></span>|[<span data-ttu-id="9bd22-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="9bd22-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="9bd22-166">模板的子类型。</span><span class="sxs-lookup"><span data-stu-id="9bd22-166">The template's subtype.</span></span> <span data-ttu-id="9bd22-167">继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="9bd22-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="9bd22-168">可取值为：`none`、`firewall`、`diskEncryption`、`attackSurfaceReduction`、`endpointDetectionReponse`、`accountProtection`、`antivirus`、`firewallSharedAppList`、`firewallSharedIpList`、`firewallSharedPortlist`。</span><span class="sxs-lookup"><span data-stu-id="9bd22-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="9bd22-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bd22-169">publishedDateTime</span></span>|<span data-ttu-id="9bd22-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bd22-170">DateTimeOffset</span></span>|<span data-ttu-id="9bd22-171">发布模板时 继承自 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9bd22-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9bd22-172">响应</span><span class="sxs-lookup"><span data-stu-id="9bd22-172">Response</span></span>
<span data-ttu-id="9bd22-173">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bd22-173">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bd22-174">示例</span><span class="sxs-lookup"><span data-stu-id="9bd22-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bd22-175">请求</span><span class="sxs-lookup"><span data-stu-id="9bd22-175">Request</span></span>
<span data-ttu-id="9bd22-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9bd22-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="9bd22-177">响应</span><span class="sxs-lookup"><span data-stu-id="9bd22-177">Response</span></span>
<span data-ttu-id="9bd22-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bd22-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```




