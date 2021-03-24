---
title: 更新 deviceManagementAbstractComplexSettingDefinition
description: 更新 deviceManagementAbstractComplexSettingDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30344faf4060330c057d75c3ee41966c89bd558d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146851"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="12a0a-103">更新 deviceManagementAbstractComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="12a0a-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

<span data-ttu-id="12a0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a0a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12a0a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12a0a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12a0a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12a0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a0a-107">更新 [deviceManagementAbstractComplexSettingDefinition 对象](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="12a0a-107">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12a0a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12a0a-108">Prerequisites</span></span>
<span data-ttu-id="12a0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12a0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12a0a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12a0a-111">Permission type</span></span>|<span data-ttu-id="12a0a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12a0a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12a0a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12a0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12a0a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12a0a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12a0a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12a0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a0a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12a0a-116">Not supported.</span></span>|
|<span data-ttu-id="12a0a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12a0a-117">Application</span></span>|<span data-ttu-id="12a0a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12a0a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a0a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12a0a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="12a0a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12a0a-120">Request headers</span></span>
|<span data-ttu-id="12a0a-121">标头</span><span class="sxs-lookup"><span data-stu-id="12a0a-121">Header</span></span>|<span data-ttu-id="12a0a-122">值</span><span class="sxs-lookup"><span data-stu-id="12a0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12a0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12a0a-123">Authorization</span></span>|<span data-ttu-id="12a0a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12a0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12a0a-125">接受</span><span class="sxs-lookup"><span data-stu-id="12a0a-125">Accept</span></span>|<span data-ttu-id="12a0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12a0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12a0a-127">Request body</span></span>
<span data-ttu-id="12a0a-128">在请求正文中，提供 [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12a0a-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="12a0a-129">下表显示创建 [deviceManagementAbstractComplexSettingDefinition 时所需的属性](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="12a0a-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="12a0a-130">属性</span><span class="sxs-lookup"><span data-stu-id="12a0a-130">Property</span></span>|<span data-ttu-id="12a0a-131">类型</span><span class="sxs-lookup"><span data-stu-id="12a0a-131">Type</span></span>|<span data-ttu-id="12a0a-132">说明</span><span class="sxs-lookup"><span data-stu-id="12a0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a0a-133">id</span><span class="sxs-lookup"><span data-stu-id="12a0a-133">id</span></span>|<span data-ttu-id="12a0a-134">String</span><span class="sxs-lookup"><span data-stu-id="12a0a-134">String</span></span>|<span data-ttu-id="12a0a-135">设置定义的 ID 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-136">valueType</span><span class="sxs-lookup"><span data-stu-id="12a0a-136">valueType</span></span>|[<span data-ttu-id="12a0a-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="12a0a-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="12a0a-138">值数据类型继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="12a0a-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="12a0a-139">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="12a0a-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="12a0a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="12a0a-140">displayName</span></span>|<span data-ttu-id="12a0a-141">String</span><span class="sxs-lookup"><span data-stu-id="12a0a-141">String</span></span>|<span data-ttu-id="12a0a-142">该设置显示名称继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="12a0a-143">isTopLevel</span></span>|<span data-ttu-id="12a0a-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="12a0a-144">Boolean</span></span>|<span data-ttu-id="12a0a-145">如果该设置是顶级设置，则无需封装在集合或复杂设置中即可配置它。继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-146">说明</span><span class="sxs-lookup"><span data-stu-id="12a0a-146">description</span></span>|<span data-ttu-id="12a0a-147">String</span><span class="sxs-lookup"><span data-stu-id="12a0a-147">String</span></span>|<span data-ttu-id="12a0a-148">设置的说明 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="12a0a-149">placeholderText</span></span>|<span data-ttu-id="12a0a-150">String</span><span class="sxs-lookup"><span data-stu-id="12a0a-150">String</span></span>|<span data-ttu-id="12a0a-151">占位符文本作为有效输入的示例 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="12a0a-152">documentationUrl</span></span>|<span data-ttu-id="12a0a-153">String</span><span class="sxs-lookup"><span data-stu-id="12a0a-153">String</span></span>|<span data-ttu-id="12a0a-154">设置文档的 URL 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="12a0a-155">headerTitle</span></span>|<span data-ttu-id="12a0a-156">String</span><span class="sxs-lookup"><span data-stu-id="12a0a-156">String</span></span>|<span data-ttu-id="12a0a-157">设置标头的标题表示设置/设置的类别/部分 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-157">title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="12a0a-158">headerSubtitle</span></span>|<span data-ttu-id="12a0a-159">String</span><span class="sxs-lookup"><span data-stu-id="12a0a-159">String</span></span>|<span data-ttu-id="12a0a-160">有关类别/节的更多详细信息的设置标头的副标题 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-160">subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-161">keywords</span><span class="sxs-lookup"><span data-stu-id="12a0a-161">keywords</span></span>|<span data-ttu-id="12a0a-162">String collection</span><span class="sxs-lookup"><span data-stu-id="12a0a-162">String collection</span></span>|<span data-ttu-id="12a0a-163">与设置关联的关键字 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-163">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-164">约束</span><span class="sxs-lookup"><span data-stu-id="12a0a-164">constraints</span></span>|<span data-ttu-id="12a0a-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12a0a-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="12a0a-166">设置值的约束集合 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-166">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-167">依赖项</span><span class="sxs-lookup"><span data-stu-id="12a0a-167">dependencies</span></span>|<span data-ttu-id="12a0a-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12a0a-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="12a0a-169">其他设置上的依赖项集合 继承自 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12a0a-169">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="12a0a-170">实现</span><span class="sxs-lookup"><span data-stu-id="12a0a-170">implementations</span></span>|<span data-ttu-id="12a0a-171">String collection</span><span class="sxs-lookup"><span data-stu-id="12a0a-171">String collection</span></span>|<span data-ttu-id="12a0a-172">此抽象复杂设置的所有可能的实现的定义 ID 列表</span><span class="sxs-lookup"><span data-stu-id="12a0a-172">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="12a0a-173">响应</span><span class="sxs-lookup"><span data-stu-id="12a0a-173">Response</span></span>
<span data-ttu-id="12a0a-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12a0a-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a0a-175">示例</span><span class="sxs-lookup"><span data-stu-id="12a0a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a0a-176">请求</span><span class="sxs-lookup"><span data-stu-id="12a0a-176">Request</span></span>
<span data-ttu-id="12a0a-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12a0a-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1088

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="12a0a-178">响应</span><span class="sxs-lookup"><span data-stu-id="12a0a-178">Response</span></span>
<span data-ttu-id="12a0a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12a0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
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
  "implementations": [
    "Implementations value"
  ]
}
```




