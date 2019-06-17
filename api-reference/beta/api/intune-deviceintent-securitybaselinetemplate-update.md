---
title: 更新 securityBaselineTemplate
description: 更新 securityBaselineTemplate 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f31343da2c7a5be98de891f289eeba044a31ed5b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959409"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="497cb-103">更新 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="497cb-103">Update securityBaselineTemplate</span></span>

> <span data-ttu-id="497cb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="497cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="497cb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="497cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="497cb-106">更新[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="497cb-106">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="497cb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="497cb-107">Prerequisites</span></span>
<span data-ttu-id="497cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="497cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="497cb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="497cb-110">Permission type</span></span>|<span data-ttu-id="497cb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="497cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="497cb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="497cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="497cb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497cb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="497cb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="497cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="497cb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="497cb-115">Not supported.</span></span>|
|<span data-ttu-id="497cb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="497cb-116">Application</span></span>|<span data-ttu-id="497cb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="497cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="497cb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="497cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="497cb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="497cb-119">Request headers</span></span>
|<span data-ttu-id="497cb-120">标头</span><span class="sxs-lookup"><span data-stu-id="497cb-120">Header</span></span>|<span data-ttu-id="497cb-121">值</span><span class="sxs-lookup"><span data-stu-id="497cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="497cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="497cb-122">Authorization</span></span>|<span data-ttu-id="497cb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="497cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="497cb-124">接受</span><span class="sxs-lookup"><span data-stu-id="497cb-124">Accept</span></span>|<span data-ttu-id="497cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="497cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="497cb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="497cb-126">Request body</span></span>
<span data-ttu-id="497cb-127">在请求正文中, 提供[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="497cb-127">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="497cb-128">下表显示创建[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="497cb-128">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="497cb-129">属性</span><span class="sxs-lookup"><span data-stu-id="497cb-129">Property</span></span>|<span data-ttu-id="497cb-130">类型</span><span class="sxs-lookup"><span data-stu-id="497cb-130">Type</span></span>|<span data-ttu-id="497cb-131">说明</span><span class="sxs-lookup"><span data-stu-id="497cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="497cb-132">id</span><span class="sxs-lookup"><span data-stu-id="497cb-132">id</span></span>|<span data-ttu-id="497cb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="497cb-133">String</span></span>|<span data-ttu-id="497cb-134">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID</span><span class="sxs-lookup"><span data-stu-id="497cb-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="497cb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="497cb-135">displayName</span></span>|<span data-ttu-id="497cb-136">String</span><span class="sxs-lookup"><span data-stu-id="497cb-136">String</span></span>|<span data-ttu-id="497cb-137">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="497cb-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="497cb-138">说明</span><span class="sxs-lookup"><span data-stu-id="497cb-138">description</span></span>|<span data-ttu-id="497cb-139">String</span><span class="sxs-lookup"><span data-stu-id="497cb-139">String</span></span>|<span data-ttu-id="497cb-140">模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="497cb-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="497cb-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="497cb-141">versionInfo</span></span>|<span data-ttu-id="497cb-142">String</span><span class="sxs-lookup"><span data-stu-id="497cb-142">String</span></span>|<span data-ttu-id="497cb-143">模板的版本信息继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="497cb-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="497cb-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="497cb-144">isDeprecated</span></span>|<span data-ttu-id="497cb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="497cb-145">Boolean</span></span>|<span data-ttu-id="497cb-146">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="497cb-146">The template is deprecated or not.</span></span> <span data-ttu-id="497cb-147">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="497cb-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="497cb-148">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="497cb-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="497cb-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="497cb-149">intentCount</span></span>|<span data-ttu-id="497cb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="497cb-150">Int32</span></span>|<span data-ttu-id="497cb-151">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="497cb-151">Number of Intents created from this template.</span></span> <span data-ttu-id="497cb-152">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="497cb-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="497cb-153">templateType</span><span class="sxs-lookup"><span data-stu-id="497cb-153">templateType</span></span>|[<span data-ttu-id="497cb-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="497cb-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="497cb-155">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="497cb-155">The template's type.</span></span> <span data-ttu-id="497cb-156">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="497cb-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="497cb-157">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="497cb-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="497cb-158">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="497cb-158">publishedDateTime</span></span>|<span data-ttu-id="497cb-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="497cb-159">DateTimeOffset</span></span>|<span data-ttu-id="497cb-160">从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承发布模板时</span><span class="sxs-lookup"><span data-stu-id="497cb-160">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="497cb-161">响应</span><span class="sxs-lookup"><span data-stu-id="497cb-161">Response</span></span>
<span data-ttu-id="497cb-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="497cb-162">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="497cb-163">示例</span><span class="sxs-lookup"><span data-stu-id="497cb-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="497cb-164">请求</span><span class="sxs-lookup"><span data-stu-id="497cb-164">Request</span></span>
<span data-ttu-id="497cb-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="497cb-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="497cb-166">响应</span><span class="sxs-lookup"><span data-stu-id="497cb-166">Response</span></span>
<span data-ttu-id="497cb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="497cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





