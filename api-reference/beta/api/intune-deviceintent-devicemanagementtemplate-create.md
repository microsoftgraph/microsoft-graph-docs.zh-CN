---
title: 创建 deviceManagementTemplate
description: 创建新的 deviceManagementTemplate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8df263e974037e747eb65169f6d305cef2b7b3b5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343130"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="eb35c-103">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="eb35c-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="eb35c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb35c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb35c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb35c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb35c-106">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eb35c-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb35c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb35c-107">Prerequisites</span></span>
<span data-ttu-id="eb35c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb35c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb35c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb35c-110">Permission type</span></span>|<span data-ttu-id="eb35c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb35c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb35c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb35c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb35c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb35c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb35c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb35c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb35c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb35c-115">Not supported.</span></span>|
|<span data-ttu-id="eb35c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb35c-116">Application</span></span>|<span data-ttu-id="eb35c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb35c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb35c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb35c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="eb35c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb35c-119">Request headers</span></span>
|<span data-ttu-id="eb35c-120">标头</span><span class="sxs-lookup"><span data-stu-id="eb35c-120">Header</span></span>|<span data-ttu-id="eb35c-121">值</span><span class="sxs-lookup"><span data-stu-id="eb35c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb35c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb35c-122">Authorization</span></span>|<span data-ttu-id="eb35c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb35c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb35c-124">接受</span><span class="sxs-lookup"><span data-stu-id="eb35c-124">Accept</span></span>|<span data-ttu-id="eb35c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb35c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb35c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb35c-126">Request body</span></span>
<span data-ttu-id="eb35c-127">在请求正文中, 提供 deviceManagementTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb35c-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="eb35c-128">下表显示创建 deviceManagementTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb35c-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="eb35c-129">属性</span><span class="sxs-lookup"><span data-stu-id="eb35c-129">Property</span></span>|<span data-ttu-id="eb35c-130">类型</span><span class="sxs-lookup"><span data-stu-id="eb35c-130">Type</span></span>|<span data-ttu-id="eb35c-131">说明</span><span class="sxs-lookup"><span data-stu-id="eb35c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb35c-132">id</span><span class="sxs-lookup"><span data-stu-id="eb35c-132">id</span></span>|<span data-ttu-id="eb35c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="eb35c-133">String</span></span>|<span data-ttu-id="eb35c-134">模板 ID</span><span class="sxs-lookup"><span data-stu-id="eb35c-134">The template ID</span></span>|
|<span data-ttu-id="eb35c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="eb35c-135">displayName</span></span>|<span data-ttu-id="eb35c-136">String</span><span class="sxs-lookup"><span data-stu-id="eb35c-136">String</span></span>|<span data-ttu-id="eb35c-137">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="eb35c-137">The template's display name</span></span>|
|<span data-ttu-id="eb35c-138">说明</span><span class="sxs-lookup"><span data-stu-id="eb35c-138">description</span></span>|<span data-ttu-id="eb35c-139">String</span><span class="sxs-lookup"><span data-stu-id="eb35c-139">String</span></span>|<span data-ttu-id="eb35c-140">模板的说明</span><span class="sxs-lookup"><span data-stu-id="eb35c-140">The template's description</span></span>|
|<span data-ttu-id="eb35c-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="eb35c-141">versionInfo</span></span>|<span data-ttu-id="eb35c-142">String</span><span class="sxs-lookup"><span data-stu-id="eb35c-142">String</span></span>|<span data-ttu-id="eb35c-143">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="eb35c-143">The template's version information</span></span>|
|<span data-ttu-id="eb35c-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="eb35c-144">isDeprecated</span></span>|<span data-ttu-id="eb35c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb35c-145">Boolean</span></span>|<span data-ttu-id="eb35c-146">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="eb35c-146">The template is deprecated or not.</span></span> <span data-ttu-id="eb35c-147">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="eb35c-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="eb35c-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="eb35c-148">intentCount</span></span>|<span data-ttu-id="eb35c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="eb35c-149">Int32</span></span>|<span data-ttu-id="eb35c-150">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="eb35c-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="eb35c-151">templateType</span><span class="sxs-lookup"><span data-stu-id="eb35c-151">templateType</span></span>|[<span data-ttu-id="eb35c-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="eb35c-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="eb35c-153">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="eb35c-153">The template's type.</span></span> <span data-ttu-id="eb35c-154">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="eb35c-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="eb35c-155">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb35c-155">publishedDateTime</span></span>|<span data-ttu-id="eb35c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb35c-156">DateTimeOffset</span></span>|<span data-ttu-id="eb35c-157">发布模板时</span><span class="sxs-lookup"><span data-stu-id="eb35c-157">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="eb35c-158">响应</span><span class="sxs-lookup"><span data-stu-id="eb35c-158">Response</span></span>
<span data-ttu-id="eb35c-159">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eb35c-159">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb35c-160">示例</span><span class="sxs-lookup"><span data-stu-id="eb35c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb35c-161">请求</span><span class="sxs-lookup"><span data-stu-id="eb35c-161">Request</span></span>
<span data-ttu-id="eb35c-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb35c-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="eb35c-163">响应</span><span class="sxs-lookup"><span data-stu-id="eb35c-163">Response</span></span>
<span data-ttu-id="eb35c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb35c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```






