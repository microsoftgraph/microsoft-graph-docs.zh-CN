---
title: 更新 deviceManagementConfigurationCategory
description: 更新 deviceManagementConfigurationCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b34323a883b24f9849f4b5d140f0dc0dc5faa08
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866270"
---
# <a name="update-devicemanagementconfigurationcategory"></a><span data-ttu-id="cdcff-103">更新 deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="cdcff-103">Update deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="cdcff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdcff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdcff-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cdcff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdcff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdcff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdcff-107">更新 [deviceManagementConfigurationCategory 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="cdcff-107">Update the properties of a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdcff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cdcff-108">Prerequisites</span></span>
<span data-ttu-id="cdcff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdcff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdcff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdcff-111">Permission type</span></span>|<span data-ttu-id="cdcff-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdcff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdcff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdcff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdcff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdcff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdcff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdcff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdcff-116">Not supported.</span></span>|
|<span data-ttu-id="cdcff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdcff-117">Application</span></span>|<span data-ttu-id="cdcff-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcff-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdcff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdcff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="cdcff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdcff-120">Request headers</span></span>
|<span data-ttu-id="cdcff-121">标头</span><span class="sxs-lookup"><span data-stu-id="cdcff-121">Header</span></span>|<span data-ttu-id="cdcff-122">值</span><span class="sxs-lookup"><span data-stu-id="cdcff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdcff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdcff-123">Authorization</span></span>|<span data-ttu-id="cdcff-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cdcff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdcff-125">接受</span><span class="sxs-lookup"><span data-stu-id="cdcff-125">Accept</span></span>|<span data-ttu-id="cdcff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdcff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdcff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdcff-127">Request body</span></span>
<span data-ttu-id="cdcff-128">在请求正文中，提供 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdcff-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

