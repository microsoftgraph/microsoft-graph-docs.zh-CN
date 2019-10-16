---
title: 更新 deviceManagementTemplate
description: 更新 deviceManagementTemplate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f05999d160b2fd947f4c44f3130c95aa34756e07
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532055"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="3c910-103">更新 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="3c910-103">Update deviceManagementTemplate</span></span>

> <span data-ttu-id="3c910-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c910-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c910-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c910-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c910-106">更新[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c910-106">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c910-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c910-107">Prerequisites</span></span>
<span data-ttu-id="3c910-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c910-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c910-110">Permission type</span></span>|<span data-ttu-id="3c910-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c910-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c910-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c910-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c910-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c910-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c910-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c910-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c910-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c910-115">Not supported.</span></span>|
|<span data-ttu-id="3c910-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c910-116">Application</span></span>|<span data-ttu-id="3c910-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c910-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c910-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c910-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="3c910-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c910-119">Request headers</span></span>
|<span data-ttu-id="3c910-120">标头</span><span class="sxs-lookup"><span data-stu-id="3c910-120">Header</span></span>|<span data-ttu-id="3c910-121">值</span><span class="sxs-lookup"><span data-stu-id="3c910-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c910-122">授权</span><span class="sxs-lookup"><span data-stu-id="3c910-122">Authorization</span></span>|<span data-ttu-id="3c910-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c910-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c910-124">接受</span><span class="sxs-lookup"><span data-stu-id="3c910-124">Accept</span></span>|<span data-ttu-id="3c910-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c910-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c910-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c910-126">Request body</span></span>
<span data-ttu-id="3c910-127">在请求正文中，提供[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c910-127">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="3c910-128">下表显示创建[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c910-128">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="3c910-129">属性</span><span class="sxs-lookup"><span data-stu-id="3c910-129">Property</span></span>|<span data-ttu-id="3c910-130">类型</span><span class="sxs-lookup"><span data-stu-id="3c910-130">Type</span></span>|<span data-ttu-id="3c910-131">说明</span><span class="sxs-lookup"><span data-stu-id="3c910-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c910-132">id</span><span class="sxs-lookup"><span data-stu-id="3c910-132">id</span></span>|<span data-ttu-id="3c910-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3c910-133">String</span></span>|<span data-ttu-id="3c910-134">模板 ID</span><span class="sxs-lookup"><span data-stu-id="3c910-134">The template ID</span></span>|
|<span data-ttu-id="3c910-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3c910-135">displayName</span></span>|<span data-ttu-id="3c910-136">String</span><span class="sxs-lookup"><span data-stu-id="3c910-136">String</span></span>|<span data-ttu-id="3c910-137">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="3c910-137">The template's display name</span></span>|
|<span data-ttu-id="3c910-138">说明</span><span class="sxs-lookup"><span data-stu-id="3c910-138">description</span></span>|<span data-ttu-id="3c910-139">String</span><span class="sxs-lookup"><span data-stu-id="3c910-139">String</span></span>|<span data-ttu-id="3c910-140">模板的说明</span><span class="sxs-lookup"><span data-stu-id="3c910-140">The template's description</span></span>|
|<span data-ttu-id="3c910-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="3c910-141">versionInfo</span></span>|<span data-ttu-id="3c910-142">字符串</span><span class="sxs-lookup"><span data-stu-id="3c910-142">String</span></span>|<span data-ttu-id="3c910-143">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="3c910-143">The template's version information</span></span>|
|<span data-ttu-id="3c910-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="3c910-144">isDeprecated</span></span>|<span data-ttu-id="3c910-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c910-145">Boolean</span></span>|<span data-ttu-id="3c910-146">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="3c910-146">The template is deprecated or not.</span></span> <span data-ttu-id="3c910-147">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="3c910-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="3c910-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="3c910-148">intentCount</span></span>|<span data-ttu-id="3c910-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3c910-149">Int32</span></span>|<span data-ttu-id="3c910-150">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="3c910-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="3c910-151">templateType</span><span class="sxs-lookup"><span data-stu-id="3c910-151">templateType</span></span>|[<span data-ttu-id="3c910-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="3c910-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="3c910-153">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="3c910-153">The template's type.</span></span> <span data-ttu-id="3c910-154">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`。</span><span class="sxs-lookup"><span data-stu-id="3c910-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span></span>|
|<span data-ttu-id="3c910-155">platformType</span><span class="sxs-lookup"><span data-stu-id="3c910-155">platformType</span></span>|[<span data-ttu-id="3c910-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="3c910-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="3c910-157">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="3c910-157">The template's platform.</span></span> <span data-ttu-id="3c910-158">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="3c910-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="3c910-159">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c910-159">publishedDateTime</span></span>|<span data-ttu-id="3c910-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c910-160">DateTimeOffset</span></span>|<span data-ttu-id="3c910-161">发布模板时</span><span class="sxs-lookup"><span data-stu-id="3c910-161">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="3c910-162">响应</span><span class="sxs-lookup"><span data-stu-id="3c910-162">Response</span></span>
<span data-ttu-id="3c910-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c910-163">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c910-164">示例</span><span class="sxs-lookup"><span data-stu-id="3c910-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c910-165">请求</span><span class="sxs-lookup"><span data-stu-id="3c910-165">Request</span></span>
<span data-ttu-id="3c910-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c910-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="3c910-167">响应</span><span class="sxs-lookup"><span data-stu-id="3c910-167">Response</span></span>
<span data-ttu-id="3c910-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c910-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






