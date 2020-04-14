---
title: 更新 securityBaselineTemplate
description: 更新 securityBaselineTemplate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d20b7f5b27f130393996573a27b9e00b42a2f0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427095"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="da62b-103">更新 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="da62b-103">Update securityBaselineTemplate</span></span>

<span data-ttu-id="da62b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da62b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da62b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da62b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da62b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da62b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da62b-107">更新[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da62b-107">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da62b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da62b-108">Prerequisites</span></span>
<span data-ttu-id="da62b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da62b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da62b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da62b-111">Permission type</span></span>|<span data-ttu-id="da62b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da62b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da62b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da62b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da62b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da62b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da62b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da62b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da62b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da62b-116">Not supported.</span></span>|
|<span data-ttu-id="da62b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da62b-117">Application</span></span>|<span data-ttu-id="da62b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da62b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da62b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da62b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="da62b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da62b-120">Request headers</span></span>
|<span data-ttu-id="da62b-121">标头</span><span class="sxs-lookup"><span data-stu-id="da62b-121">Header</span></span>|<span data-ttu-id="da62b-122">值</span><span class="sxs-lookup"><span data-stu-id="da62b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da62b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da62b-123">Authorization</span></span>|<span data-ttu-id="da62b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da62b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da62b-125">接受</span><span class="sxs-lookup"><span data-stu-id="da62b-125">Accept</span></span>|<span data-ttu-id="da62b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da62b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da62b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da62b-127">Request body</span></span>
<span data-ttu-id="da62b-128">在请求正文中，提供[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da62b-128">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="da62b-129">下表显示创建[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da62b-129">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="da62b-130">属性</span><span class="sxs-lookup"><span data-stu-id="da62b-130">Property</span></span>|<span data-ttu-id="da62b-131">类型</span><span class="sxs-lookup"><span data-stu-id="da62b-131">Type</span></span>|<span data-ttu-id="da62b-132">说明</span><span class="sxs-lookup"><span data-stu-id="da62b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da62b-133">id</span><span class="sxs-lookup"><span data-stu-id="da62b-133">id</span></span>|<span data-ttu-id="da62b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="da62b-134">String</span></span>|<span data-ttu-id="da62b-135">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID</span><span class="sxs-lookup"><span data-stu-id="da62b-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="da62b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="da62b-136">displayName</span></span>|<span data-ttu-id="da62b-137">String</span><span class="sxs-lookup"><span data-stu-id="da62b-137">String</span></span>|<span data-ttu-id="da62b-138">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="da62b-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="da62b-139">description</span><span class="sxs-lookup"><span data-stu-id="da62b-139">description</span></span>|<span data-ttu-id="da62b-140">String</span><span class="sxs-lookup"><span data-stu-id="da62b-140">String</span></span>|<span data-ttu-id="da62b-141">模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="da62b-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="da62b-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="da62b-142">versionInfo</span></span>|<span data-ttu-id="da62b-143">String</span><span class="sxs-lookup"><span data-stu-id="da62b-143">String</span></span>|<span data-ttu-id="da62b-144">模板的版本信息继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="da62b-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="da62b-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="da62b-145">isDeprecated</span></span>|<span data-ttu-id="da62b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="da62b-146">Boolean</span></span>|<span data-ttu-id="da62b-147">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="da62b-147">The template is deprecated or not.</span></span> <span data-ttu-id="da62b-148">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="da62b-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="da62b-149">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="da62b-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="da62b-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="da62b-150">intentCount</span></span>|<span data-ttu-id="da62b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="da62b-151">Int32</span></span>|<span data-ttu-id="da62b-152">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="da62b-152">Number of Intents created from this template.</span></span> <span data-ttu-id="da62b-153">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="da62b-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="da62b-154">templateType</span><span class="sxs-lookup"><span data-stu-id="da62b-154">templateType</span></span>|[<span data-ttu-id="da62b-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="da62b-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="da62b-156">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="da62b-156">The template's type.</span></span> <span data-ttu-id="da62b-157">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="da62b-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="da62b-158">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`。</span><span class="sxs-lookup"><span data-stu-id="da62b-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="da62b-159">platformType</span><span class="sxs-lookup"><span data-stu-id="da62b-159">platformType</span></span>|[<span data-ttu-id="da62b-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="da62b-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="da62b-161">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="da62b-161">The template's platform.</span></span> <span data-ttu-id="da62b-162">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="da62b-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="da62b-163">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="da62b-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="da62b-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="da62b-164">publishedDateTime</span></span>|<span data-ttu-id="da62b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da62b-165">DateTimeOffset</span></span>|<span data-ttu-id="da62b-166">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承发布模板时</span><span class="sxs-lookup"><span data-stu-id="da62b-166">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="da62b-167">响应</span><span class="sxs-lookup"><span data-stu-id="da62b-167">Response</span></span>
<span data-ttu-id="da62b-168">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da62b-168">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da62b-169">示例</span><span class="sxs-lookup"><span data-stu-id="da62b-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="da62b-170">请求</span><span class="sxs-lookup"><span data-stu-id="da62b-170">Request</span></span>
<span data-ttu-id="da62b-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da62b-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="da62b-172">响应</span><span class="sxs-lookup"><span data-stu-id="da62b-172">Response</span></span>
<span data-ttu-id="da62b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da62b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