<span data-ttu-id="cdcff-129">下表显示创建 [deviceManagementConfigurationCategory 时所需的属性](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="cdcff-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span></span>

|<span data-ttu-id="cdcff-130">属性</span><span class="sxs-lookup"><span data-stu-id="cdcff-130">Property</span></span>|<span data-ttu-id="cdcff-131">类型</span><span class="sxs-lookup"><span data-stu-id="cdcff-131">Type</span></span>|<span data-ttu-id="cdcff-132">说明</span><span class="sxs-lookup"><span data-stu-id="cdcff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdcff-133">id</span><span class="sxs-lookup"><span data-stu-id="cdcff-133">id</span></span>|<span data-ttu-id="cdcff-134">String</span><span class="sxs-lookup"><span data-stu-id="cdcff-134">String</span></span>|<span data-ttu-id="cdcff-135">项的标识符</span><span class="sxs-lookup"><span data-stu-id="cdcff-135">Identifier for item</span></span>|
|<span data-ttu-id="cdcff-136">说明</span><span class="sxs-lookup"><span data-stu-id="cdcff-136">description</span></span>|<span data-ttu-id="cdcff-137">String</span><span class="sxs-lookup"><span data-stu-id="cdcff-137">String</span></span>|<span data-ttu-id="cdcff-138">项目说明</span><span class="sxs-lookup"><span data-stu-id="cdcff-138">Description of the item</span></span>|
|<span data-ttu-id="cdcff-139">helpText</span><span class="sxs-lookup"><span data-stu-id="cdcff-139">helpText</span></span>|<span data-ttu-id="cdcff-140">String</span><span class="sxs-lookup"><span data-stu-id="cdcff-140">String</span></span>|<span data-ttu-id="cdcff-141">项目的帮助文本</span><span class="sxs-lookup"><span data-stu-id="cdcff-141">Help text of the item</span></span>|
|<span data-ttu-id="cdcff-142">name</span><span class="sxs-lookup"><span data-stu-id="cdcff-142">name</span></span>|<span data-ttu-id="cdcff-143">String</span><span class="sxs-lookup"><span data-stu-id="cdcff-143">String</span></span>|<span data-ttu-id="cdcff-144">项目名称</span><span class="sxs-lookup"><span data-stu-id="cdcff-144">Name of the item</span></span>|
|<span data-ttu-id="cdcff-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cdcff-145">displayName</span></span>|<span data-ttu-id="cdcff-146">String</span><span class="sxs-lookup"><span data-stu-id="cdcff-146">String</span></span>|<span data-ttu-id="cdcff-147">项目的显示名称</span><span class="sxs-lookup"><span data-stu-id="cdcff-147">Display name of the item</span></span>|
|<span data-ttu-id="cdcff-148">平台</span><span class="sxs-lookup"><span data-stu-id="cdcff-148">platforms</span></span>|[<span data-ttu-id="cdcff-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="cdcff-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="cdcff-150">平台类型，类别中的设置具有。</span><span class="sxs-lookup"><span data-stu-id="cdcff-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="cdcff-151">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="cdcff-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="cdcff-152">technologies</span><span class="sxs-lookup"><span data-stu-id="cdcff-152">technologies</span></span>|[<span data-ttu-id="cdcff-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="cdcff-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="cdcff-154">技术类型，类别中的设置具有。</span><span class="sxs-lookup"><span data-stu-id="cdcff-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="cdcff-155">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="cdcff-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="cdcff-156">settingUsage</span><span class="sxs-lookup"><span data-stu-id="cdcff-156">settingUsage</span></span>|[<span data-ttu-id="cdcff-157">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="cdcff-157">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="cdcff-158">指示类别包含用于合规性或配置的设置。</span><span class="sxs-lookup"><span data-stu-id="cdcff-158">Indicates that the category contains settings that are used for Compliance or Configuration.</span></span> <span data-ttu-id="cdcff-159">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="cdcff-159">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="cdcff-160">parentCategoryId</span><span class="sxs-lookup"><span data-stu-id="cdcff-160">parentCategoryId</span></span>|<span data-ttu-id="cdcff-161">String</span><span class="sxs-lookup"><span data-stu-id="cdcff-161">String</span></span>|<span data-ttu-id="cdcff-162">类别的父 ID。</span><span class="sxs-lookup"><span data-stu-id="cdcff-162">Parent id of the category.</span></span>|
|<span data-ttu-id="cdcff-163">rootCategoryId</span><span class="sxs-lookup"><span data-stu-id="cdcff-163">rootCategoryId</span></span>|<span data-ttu-id="cdcff-164">String</span><span class="sxs-lookup"><span data-stu-id="cdcff-164">String</span></span>|<span data-ttu-id="cdcff-165">类别的根 ID。</span><span class="sxs-lookup"><span data-stu-id="cdcff-165">Root id of the category.</span></span>|
|<span data-ttu-id="cdcff-166">childCategoryIds</span><span class="sxs-lookup"><span data-stu-id="cdcff-166">childCategoryIds</span></span>|<span data-ttu-id="cdcff-167">String 集合</span><span class="sxs-lookup"><span data-stu-id="cdcff-167">String collection</span></span>|<span data-ttu-id="cdcff-168">类别的子 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="cdcff-168">List of child ids of the category.</span></span>|



## <a name="response"></a><span data-ttu-id="cdcff-169">响应</span><span class="sxs-lookup"><span data-stu-id="cdcff-169">Response</span></span>
<span data-ttu-id="cdcff-170">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cdcff-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdcff-171">示例</span><span class="sxs-lookup"><span data-stu-id="cdcff-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdcff-172">请求</span><span class="sxs-lookup"><span data-stu-id="cdcff-172">Request</span></span>
<span data-ttu-id="cdcff-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdcff-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
Content-type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cdcff-174">响应</span><span class="sxs-lookup"><span data-stu-id="cdcff-174">Response</span></span>
<span data-ttu-id="cdcff-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdcff-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 514

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```




