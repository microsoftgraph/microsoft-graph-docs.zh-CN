---
title: 创建 deviceManagementTemplate
description: 创建新的 deviceManagementTemplate 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 102fa662dd9cf6eef9a4949f8dc9250e69cfadbf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915984"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="a2348-103">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2348-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="a2348-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2348-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2348-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2348-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2348-106">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2348-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2348-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2348-107">Prerequisites</span></span>
<span data-ttu-id="a2348-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2348-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2348-110">Permission type</span></span>|<span data-ttu-id="a2348-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2348-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2348-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2348-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2348-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2348-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2348-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2348-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2348-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2348-115">Not supported.</span></span>|
|<span data-ttu-id="a2348-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2348-116">Application</span></span>|<span data-ttu-id="a2348-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2348-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2348-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2348-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="a2348-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2348-119">Request headers</span></span>
|<span data-ttu-id="a2348-120">标头</span><span class="sxs-lookup"><span data-stu-id="a2348-120">Header</span></span>|<span data-ttu-id="a2348-121">值</span><span class="sxs-lookup"><span data-stu-id="a2348-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2348-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2348-122">Authorization</span></span>|<span data-ttu-id="a2348-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2348-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2348-124">接受</span><span class="sxs-lookup"><span data-stu-id="a2348-124">Accept</span></span>|<span data-ttu-id="a2348-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2348-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2348-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2348-126">Request body</span></span>
<span data-ttu-id="a2348-127">在请求正文中, 提供 deviceManagementTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2348-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="a2348-128">下表显示创建 deviceManagementTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2348-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="a2348-129">属性</span><span class="sxs-lookup"><span data-stu-id="a2348-129">Property</span></span>|<span data-ttu-id="a2348-130">类型</span><span class="sxs-lookup"><span data-stu-id="a2348-130">Type</span></span>|<span data-ttu-id="a2348-131">说明</span><span class="sxs-lookup"><span data-stu-id="a2348-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2348-132">id</span><span class="sxs-lookup"><span data-stu-id="a2348-132">id</span></span>|<span data-ttu-id="a2348-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a2348-133">String</span></span>|<span data-ttu-id="a2348-134">模板 ID</span><span class="sxs-lookup"><span data-stu-id="a2348-134">The template ID</span></span>|
|<span data-ttu-id="a2348-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a2348-135">displayName</span></span>|<span data-ttu-id="a2348-136">String</span><span class="sxs-lookup"><span data-stu-id="a2348-136">String</span></span>|<span data-ttu-id="a2348-137">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="a2348-137">The template's display name</span></span>|
|<span data-ttu-id="a2348-138">说明</span><span class="sxs-lookup"><span data-stu-id="a2348-138">description</span></span>|<span data-ttu-id="a2348-139">String</span><span class="sxs-lookup"><span data-stu-id="a2348-139">String</span></span>|<span data-ttu-id="a2348-140">模板的说明</span><span class="sxs-lookup"><span data-stu-id="a2348-140">The template's description</span></span>|
|<span data-ttu-id="a2348-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="a2348-141">versionInfo</span></span>|<span data-ttu-id="a2348-142">String</span><span class="sxs-lookup"><span data-stu-id="a2348-142">String</span></span>|<span data-ttu-id="a2348-143">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="a2348-143">The template's version information</span></span>|
|<span data-ttu-id="a2348-144">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="a2348-144">isDeprecated</span></span>|<span data-ttu-id="a2348-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2348-145">Boolean</span></span>|<span data-ttu-id="a2348-146">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="a2348-146">The template is deprecated or not.</span></span> <span data-ttu-id="a2348-147">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="a2348-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="a2348-148">intentCount</span><span class="sxs-lookup"><span data-stu-id="a2348-148">intentCount</span></span>|<span data-ttu-id="a2348-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a2348-149">Int32</span></span>|<span data-ttu-id="a2348-150">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="a2348-150">Number of Intents created from this template.</span></span>|



## <a name="response"></a><span data-ttu-id="a2348-151">响应</span><span class="sxs-lookup"><span data-stu-id="a2348-151">Response</span></span>
<span data-ttu-id="a2348-152">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2348-152">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2348-153">示例</span><span class="sxs-lookup"><span data-stu-id="a2348-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2348-154">请求</span><span class="sxs-lookup"><span data-stu-id="a2348-154">Request</span></span>
<span data-ttu-id="a2348-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2348-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```

### <a name="response"></a><span data-ttu-id="a2348-156">响应</span><span class="sxs-lookup"><span data-stu-id="a2348-156">Response</span></span>
<span data-ttu-id="a2348-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2348-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11
}
```




