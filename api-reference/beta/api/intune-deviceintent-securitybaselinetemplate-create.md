---
title: 创建 securityBaselineTemplate
description: 创建新的 securityBaselineTemplate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ecf477b0ad24232cd9a42e7e1070dcf266d6d14
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945338"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="0f83c-103">创建 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="0f83c-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="0f83c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f83c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f83c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f83c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f83c-106">创建新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f83c-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f83c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f83c-107">Prerequisites</span></span>
<span data-ttu-id="0f83c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f83c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f83c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f83c-110">Permission type</span></span>|<span data-ttu-id="0f83c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f83c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f83c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f83c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f83c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f83c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f83c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f83c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f83c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f83c-115">Not supported.</span></span>|
|<span data-ttu-id="0f83c-116">Application</span><span class="sxs-lookup"><span data-stu-id="0f83c-116">Application</span></span>|<span data-ttu-id="0f83c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f83c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f83c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f83c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="0f83c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f83c-119">Request headers</span></span>
|<span data-ttu-id="0f83c-120">标头</span><span class="sxs-lookup"><span data-stu-id="0f83c-120">Header</span></span>|<span data-ttu-id="0f83c-121">值</span><span class="sxs-lookup"><span data-stu-id="0f83c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f83c-122">授权</span><span class="sxs-lookup"><span data-stu-id="0f83c-122">Authorization</span></span>|<span data-ttu-id="0f83c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f83c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f83c-124">接受</span><span class="sxs-lookup"><span data-stu-id="0f83c-124">Accept</span></span>|<span data-ttu-id="0f83c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f83c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f83c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f83c-126">Request body</span></span>
<span data-ttu-id="0f83c-127">在请求正文中，提供 securityBaselineTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f83c-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="0f83c-128">下表显示创建 securityBaselineTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0f83c-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="0f83c-129">属性</span><span class="sxs-lookup"><span data-stu-id="0f83c-129">Property</span></span>|<span data-ttu-id="0f83c-130">类型</span><span class="sxs-lookup"><span data-stu-id="0f83c-130">Type</span></span>|<span data-ttu-id="0f83c-131">说明</span><span class="sxs-lookup"><span data-stu-id="0f83c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f83c-132">id</span><span class="sxs-lookup"><span data-stu-id="0f83c-132">id</span></span>|<span data-ttu-id="0f83c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0f83c-133">String</span></span>|<span data-ttu-id="0f83c-134">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID</span><span class="sxs-lookup"><span data-stu-id="0f83c-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="0f83c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0f83c-135">displayName</span></span>|<span data-ttu-id="0f83c-136">String</span><span class="sxs-lookup"><span data-stu-id="0f83c-136">String</span></span>|<span data-ttu-id="0f83c-137">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="0f83c-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="0f83c-138">说明</span><span class="sxs-lookup"><span data-stu-id="0f83c-138">description</span></span>|<span data-ttu-id="0f83c-139">String</span><span class="sxs-lookup"><span data-stu-id="0f83c-139">String</span></span>|<span data-ttu-id="0f83c-140">模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0f83c-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="0f83c-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="0f83c-141">versionInfo</span></span>|<span data-ttu-id="0f83c-142">字符串</span><span class="sxs-lookup"><span data-stu-id="0f83c-142">String</span></span>|<span data-ttu-id="0f83c-143">模板的版本信息继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0f83c-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="0f83c-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="0f83c-144">isDeprecated</span></span>|<span data-ttu-id="0f83c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f83c-145">Boolean</span></span>|<span data-ttu-id="0f83c-146">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="0f83c-146">The template is deprecated or not.</span></span> <span data-ttu-id="0f83c-147">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="0f83c-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="0f83c-148">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0f83c-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="0f83c-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="0f83c-149">intentCount</span></span>|<span data-ttu-id="0f83c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0f83c-150">Int32</span></span>|<span data-ttu-id="0f83c-151">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="0f83c-151">Number of Intents created from this template.</span></span> <span data-ttu-id="0f83c-152">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="0f83c-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="0f83c-153">templateType</span><span class="sxs-lookup"><span data-stu-id="0f83c-153">templateType</span></span>|[<span data-ttu-id="0f83c-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="0f83c-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="0f83c-155">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="0f83c-155">The template's type.</span></span> <span data-ttu-id="0f83c-156">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="0f83c-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="0f83c-157">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`。</span><span class="sxs-lookup"><span data-stu-id="0f83c-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span></span>|
|<span data-ttu-id="0f83c-158">platformType</span><span class="sxs-lookup"><span data-stu-id="0f83c-158">platformType</span></span>|[<span data-ttu-id="0f83c-159">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="0f83c-159">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="0f83c-160">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="0f83c-160">The template's platform.</span></span> <span data-ttu-id="0f83c-161">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="0f83c-161">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="0f83c-162">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="0f83c-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="0f83c-163">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f83c-163">publishedDateTime</span></span>|<span data-ttu-id="0f83c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f83c-164">DateTimeOffset</span></span>|<span data-ttu-id="0f83c-165">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承发布模板时</span><span class="sxs-lookup"><span data-stu-id="0f83c-165">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0f83c-166">响应</span><span class="sxs-lookup"><span data-stu-id="0f83c-166">Response</span></span>
<span data-ttu-id="0f83c-167">如果成功，此方法在响应`201 Created`正文中返回响应代码和[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f83c-167">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f83c-168">示例</span><span class="sxs-lookup"><span data-stu-id="0f83c-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f83c-169">请求</span><span class="sxs-lookup"><span data-stu-id="0f83c-169">Request</span></span>
<span data-ttu-id="0f83c-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f83c-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="0f83c-171">响应</span><span class="sxs-lookup"><span data-stu-id="0f83c-171">Response</span></span>
<span data-ttu-id="0f83c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f83c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 420

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
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





