---
title: 创建 deviceManagementComplexSettingDefinition
description: 创建新的 deviceManagementComplexSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 018c9a5619c61a84c1b76f9467f3af30318ccc0c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290082"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="d3035-103">创建 deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="d3035-103">Create deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="d3035-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3035-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3035-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3035-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3035-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3035-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3035-107">创建新的 [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3035-107">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3035-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3035-108">Prerequisites</span></span>
<span data-ttu-id="d3035-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3035-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3035-111">Permission type</span></span>|<span data-ttu-id="d3035-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d3035-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3035-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3035-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3035-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3035-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3035-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3035-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3035-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3035-116">Not supported.</span></span>|
|<span data-ttu-id="d3035-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3035-117">Application</span></span>|<span data-ttu-id="d3035-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3035-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3035-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3035-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/settingDefinitions
POST /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="d3035-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3035-120">Request headers</span></span>
|<span data-ttu-id="d3035-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3035-121">Header</span></span>|<span data-ttu-id="d3035-122">值</span><span class="sxs-lookup"><span data-stu-id="d3035-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3035-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3035-123">Authorization</span></span>|<span data-ttu-id="d3035-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3035-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3035-125">接受</span><span class="sxs-lookup"><span data-stu-id="d3035-125">Accept</span></span>|<span data-ttu-id="d3035-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3035-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3035-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3035-127">Request body</span></span>
<span data-ttu-id="d3035-128">在请求正文中，提供 deviceManagementComplexSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3035-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="d3035-129">下表显示创建 deviceManagementComplexSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d3035-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="d3035-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3035-130">Property</span></span>|<span data-ttu-id="d3035-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3035-131">Type</span></span>|<span data-ttu-id="d3035-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3035-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3035-133">id</span><span class="sxs-lookup"><span data-stu-id="d3035-133">id</span></span>|<span data-ttu-id="d3035-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d3035-134">String</span></span>|<span data-ttu-id="d3035-135">从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="d3035-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-136">valueType</span><span class="sxs-lookup"><span data-stu-id="d3035-136">valueType</span></span>|[<span data-ttu-id="d3035-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="d3035-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="d3035-138">继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="d3035-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="d3035-139">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="d3035-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="d3035-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d3035-140">displayName</span></span>|<span data-ttu-id="d3035-141">字符串</span><span class="sxs-lookup"><span data-stu-id="d3035-141">String</span></span>|<span data-ttu-id="d3035-142">设置的显示名称继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d3035-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="d3035-143">isTopLevel</span></span>|<span data-ttu-id="d3035-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3035-144">Boolean</span></span>|<span data-ttu-id="d3035-145">如果设置是顶级的，则可以对其进行配置，而无需将其包装在从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。</span><span class="sxs-lookup"><span data-stu-id="d3035-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-146">description</span><span class="sxs-lookup"><span data-stu-id="d3035-146">description</span></span>|<span data-ttu-id="d3035-147">字符串</span><span class="sxs-lookup"><span data-stu-id="d3035-147">String</span></span>|<span data-ttu-id="d3035-148">该设置的说明继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d3035-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="d3035-149">placeholderText</span></span>|<span data-ttu-id="d3035-150">字符串</span><span class="sxs-lookup"><span data-stu-id="d3035-150">String</span></span>|<span data-ttu-id="d3035-151">占位符文本作为从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的有效输入的示例</span><span class="sxs-lookup"><span data-stu-id="d3035-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="d3035-152">documentationUrl</span></span>|<span data-ttu-id="d3035-153">字符串</span><span class="sxs-lookup"><span data-stu-id="d3035-153">String</span></span>|<span data-ttu-id="d3035-154">设置从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url</span><span class="sxs-lookup"><span data-stu-id="d3035-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="d3035-155">headerTitle</span></span>|<span data-ttu-id="d3035-156">字符串</span><span class="sxs-lookup"><span data-stu-id="d3035-156">String</span></span>|<span data-ttu-id="d3035-157">设置标头的标题代表从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置/设置的类别/部分</span><span class="sxs-lookup"><span data-stu-id="d3035-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="d3035-158">headerSubtitle</span></span>|<span data-ttu-id="d3035-159">字符串</span><span class="sxs-lookup"><span data-stu-id="d3035-159">String</span></span>|<span data-ttu-id="d3035-160">设置标头的副标题有关从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的类别/部分的更多详细信息</span><span class="sxs-lookup"><span data-stu-id="d3035-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-161">keywords</span><span class="sxs-lookup"><span data-stu-id="d3035-161">keywords</span></span>|<span data-ttu-id="d3035-162">String 集合</span><span class="sxs-lookup"><span data-stu-id="d3035-162">String collection</span></span>|<span data-ttu-id="d3035-163">与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字</span><span class="sxs-lookup"><span data-stu-id="d3035-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-164">施加</span><span class="sxs-lookup"><span data-stu-id="d3035-164">constraints</span></span>|<span data-ttu-id="d3035-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3035-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="d3035-166">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="d3035-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-167">依</span><span class="sxs-lookup"><span data-stu-id="d3035-167">dependencies</span></span>|<span data-ttu-id="d3035-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3035-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="d3035-169">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合</span><span class="sxs-lookup"><span data-stu-id="d3035-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="d3035-170">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="d3035-170">propertyDefinitionIds</span></span>|<span data-ttu-id="d3035-171">String 集合</span><span class="sxs-lookup"><span data-stu-id="d3035-171">String collection</span></span>|<span data-ttu-id="d3035-172">复杂设置的每个属性的定义</span><span class="sxs-lookup"><span data-stu-id="d3035-172">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="d3035-173">响应</span><span class="sxs-lookup"><span data-stu-id="d3035-173">Response</span></span>
<span data-ttu-id="d3035-174">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3035-174">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3035-175">示例</span><span class="sxs-lookup"><span data-stu-id="d3035-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3035-176">请求</span><span class="sxs-lookup"><span data-stu-id="d3035-176">Request</span></span>
<span data-ttu-id="d3035-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3035-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="d3035-178">响应</span><span class="sxs-lookup"><span data-stu-id="d3035-178">Response</span></span>
<span data-ttu-id="d3035-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3035-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




