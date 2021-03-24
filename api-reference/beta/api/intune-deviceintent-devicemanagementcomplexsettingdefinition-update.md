---
title: 更新 deviceManagementComplexSettingDefinition
description: 更新 deviceManagementComplexSettingDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e09bbe4c8372840b35cd27229750f781282f115
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132119"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="5c1ca-103">更新 deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="5c1ca-103">Update deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="5c1ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c1ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c1ca-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c1ca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c1ca-107">更新 [deviceManagementComplexSettingDefinition 对象](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-107">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c1ca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c1ca-108">Prerequisites</span></span>
<span data-ttu-id="5c1ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c1ca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c1ca-111">Permission type</span></span>|<span data-ttu-id="5c1ca-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c1ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c1ca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c1ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c1ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c1ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c1ca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c1ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c1ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-116">Not supported.</span></span>|
|<span data-ttu-id="5c1ca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c1ca-117">Application</span></span>|<span data-ttu-id="5c1ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c1ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c1ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c1ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="5c1ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c1ca-120">Request headers</span></span>
|<span data-ttu-id="5c1ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="5c1ca-121">Header</span></span>|<span data-ttu-id="5c1ca-122">值</span><span class="sxs-lookup"><span data-stu-id="5c1ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c1ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c1ca-123">Authorization</span></span>|<span data-ttu-id="5c1ca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c1ca-125">接受</span><span class="sxs-lookup"><span data-stu-id="5c1ca-125">Accept</span></span>|<span data-ttu-id="5c1ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c1ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c1ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c1ca-127">Request body</span></span>
<span data-ttu-id="5c1ca-128">在请求正文中，提供 [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="5c1ca-129">下表显示创建 [deviceManagementComplexSettingDefinition 时所需的属性](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="5c1ca-130">属性</span><span class="sxs-lookup"><span data-stu-id="5c1ca-130">Property</span></span>|<span data-ttu-id="5c1ca-131">类型</span><span class="sxs-lookup"><span data-stu-id="5c1ca-131">Type</span></span>|<span data-ttu-id="5c1ca-132">说明</span><span class="sxs-lookup"><span data-stu-id="5c1ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c1ca-133">id</span><span class="sxs-lookup"><span data-stu-id="5c1ca-133">id</span></span>|<span data-ttu-id="5c1ca-134">String</span><span class="sxs-lookup"><span data-stu-id="5c1ca-134">String</span></span>|<span data-ttu-id="5c1ca-135">设置定义的 ID 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-136">valueType</span><span class="sxs-lookup"><span data-stu-id="5c1ca-136">valueType</span></span>|[<span data-ttu-id="5c1ca-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="5c1ca-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="5c1ca-138">值数据类型继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="5c1ca-139">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="5c1ca-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5c1ca-140">displayName</span></span>|<span data-ttu-id="5c1ca-141">String</span><span class="sxs-lookup"><span data-stu-id="5c1ca-141">String</span></span>|<span data-ttu-id="5c1ca-142">该设置显示名称继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="5c1ca-143">isTopLevel</span></span>|<span data-ttu-id="5c1ca-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c1ca-144">Boolean</span></span>|<span data-ttu-id="5c1ca-145">如果该设置是顶级设置，则无需封装在集合或复杂设置中即可配置它。继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-146">说明</span><span class="sxs-lookup"><span data-stu-id="5c1ca-146">description</span></span>|<span data-ttu-id="5c1ca-147">String</span><span class="sxs-lookup"><span data-stu-id="5c1ca-147">String</span></span>|<span data-ttu-id="5c1ca-148">设置的说明 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="5c1ca-149">placeholderText</span></span>|<span data-ttu-id="5c1ca-150">String</span><span class="sxs-lookup"><span data-stu-id="5c1ca-150">String</span></span>|<span data-ttu-id="5c1ca-151">占位符文本作为有效输入的示例 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="5c1ca-152">documentationUrl</span></span>|<span data-ttu-id="5c1ca-153">String</span><span class="sxs-lookup"><span data-stu-id="5c1ca-153">String</span></span>|<span data-ttu-id="5c1ca-154">设置文档的 URL 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="5c1ca-155">headerTitle</span></span>|<span data-ttu-id="5c1ca-156">String</span><span class="sxs-lookup"><span data-stu-id="5c1ca-156">String</span></span>|<span data-ttu-id="5c1ca-157">设置标头的标题表示设置/设置的类别/部分 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="5c1ca-158">headerSubtitle</span></span>|<span data-ttu-id="5c1ca-159">String</span><span class="sxs-lookup"><span data-stu-id="5c1ca-159">String</span></span>|<span data-ttu-id="5c1ca-160">有关类别/节的更多详细信息的设置标头的副标题 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-161">keywords</span><span class="sxs-lookup"><span data-stu-id="5c1ca-161">keywords</span></span>|<span data-ttu-id="5c1ca-162">String collection</span><span class="sxs-lookup"><span data-stu-id="5c1ca-162">String collection</span></span>|<span data-ttu-id="5c1ca-163">与设置关联的关键字 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-164">约束</span><span class="sxs-lookup"><span data-stu-id="5c1ca-164">constraints</span></span>|<span data-ttu-id="5c1ca-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c1ca-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="5c1ca-166">设置值的约束集合 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-167">依赖项</span><span class="sxs-lookup"><span data-stu-id="5c1ca-167">dependencies</span></span>|<span data-ttu-id="5c1ca-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c1ca-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="5c1ca-169">其他设置上的依赖项集合 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5c1ca-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5c1ca-170">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="5c1ca-170">propertyDefinitionIds</span></span>|<span data-ttu-id="5c1ca-171">String collection</span><span class="sxs-lookup"><span data-stu-id="5c1ca-171">String collection</span></span>|<span data-ttu-id="5c1ca-172">复杂设置的每个属性的定义</span><span class="sxs-lookup"><span data-stu-id="5c1ca-172">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="5c1ca-173">响应</span><span class="sxs-lookup"><span data-stu-id="5c1ca-173">Response</span></span>
<span data-ttu-id="5c1ca-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c1ca-175">示例</span><span class="sxs-lookup"><span data-stu-id="5c1ca-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c1ca-176">请求</span><span class="sxs-lookup"><span data-stu-id="5c1ca-176">Request</span></span>
<span data-ttu-id="5c1ca-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1094

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5c1ca-178">响应</span><span class="sxs-lookup"><span data-stu-id="5c1ca-178">Response</span></span>
<span data-ttu-id="5c1ca-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c1ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1143

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "headerTitle": "Header Title value",
  "headerSubtitle": "Header Subtitle value",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "Supported Types value"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "Supported Types value"
          ]
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```




