---
title: 更新 securityBaselineTemplate
description: 更新 securityBaselineTemplate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18a2281455f0611f745abe35c2ce1e6e5d6b61a6
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122726"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="b3ffe-103">更新 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="b3ffe-103">Update securityBaselineTemplate</span></span>

<span data-ttu-id="b3ffe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3ffe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3ffe-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3ffe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3ffe-107">更新[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-107">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3ffe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3ffe-108">Prerequisites</span></span>
<span data-ttu-id="b3ffe-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b3ffe-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b3ffe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3ffe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3ffe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3ffe-111">Permission type</span></span>|<span data-ttu-id="b3ffe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3ffe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3ffe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3ffe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3ffe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3ffe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3ffe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3ffe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3ffe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-116">Not supported.</span></span>|
|<span data-ttu-id="b3ffe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3ffe-117">Application</span></span>|<span data-ttu-id="b3ffe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3ffe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3ffe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3ffe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="b3ffe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3ffe-120">Request headers</span></span>
|<span data-ttu-id="b3ffe-121">标头</span><span class="sxs-lookup"><span data-stu-id="b3ffe-121">Header</span></span>|<span data-ttu-id="b3ffe-122">值</span><span class="sxs-lookup"><span data-stu-id="b3ffe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3ffe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3ffe-123">Authorization</span></span>|<span data-ttu-id="b3ffe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3ffe-125">接受</span><span class="sxs-lookup"><span data-stu-id="b3ffe-125">Accept</span></span>|<span data-ttu-id="b3ffe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3ffe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3ffe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3ffe-127">Request body</span></span>
<span data-ttu-id="b3ffe-128">在请求正文中，提供[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-128">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="b3ffe-129">下表显示创建[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-129">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="b3ffe-130">属性</span><span class="sxs-lookup"><span data-stu-id="b3ffe-130">Property</span></span>|<span data-ttu-id="b3ffe-131">类型</span><span class="sxs-lookup"><span data-stu-id="b3ffe-131">Type</span></span>|<span data-ttu-id="b3ffe-132">说明</span><span class="sxs-lookup"><span data-stu-id="b3ffe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3ffe-133">id</span><span class="sxs-lookup"><span data-stu-id="b3ffe-133">id</span></span>|<span data-ttu-id="b3ffe-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b3ffe-134">String</span></span>|<span data-ttu-id="b3ffe-135">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID</span><span class="sxs-lookup"><span data-stu-id="b3ffe-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="b3ffe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b3ffe-136">displayName</span></span>|<span data-ttu-id="b3ffe-137">String</span><span class="sxs-lookup"><span data-stu-id="b3ffe-137">String</span></span>|<span data-ttu-id="b3ffe-138">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="b3ffe-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="b3ffe-139">说明</span><span class="sxs-lookup"><span data-stu-id="b3ffe-139">description</span></span>|<span data-ttu-id="b3ffe-140">String</span><span class="sxs-lookup"><span data-stu-id="b3ffe-140">String</span></span>|<span data-ttu-id="b3ffe-141">模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b3ffe-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="b3ffe-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="b3ffe-142">versionInfo</span></span>|<span data-ttu-id="b3ffe-143">String</span><span class="sxs-lookup"><span data-stu-id="b3ffe-143">String</span></span>|<span data-ttu-id="b3ffe-144">模板的版本信息继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b3ffe-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="b3ffe-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="b3ffe-145">isDeprecated</span></span>|<span data-ttu-id="b3ffe-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3ffe-146">Boolean</span></span>|<span data-ttu-id="b3ffe-147">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-147">The template is deprecated or not.</span></span> <span data-ttu-id="b3ffe-148">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="b3ffe-149">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b3ffe-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="b3ffe-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="b3ffe-150">intentCount</span></span>|<span data-ttu-id="b3ffe-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b3ffe-151">Int32</span></span>|<span data-ttu-id="b3ffe-152">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-152">Number of Intents created from this template.</span></span> <span data-ttu-id="b3ffe-153">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b3ffe-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="b3ffe-154">templateType</span><span class="sxs-lookup"><span data-stu-id="b3ffe-154">templateType</span></span>|[<span data-ttu-id="b3ffe-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="b3ffe-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="b3ffe-156">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-156">The template's type.</span></span> <span data-ttu-id="b3ffe-157">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="b3ffe-158">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`、`deviceConfigurationForOffice365`。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span></span>|
|<span data-ttu-id="b3ffe-159">platformType</span><span class="sxs-lookup"><span data-stu-id="b3ffe-159">platformType</span></span>|[<span data-ttu-id="b3ffe-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="b3ffe-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="b3ffe-161">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-161">The template's platform.</span></span> <span data-ttu-id="b3ffe-162">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="b3ffe-163">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="b3ffe-164">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="b3ffe-164">templateSubtype</span></span>|[<span data-ttu-id="b3ffe-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="b3ffe-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="b3ffe-166">模板的子类型。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-166">The template's subtype.</span></span> <span data-ttu-id="b3ffe-167">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="b3ffe-168">可取值为：`none`、`firewall`、`diskEncryption`、`attackSurfaceReduction`、`endpointDetectionReponse`、`accountProtection` 或 `antivirus`。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span></span>|
|<span data-ttu-id="b3ffe-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3ffe-169">publishedDateTime</span></span>|<span data-ttu-id="b3ffe-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3ffe-170">DateTimeOffset</span></span>|<span data-ttu-id="b3ffe-171">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承发布模板时</span><span class="sxs-lookup"><span data-stu-id="b3ffe-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b3ffe-172">响应</span><span class="sxs-lookup"><span data-stu-id="b3ffe-172">Response</span></span>
<span data-ttu-id="b3ffe-173">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-173">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3ffe-174">示例</span><span class="sxs-lookup"><span data-stu-id="b3ffe-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3ffe-175">请求</span><span class="sxs-lookup"><span data-stu-id="b3ffe-175">Request</span></span>
<span data-ttu-id="b3ffe-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3ffe-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="b3ffe-177">响应</span><span class="sxs-lookup"><span data-stu-id="b3ffe-177">Response</span></span>
<span data-ttu-id="b3ffe-178">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b3ffe-178">Here is an example of the response.</span></span> <span data-ttu-id="b3ffe-179">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b3ffe-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b3ffe-180">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b3ffe-180">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



