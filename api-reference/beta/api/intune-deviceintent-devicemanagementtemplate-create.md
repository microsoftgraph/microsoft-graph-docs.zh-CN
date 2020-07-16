---
title: 创建 deviceManagementTemplate
description: 创建新的 deviceManagementTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc741640f5f8762985ccbe7ad2d261524f9ee73c
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122754"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="6308e-103">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="6308e-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="6308e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6308e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6308e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6308e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6308e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6308e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6308e-107">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6308e-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6308e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6308e-108">Prerequisites</span></span>
<span data-ttu-id="6308e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6308e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6308e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6308e-111">Permission type</span></span>|<span data-ttu-id="6308e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6308e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6308e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6308e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6308e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6308e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6308e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6308e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6308e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6308e-116">Not supported.</span></span>|
|<span data-ttu-id="6308e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6308e-117">Application</span></span>|<span data-ttu-id="6308e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6308e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6308e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6308e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="6308e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6308e-120">Request headers</span></span>
|<span data-ttu-id="6308e-121">标头</span><span class="sxs-lookup"><span data-stu-id="6308e-121">Header</span></span>|<span data-ttu-id="6308e-122">值</span><span class="sxs-lookup"><span data-stu-id="6308e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6308e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6308e-123">Authorization</span></span>|<span data-ttu-id="6308e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6308e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6308e-125">接受</span><span class="sxs-lookup"><span data-stu-id="6308e-125">Accept</span></span>|<span data-ttu-id="6308e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6308e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6308e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6308e-127">Request body</span></span>
<span data-ttu-id="6308e-128">在请求正文中，提供 deviceManagementTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6308e-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="6308e-129">下表显示创建 deviceManagementTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6308e-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="6308e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6308e-130">Property</span></span>|<span data-ttu-id="6308e-131">类型</span><span class="sxs-lookup"><span data-stu-id="6308e-131">Type</span></span>|<span data-ttu-id="6308e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6308e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6308e-133">id</span><span class="sxs-lookup"><span data-stu-id="6308e-133">id</span></span>|<span data-ttu-id="6308e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6308e-134">String</span></span>|<span data-ttu-id="6308e-135">模板 ID</span><span class="sxs-lookup"><span data-stu-id="6308e-135">The template ID</span></span>|
|<span data-ttu-id="6308e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6308e-136">displayName</span></span>|<span data-ttu-id="6308e-137">String</span><span class="sxs-lookup"><span data-stu-id="6308e-137">String</span></span>|<span data-ttu-id="6308e-138">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="6308e-138">The template's display name</span></span>|
|<span data-ttu-id="6308e-139">说明</span><span class="sxs-lookup"><span data-stu-id="6308e-139">description</span></span>|<span data-ttu-id="6308e-140">String</span><span class="sxs-lookup"><span data-stu-id="6308e-140">String</span></span>|<span data-ttu-id="6308e-141">模板的说明</span><span class="sxs-lookup"><span data-stu-id="6308e-141">The template's description</span></span>|
|<span data-ttu-id="6308e-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="6308e-142">versionInfo</span></span>|<span data-ttu-id="6308e-143">String</span><span class="sxs-lookup"><span data-stu-id="6308e-143">String</span></span>|<span data-ttu-id="6308e-144">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="6308e-144">The template's version information</span></span>|
|<span data-ttu-id="6308e-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="6308e-145">isDeprecated</span></span>|<span data-ttu-id="6308e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6308e-146">Boolean</span></span>|<span data-ttu-id="6308e-147">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="6308e-147">The template is deprecated or not.</span></span> <span data-ttu-id="6308e-148">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="6308e-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="6308e-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="6308e-149">intentCount</span></span>|<span data-ttu-id="6308e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6308e-150">Int32</span></span>|<span data-ttu-id="6308e-151">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="6308e-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="6308e-152">templateType</span><span class="sxs-lookup"><span data-stu-id="6308e-152">templateType</span></span>|[<span data-ttu-id="6308e-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="6308e-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="6308e-154">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="6308e-154">The template's type.</span></span> <span data-ttu-id="6308e-155">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`、`deviceConfigurationForOffice365`。</span><span class="sxs-lookup"><span data-stu-id="6308e-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span></span>|
|<span data-ttu-id="6308e-156">platformType</span><span class="sxs-lookup"><span data-stu-id="6308e-156">platformType</span></span>|[<span data-ttu-id="6308e-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="6308e-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="6308e-158">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="6308e-158">The template's platform.</span></span> <span data-ttu-id="6308e-159">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="6308e-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="6308e-160">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="6308e-160">templateSubtype</span></span>|[<span data-ttu-id="6308e-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="6308e-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="6308e-162">模板的子类型。</span><span class="sxs-lookup"><span data-stu-id="6308e-162">The template's subtype.</span></span> <span data-ttu-id="6308e-163">可取值为：`none`、`firewall`、`diskEncryption`、`attackSurfaceReduction`、`endpointDetectionReponse`、`accountProtection` 或 `antivirus`。</span><span class="sxs-lookup"><span data-stu-id="6308e-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span></span>|
|<span data-ttu-id="6308e-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="6308e-164">publishedDateTime</span></span>|<span data-ttu-id="6308e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6308e-165">DateTimeOffset</span></span>|<span data-ttu-id="6308e-166">发布模板时</span><span class="sxs-lookup"><span data-stu-id="6308e-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="6308e-167">响应</span><span class="sxs-lookup"><span data-stu-id="6308e-167">Response</span></span>
<span data-ttu-id="6308e-168">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6308e-168">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6308e-169">示例</span><span class="sxs-lookup"><span data-stu-id="6308e-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="6308e-170">请求</span><span class="sxs-lookup"><span data-stu-id="6308e-170">Request</span></span>
<span data-ttu-id="6308e-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6308e-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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

### <a name="response"></a><span data-ttu-id="6308e-172">响应</span><span class="sxs-lookup"><span data-stu-id="6308e-172">Response</span></span>
<span data-ttu-id="6308e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6308e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
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



