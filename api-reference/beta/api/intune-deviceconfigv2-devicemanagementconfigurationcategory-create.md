---
title: 创建 deviceManagementConfigurationCategory
description: 创建新的 deviceManagementConfigurationCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67a96b6d4d7ac90040a4a03573b85caaba3a96e7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301828"
---
# <a name="create-devicemanagementconfigurationcategory"></a><span data-ttu-id="7b3c7-103">创建 deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="7b3c7-103">Create deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="7b3c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b3c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b3c7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b3c7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b3c7-107">创建新的 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-107">Create a new [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b3c7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7b3c7-108">Prerequisites</span></span>
<span data-ttu-id="7b3c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b3c7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b3c7-111">Permission type</span></span>|<span data-ttu-id="7b3c7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7b3c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b3c7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b3c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b3c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b3c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b3c7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b3c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b3c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-116">Not supported.</span></span>|
|<span data-ttu-id="7b3c7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b3c7-117">Application</span></span>|<span data-ttu-id="7b3c7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b3c7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b3c7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b3c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationCategories
```

## <a name="request-headers"></a><span data-ttu-id="7b3c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b3c7-120">Request headers</span></span>
|<span data-ttu-id="7b3c7-121">标头</span><span class="sxs-lookup"><span data-stu-id="7b3c7-121">Header</span></span>|<span data-ttu-id="7b3c7-122">值</span><span class="sxs-lookup"><span data-stu-id="7b3c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b3c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b3c7-123">Authorization</span></span>|<span data-ttu-id="7b3c7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b3c7-125">接受</span><span class="sxs-lookup"><span data-stu-id="7b3c7-125">Accept</span></span>|<span data-ttu-id="7b3c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b3c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b3c7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b3c7-127">Request body</span></span>
<span data-ttu-id="7b3c7-128">在请求正文中，提供 deviceManagementConfigurationCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-128">In the request body, supply a JSON representation for the deviceManagementConfigurationCategory object.</span></span>

<span data-ttu-id="7b3c7-129">下表显示创建 deviceManagementConfigurationCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-129">The following table shows the properties that are required when you create the deviceManagementConfigurationCategory.</span></span>

|<span data-ttu-id="7b3c7-130">属性</span><span class="sxs-lookup"><span data-stu-id="7b3c7-130">Property</span></span>|<span data-ttu-id="7b3c7-131">类型</span><span class="sxs-lookup"><span data-stu-id="7b3c7-131">Type</span></span>|<span data-ttu-id="7b3c7-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b3c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b3c7-133">id</span><span class="sxs-lookup"><span data-stu-id="7b3c7-133">id</span></span>|<span data-ttu-id="7b3c7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7b3c7-134">String</span></span>|<span data-ttu-id="7b3c7-135">项的标识符</span><span class="sxs-lookup"><span data-stu-id="7b3c7-135">Identifier for item</span></span>|
|<span data-ttu-id="7b3c7-136">description</span><span class="sxs-lookup"><span data-stu-id="7b3c7-136">description</span></span>|<span data-ttu-id="7b3c7-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7b3c7-137">String</span></span>|<span data-ttu-id="7b3c7-138">项目的说明</span><span class="sxs-lookup"><span data-stu-id="7b3c7-138">Description of the item</span></span>|
|<span data-ttu-id="7b3c7-139">helpText</span><span class="sxs-lookup"><span data-stu-id="7b3c7-139">helpText</span></span>|<span data-ttu-id="7b3c7-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7b3c7-140">String</span></span>|<span data-ttu-id="7b3c7-141">项目的帮助文本</span><span class="sxs-lookup"><span data-stu-id="7b3c7-141">Help text of the item</span></span>|
|<span data-ttu-id="7b3c7-142">name</span><span class="sxs-lookup"><span data-stu-id="7b3c7-142">name</span></span>|<span data-ttu-id="7b3c7-143">字符串</span><span class="sxs-lookup"><span data-stu-id="7b3c7-143">String</span></span>|<span data-ttu-id="7b3c7-144">项目的名称</span><span class="sxs-lookup"><span data-stu-id="7b3c7-144">Name of the item</span></span>|
|<span data-ttu-id="7b3c7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7b3c7-145">displayName</span></span>|<span data-ttu-id="7b3c7-146">字符串</span><span class="sxs-lookup"><span data-stu-id="7b3c7-146">String</span></span>|<span data-ttu-id="7b3c7-147">项目的显示名称</span><span class="sxs-lookup"><span data-stu-id="7b3c7-147">Display name of the item</span></span>|
|<span data-ttu-id="7b3c7-148">平台</span><span class="sxs-lookup"><span data-stu-id="7b3c7-148">platforms</span></span>|[<span data-ttu-id="7b3c7-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="7b3c7-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="7b3c7-150">平台类型，类别中的设置具有。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="7b3c7-151">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="7b3c7-152">技术</span><span class="sxs-lookup"><span data-stu-id="7b3c7-152">technologies</span></span>|[<span data-ttu-id="7b3c7-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="7b3c7-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="7b3c7-154">技术类型，类别中的设置具有。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="7b3c7-155">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|



## <a name="response"></a><span data-ttu-id="7b3c7-156">响应</span><span class="sxs-lookup"><span data-stu-id="7b3c7-156">Response</span></span>
<span data-ttu-id="7b3c7-157">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-157">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b3c7-158">示例</span><span class="sxs-lookup"><span data-stu-id="7b3c7-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b3c7-159">请求</span><span class="sxs-lookup"><span data-stu-id="7b3c7-159">Request</span></span>
<span data-ttu-id="7b3c7-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationCategories
Content-type: application/json
Content-length: 268

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm"
}
```

### <a name="response"></a><span data-ttu-id="7b3c7-161">响应</span><span class="sxs-lookup"><span data-stu-id="7b3c7-161">Response</span></span>
<span data-ttu-id="7b3c7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7b3c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm"
}
```




