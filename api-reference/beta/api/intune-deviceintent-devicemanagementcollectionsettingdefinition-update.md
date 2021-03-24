---
title: 更新 deviceManagementCollectionSettingDefinition
description: 更新 deviceManagementCollectionSettingDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0bfd9fc6e84ba6c11d6941e87a7acac9237c3562
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132126"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="e1705-103">更新 deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="e1705-103">Update deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="e1705-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1705-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1705-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1705-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1705-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1705-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1705-107">更新 [deviceManagementCollectionSettingDefinition 对象](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e1705-107">Update the properties of a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1705-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e1705-108">Prerequisites</span></span>
<span data-ttu-id="e1705-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1705-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1705-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1705-111">Permission type</span></span>|<span data-ttu-id="e1705-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1705-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1705-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1705-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1705-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1705-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1705-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1705-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1705-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1705-116">Not supported.</span></span>|
|<span data-ttu-id="e1705-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1705-117">Application</span></span>|<span data-ttu-id="e1705-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1705-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1705-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1705-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e1705-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1705-120">Request headers</span></span>
|<span data-ttu-id="e1705-121">标头</span><span class="sxs-lookup"><span data-stu-id="e1705-121">Header</span></span>|<span data-ttu-id="e1705-122">值</span><span class="sxs-lookup"><span data-stu-id="e1705-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1705-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1705-123">Authorization</span></span>|<span data-ttu-id="e1705-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e1705-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1705-125">接受</span><span class="sxs-lookup"><span data-stu-id="e1705-125">Accept</span></span>|<span data-ttu-id="e1705-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1705-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1705-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1705-127">Request body</span></span>
<span data-ttu-id="e1705-128">在请求正文中，提供 [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1705-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

<span data-ttu-id="e1705-129">下表显示创建 [deviceManagementCollectionSettingDefinition 时所需的属性](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e1705-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md).</span></span>

|<span data-ttu-id="e1705-130">属性</span><span class="sxs-lookup"><span data-stu-id="e1705-130">Property</span></span>|<span data-ttu-id="e1705-131">类型</span><span class="sxs-lookup"><span data-stu-id="e1705-131">Type</span></span>|<span data-ttu-id="e1705-132">说明</span><span class="sxs-lookup"><span data-stu-id="e1705-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1705-133">id</span><span class="sxs-lookup"><span data-stu-id="e1705-133">id</span></span>|<span data-ttu-id="e1705-134">String</span><span class="sxs-lookup"><span data-stu-id="e1705-134">String</span></span>|<span data-ttu-id="e1705-135">设置定义的 ID 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-136">valueType</span><span class="sxs-lookup"><span data-stu-id="e1705-136">valueType</span></span>|[<span data-ttu-id="e1705-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="e1705-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="e1705-138">值数据类型继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="e1705-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="e1705-139">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="e1705-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="e1705-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e1705-140">displayName</span></span>|<span data-ttu-id="e1705-141">String</span><span class="sxs-lookup"><span data-stu-id="e1705-141">String</span></span>|<span data-ttu-id="e1705-142">该设置显示名称继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="e1705-143">isTopLevel</span></span>|<span data-ttu-id="e1705-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1705-144">Boolean</span></span>|<span data-ttu-id="e1705-145">如果该设置是顶级设置，则无需封装在集合或复杂设置中即可配置它。继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-146">说明</span><span class="sxs-lookup"><span data-stu-id="e1705-146">description</span></span>|<span data-ttu-id="e1705-147">String</span><span class="sxs-lookup"><span data-stu-id="e1705-147">String</span></span>|<span data-ttu-id="e1705-148">设置的说明 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="e1705-149">placeholderText</span></span>|<span data-ttu-id="e1705-150">String</span><span class="sxs-lookup"><span data-stu-id="e1705-150">String</span></span>|<span data-ttu-id="e1705-151">占位符文本作为有效输入的示例 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="e1705-152">documentationUrl</span></span>|<span data-ttu-id="e1705-153">String</span><span class="sxs-lookup"><span data-stu-id="e1705-153">String</span></span>|<span data-ttu-id="e1705-154">设置文档的 URL 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="e1705-155">headerTitle</span></span>|<span data-ttu-id="e1705-156">String</span><span class="sxs-lookup"><span data-stu-id="e1705-156">String</span></span>|<span data-ttu-id="e1705-157">设置标头的标题表示设置/设置的类别/部分 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="e1705-158">headerSubtitle</span></span>|<span data-ttu-id="e1705-159">String</span><span class="sxs-lookup"><span data-stu-id="e1705-159">String</span></span>|<span data-ttu-id="e1705-160">有关类别/节的更多详细信息的设置标头的副标题 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-161">keywords</span><span class="sxs-lookup"><span data-stu-id="e1705-161">keywords</span></span>|<span data-ttu-id="e1705-162">String collection</span><span class="sxs-lookup"><span data-stu-id="e1705-162">String collection</span></span>|<span data-ttu-id="e1705-163">与设置关联的关键字 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-164">约束</span><span class="sxs-lookup"><span data-stu-id="e1705-164">constraints</span></span>|<span data-ttu-id="e1705-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1705-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="e1705-166">设置值的约束集合 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-167">依赖项</span><span class="sxs-lookup"><span data-stu-id="e1705-167">dependencies</span></span>|<span data-ttu-id="e1705-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1705-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="e1705-169">其他设置上的依赖项集合 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e1705-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e1705-170">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e1705-170">elementDefinitionId</span></span>|<span data-ttu-id="e1705-171">String</span><span class="sxs-lookup"><span data-stu-id="e1705-171">String</span></span>|<span data-ttu-id="e1705-172">描述集合的每个元素外观的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="e1705-172">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="e1705-173">响应</span><span class="sxs-lookup"><span data-stu-id="e1705-173">Response</span></span>
<span data-ttu-id="e1705-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1705-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1705-175">示例</span><span class="sxs-lookup"><span data-stu-id="e1705-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1705-176">请求</span><span class="sxs-lookup"><span data-stu-id="e1705-176">Request</span></span>
<span data-ttu-id="e1705-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1705-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1081

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="e1705-178">响应</span><span class="sxs-lookup"><span data-stu-id="e1705-178">Response</span></span>
<span data-ttu-id="e1705-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1705-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  "elementDefinitionId": "Element Definition Id value"
}
```




