---
title: 创建 deviceManagementTemplate
description: 创建新的 deviceManagementTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01f3c719e0f5ad2b77c48f223dd198aa7b92e96b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381436"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="273d6-103">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="273d6-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="273d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="273d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="273d6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="273d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="273d6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="273d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="273d6-107">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="273d6-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="273d6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="273d6-108">Prerequisites</span></span>
<span data-ttu-id="273d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="273d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="273d6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="273d6-111">Permission type</span></span>|<span data-ttu-id="273d6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="273d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="273d6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="273d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="273d6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="273d6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="273d6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="273d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="273d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="273d6-116">Not supported.</span></span>|
|<span data-ttu-id="273d6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="273d6-117">Application</span></span>|<span data-ttu-id="273d6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="273d6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="273d6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="273d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="273d6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="273d6-120">Request headers</span></span>
|<span data-ttu-id="273d6-121">标头</span><span class="sxs-lookup"><span data-stu-id="273d6-121">Header</span></span>|<span data-ttu-id="273d6-122">值</span><span class="sxs-lookup"><span data-stu-id="273d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="273d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="273d6-123">Authorization</span></span>|<span data-ttu-id="273d6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="273d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="273d6-125">接受</span><span class="sxs-lookup"><span data-stu-id="273d6-125">Accept</span></span>|<span data-ttu-id="273d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="273d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="273d6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="273d6-127">Request body</span></span>
<span data-ttu-id="273d6-128">在请求正文中，提供 deviceManagementTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="273d6-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="273d6-129">下表显示创建 deviceManagementTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="273d6-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="273d6-130">属性</span><span class="sxs-lookup"><span data-stu-id="273d6-130">Property</span></span>|<span data-ttu-id="273d6-131">类型</span><span class="sxs-lookup"><span data-stu-id="273d6-131">Type</span></span>|<span data-ttu-id="273d6-132">说明</span><span class="sxs-lookup"><span data-stu-id="273d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="273d6-133">id</span><span class="sxs-lookup"><span data-stu-id="273d6-133">id</span></span>|<span data-ttu-id="273d6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="273d6-134">String</span></span>|<span data-ttu-id="273d6-135">模板 ID</span><span class="sxs-lookup"><span data-stu-id="273d6-135">The template ID</span></span>|
|<span data-ttu-id="273d6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="273d6-136">displayName</span></span>|<span data-ttu-id="273d6-137">String</span><span class="sxs-lookup"><span data-stu-id="273d6-137">String</span></span>|<span data-ttu-id="273d6-138">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="273d6-138">The template's display name</span></span>|
|<span data-ttu-id="273d6-139">description</span><span class="sxs-lookup"><span data-stu-id="273d6-139">description</span></span>|<span data-ttu-id="273d6-140">String</span><span class="sxs-lookup"><span data-stu-id="273d6-140">String</span></span>|<span data-ttu-id="273d6-141">模板的说明</span><span class="sxs-lookup"><span data-stu-id="273d6-141">The template's description</span></span>|
|<span data-ttu-id="273d6-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="273d6-142">versionInfo</span></span>|<span data-ttu-id="273d6-143">字符串</span><span class="sxs-lookup"><span data-stu-id="273d6-143">String</span></span>|<span data-ttu-id="273d6-144">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="273d6-144">The template's version information</span></span>|
|<span data-ttu-id="273d6-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="273d6-145">isDeprecated</span></span>|<span data-ttu-id="273d6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="273d6-146">Boolean</span></span>|<span data-ttu-id="273d6-147">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="273d6-147">The template is deprecated or not.</span></span> <span data-ttu-id="273d6-148">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="273d6-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="273d6-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="273d6-149">intentCount</span></span>|<span data-ttu-id="273d6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="273d6-150">Int32</span></span>|<span data-ttu-id="273d6-151">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="273d6-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="273d6-152">templateType</span><span class="sxs-lookup"><span data-stu-id="273d6-152">templateType</span></span>|[<span data-ttu-id="273d6-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="273d6-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="273d6-154">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="273d6-154">The template's type.</span></span> <span data-ttu-id="273d6-155">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`。</span><span class="sxs-lookup"><span data-stu-id="273d6-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="273d6-156">platformType</span><span class="sxs-lookup"><span data-stu-id="273d6-156">platformType</span></span>|[<span data-ttu-id="273d6-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="273d6-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="273d6-158">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="273d6-158">The template's platform.</span></span> <span data-ttu-id="273d6-159">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="273d6-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="273d6-160">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="273d6-160">publishedDateTime</span></span>|<span data-ttu-id="273d6-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="273d6-161">DateTimeOffset</span></span>|<span data-ttu-id="273d6-162">发布模板时</span><span class="sxs-lookup"><span data-stu-id="273d6-162">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="273d6-163">响应</span><span class="sxs-lookup"><span data-stu-id="273d6-163">Response</span></span>
<span data-ttu-id="273d6-164">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="273d6-164">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="273d6-165">示例</span><span class="sxs-lookup"><span data-stu-id="273d6-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="273d6-166">请求</span><span class="sxs-lookup"><span data-stu-id="273d6-166">Request</span></span>
<span data-ttu-id="273d6-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="273d6-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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

### <a name="response"></a><span data-ttu-id="273d6-168">响应</span><span class="sxs-lookup"><span data-stu-id="273d6-168">Response</span></span>
<span data-ttu-id="273d6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="273d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 420

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
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```



