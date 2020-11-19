---
title: 更新 deviceManagementTemplate
description: 更新 deviceManagementTemplate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bcfbf6400a7b81bc62ed7d4083ef3d3810b6a69b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49264210"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="0ecc2-103">更新 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="0ecc2-103">Update deviceManagementTemplate</span></span>

<span data-ttu-id="0ecc2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ecc2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ecc2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ecc2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ecc2-107">更新 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-107">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ecc2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ecc2-108">Prerequisites</span></span>
<span data-ttu-id="0ecc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ecc2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ecc2-111">Permission type</span></span>|<span data-ttu-id="0ecc2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ecc2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ecc2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ecc2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ecc2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ecc2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ecc2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ecc2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ecc2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-116">Not supported.</span></span>|
|<span data-ttu-id="0ecc2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ecc2-117">Application</span></span>|<span data-ttu-id="0ecc2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ecc2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ecc2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ecc2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="0ecc2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ecc2-120">Request headers</span></span>
|<span data-ttu-id="0ecc2-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ecc2-121">Header</span></span>|<span data-ttu-id="0ecc2-122">值</span><span class="sxs-lookup"><span data-stu-id="0ecc2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ecc2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ecc2-123">Authorization</span></span>|<span data-ttu-id="0ecc2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ecc2-125">接受</span><span class="sxs-lookup"><span data-stu-id="0ecc2-125">Accept</span></span>|<span data-ttu-id="0ecc2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ecc2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ecc2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ecc2-127">Request body</span></span>
<span data-ttu-id="0ecc2-128">在请求正文中，提供 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-128">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="0ecc2-129">下表显示创建 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-129">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="0ecc2-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ecc2-130">Property</span></span>|<span data-ttu-id="0ecc2-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ecc2-131">Type</span></span>|<span data-ttu-id="0ecc2-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ecc2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ecc2-133">id</span><span class="sxs-lookup"><span data-stu-id="0ecc2-133">id</span></span>|<span data-ttu-id="0ecc2-134">String</span><span class="sxs-lookup"><span data-stu-id="0ecc2-134">String</span></span>|<span data-ttu-id="0ecc2-135">模板 ID</span><span class="sxs-lookup"><span data-stu-id="0ecc2-135">The template ID</span></span>|
|<span data-ttu-id="0ecc2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0ecc2-136">displayName</span></span>|<span data-ttu-id="0ecc2-137">String</span><span class="sxs-lookup"><span data-stu-id="0ecc2-137">String</span></span>|<span data-ttu-id="0ecc2-138">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="0ecc2-138">The template's display name</span></span>|
|<span data-ttu-id="0ecc2-139">description</span><span class="sxs-lookup"><span data-stu-id="0ecc2-139">description</span></span>|<span data-ttu-id="0ecc2-140">String</span><span class="sxs-lookup"><span data-stu-id="0ecc2-140">String</span></span>|<span data-ttu-id="0ecc2-141">模板的说明</span><span class="sxs-lookup"><span data-stu-id="0ecc2-141">The template's description</span></span>|
|<span data-ttu-id="0ecc2-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="0ecc2-142">versionInfo</span></span>|<span data-ttu-id="0ecc2-143">String</span><span class="sxs-lookup"><span data-stu-id="0ecc2-143">String</span></span>|<span data-ttu-id="0ecc2-144">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="0ecc2-144">The template's version information</span></span>|
|<span data-ttu-id="0ecc2-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="0ecc2-145">isDeprecated</span></span>|<span data-ttu-id="0ecc2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ecc2-146">Boolean</span></span>|<span data-ttu-id="0ecc2-147">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-147">The template is deprecated or not.</span></span> <span data-ttu-id="0ecc2-148">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="0ecc2-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="0ecc2-149">intentCount</span></span>|<span data-ttu-id="0ecc2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0ecc2-150">Int32</span></span>|<span data-ttu-id="0ecc2-151">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="0ecc2-152">templateType</span><span class="sxs-lookup"><span data-stu-id="0ecc2-152">templateType</span></span>|[<span data-ttu-id="0ecc2-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="0ecc2-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="0ecc2-154">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-154">The template's type.</span></span> <span data-ttu-id="0ecc2-155">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`、`deviceConfigurationForOffice365`、`cloudPC`、`firewallSharedSettings`。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="0ecc2-156">platformType</span><span class="sxs-lookup"><span data-stu-id="0ecc2-156">platformType</span></span>|[<span data-ttu-id="0ecc2-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0ecc2-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="0ecc2-158">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-158">The template's platform.</span></span> <span data-ttu-id="0ecc2-159">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="0ecc2-160">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="0ecc2-160">templateSubtype</span></span>|[<span data-ttu-id="0ecc2-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="0ecc2-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="0ecc2-162">模板的子类型。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-162">The template's subtype.</span></span> <span data-ttu-id="0ecc2-163">可取值为：`none`、`firewall`、`diskEncryption`、`attackSurfaceReduction`、`endpointDetectionReponse`、`accountProtection`、`antivirus`、`firewallSharedAppList`、`firewallSharedIpList`、`firewallSharedPortlist`。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="0ecc2-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecc2-164">publishedDateTime</span></span>|<span data-ttu-id="0ecc2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecc2-165">DateTimeOffset</span></span>|<span data-ttu-id="0ecc2-166">发布模板时</span><span class="sxs-lookup"><span data-stu-id="0ecc2-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="0ecc2-167">响应</span><span class="sxs-lookup"><span data-stu-id="0ecc2-167">Response</span></span>
<span data-ttu-id="0ecc2-168">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ecc2-169">示例</span><span class="sxs-lookup"><span data-stu-id="0ecc2-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ecc2-170">请求</span><span class="sxs-lookup"><span data-stu-id="0ecc2-170">Request</span></span>
<span data-ttu-id="0ecc2-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="0ecc2-172">响应</span><span class="sxs-lookup"><span data-stu-id="0ecc2-172">Response</span></span>
<span data-ttu-id="0ecc2-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ecc2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




