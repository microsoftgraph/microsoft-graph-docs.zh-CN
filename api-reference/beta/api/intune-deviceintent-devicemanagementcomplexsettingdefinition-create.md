---
title: 创建 deviceManagementComplexSettingDefinition
description: 创建新的 deviceManagementComplexSettingDefinition 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e345b47010b25ecc7e239d7b4377ed48f15657d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472119"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="e90a2-103">创建 deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="e90a2-103">Create deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="e90a2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e90a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e90a2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e90a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e90a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e90a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e90a2-107">创建新的[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e90a2-107">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e90a2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e90a2-108">Prerequisites</span></span>
<span data-ttu-id="e90a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e90a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e90a2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e90a2-111">Permission type</span></span>|<span data-ttu-id="e90a2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e90a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e90a2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e90a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e90a2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e90a2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e90a2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e90a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e90a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e90a2-116">Not supported.</span></span>|
|<span data-ttu-id="e90a2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e90a2-117">Application</span></span>|<span data-ttu-id="e90a2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e90a2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e90a2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e90a2-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e90a2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e90a2-120">Request headers</span></span>
|<span data-ttu-id="e90a2-121">标头</span><span class="sxs-lookup"><span data-stu-id="e90a2-121">Header</span></span>|<span data-ttu-id="e90a2-122">值</span><span class="sxs-lookup"><span data-stu-id="e90a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e90a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e90a2-123">Authorization</span></span>|<span data-ttu-id="e90a2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e90a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e90a2-125">接受</span><span class="sxs-lookup"><span data-stu-id="e90a2-125">Accept</span></span>|<span data-ttu-id="e90a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e90a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e90a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e90a2-127">Request body</span></span>
<span data-ttu-id="e90a2-128">在请求正文中，提供 deviceManagementComplexSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e90a2-128">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="e90a2-129">下表显示创建 deviceManagementComplexSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e90a2-129">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="e90a2-130">属性</span><span class="sxs-lookup"><span data-stu-id="e90a2-130">Property</span></span>|<span data-ttu-id="e90a2-131">类型</span><span class="sxs-lookup"><span data-stu-id="e90a2-131">Type</span></span>|<span data-ttu-id="e90a2-132">说明</span><span class="sxs-lookup"><span data-stu-id="e90a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e90a2-133">id</span><span class="sxs-lookup"><span data-stu-id="e90a2-133">id</span></span>|<span data-ttu-id="e90a2-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e90a2-134">String</span></span>|<span data-ttu-id="e90a2-135">从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="e90a2-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-136">valueType</span><span class="sxs-lookup"><span data-stu-id="e90a2-136">valueType</span></span>|[<span data-ttu-id="e90a2-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="e90a2-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="e90a2-138">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="e90a2-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="e90a2-139">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="e90a2-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="e90a2-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e90a2-140">displayName</span></span>|<span data-ttu-id="e90a2-141">String</span><span class="sxs-lookup"><span data-stu-id="e90a2-141">String</span></span>|<span data-ttu-id="e90a2-142">设置的显示名称继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e90a2-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="e90a2-143">isTopLevel</span></span>|<span data-ttu-id="e90a2-144">布尔</span><span class="sxs-lookup"><span data-stu-id="e90a2-144">Boolean</span></span>|<span data-ttu-id="e90a2-145">如果设置是顶级的，则可以对其进行配置，而无需将其包装在从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。</span><span class="sxs-lookup"><span data-stu-id="e90a2-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-146">说明</span><span class="sxs-lookup"><span data-stu-id="e90a2-146">description</span></span>|<span data-ttu-id="e90a2-147">String</span><span class="sxs-lookup"><span data-stu-id="e90a2-147">String</span></span>|<span data-ttu-id="e90a2-148">该设置的说明继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e90a2-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="e90a2-149">placeholderText</span></span>|<span data-ttu-id="e90a2-150">String</span><span class="sxs-lookup"><span data-stu-id="e90a2-150">String</span></span>|<span data-ttu-id="e90a2-151">占位符文本作为从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的有效输入的示例</span><span class="sxs-lookup"><span data-stu-id="e90a2-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="e90a2-152">documentationUrl</span></span>|<span data-ttu-id="e90a2-153">String</span><span class="sxs-lookup"><span data-stu-id="e90a2-153">String</span></span>|<span data-ttu-id="e90a2-154">设置从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url</span><span class="sxs-lookup"><span data-stu-id="e90a2-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-155">keywords</span><span class="sxs-lookup"><span data-stu-id="e90a2-155">keywords</span></span>|<span data-ttu-id="e90a2-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="e90a2-156">String collection</span></span>|<span data-ttu-id="e90a2-157">与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字</span><span class="sxs-lookup"><span data-stu-id="e90a2-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-158">施加</span><span class="sxs-lookup"><span data-stu-id="e90a2-158">constraints</span></span>|<span data-ttu-id="e90a2-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="e90a2-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="e90a2-160">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="e90a2-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-161">依</span><span class="sxs-lookup"><span data-stu-id="e90a2-161">dependencies</span></span>|<span data-ttu-id="e90a2-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="e90a2-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="e90a2-163">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合</span><span class="sxs-lookup"><span data-stu-id="e90a2-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="e90a2-164">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="e90a2-164">propertyDefinitionIds</span></span>|<span data-ttu-id="e90a2-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="e90a2-165">String collection</span></span>|<span data-ttu-id="e90a2-166">复杂设置的每个属性的定义</span><span class="sxs-lookup"><span data-stu-id="e90a2-166">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="e90a2-167">响应</span><span class="sxs-lookup"><span data-stu-id="e90a2-167">Response</span></span>
<span data-ttu-id="e90a2-168">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e90a2-168">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e90a2-169">示例</span><span class="sxs-lookup"><span data-stu-id="e90a2-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="e90a2-170">请求</span><span class="sxs-lookup"><span data-stu-id="e90a2-170">Request</span></span>
<span data-ttu-id="e90a2-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e90a2-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 1008

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
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

### <a name="response"></a><span data-ttu-id="e90a2-172">响应</span><span class="sxs-lookup"><span data-stu-id="e90a2-172">Response</span></span>
<span data-ttu-id="e90a2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e90a2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1057

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "placeholderText": "Placeholder Text value",
  "documentationUrl": "https://example.com/documentationUrl/",
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





