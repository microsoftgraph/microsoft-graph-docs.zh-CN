---
title: 创建 deviceManagementComplexSettingDefinition
description: 创建新的 deviceManagementComplexSettingDefinition 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb4447ca1e82cbc64eeccd9d9ffd242c4dc525ad
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960774"
---
# <a name="create-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="dfe6c-103">创建 deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="dfe6c-103">Create deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="dfe6c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfe6c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfe6c-106">创建新的[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-106">Create a new [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfe6c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfe6c-107">Prerequisites</span></span>
<span data-ttu-id="dfe6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfe6c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfe6c-110">Permission type</span></span>|<span data-ttu-id="dfe6c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dfe6c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfe6c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfe6c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfe6c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfe6c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dfe6c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfe6c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfe6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-115">Not supported.</span></span>|
|<span data-ttu-id="dfe6c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfe6c-116">Application</span></span>|<span data-ttu-id="dfe6c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfe6c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfe6c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dfe6c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfe6c-119">Request headers</span></span>
|<span data-ttu-id="dfe6c-120">标头</span><span class="sxs-lookup"><span data-stu-id="dfe6c-120">Header</span></span>|<span data-ttu-id="dfe6c-121">值</span><span class="sxs-lookup"><span data-stu-id="dfe6c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfe6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfe6c-122">Authorization</span></span>|<span data-ttu-id="dfe6c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfe6c-124">接受</span><span class="sxs-lookup"><span data-stu-id="dfe6c-124">Accept</span></span>|<span data-ttu-id="dfe6c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfe6c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfe6c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfe6c-126">Request body</span></span>
<span data-ttu-id="dfe6c-127">在请求正文中, 提供 deviceManagementComplexSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-127">In the request body, supply a JSON representation for the deviceManagementComplexSettingDefinition object.</span></span>

<span data-ttu-id="dfe6c-128">下表显示创建 deviceManagementComplexSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-128">The following table shows the properties that are required when you create the deviceManagementComplexSettingDefinition.</span></span>

|<span data-ttu-id="dfe6c-129">属性</span><span class="sxs-lookup"><span data-stu-id="dfe6c-129">Property</span></span>|<span data-ttu-id="dfe6c-130">类型</span><span class="sxs-lookup"><span data-stu-id="dfe6c-130">Type</span></span>|<span data-ttu-id="dfe6c-131">说明</span><span class="sxs-lookup"><span data-stu-id="dfe6c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfe6c-132">id</span><span class="sxs-lookup"><span data-stu-id="dfe6c-132">id</span></span>|<span data-ttu-id="dfe6c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dfe6c-133">String</span></span>|<span data-ttu-id="dfe6c-134">从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="dfe6c-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-135">valueType</span><span class="sxs-lookup"><span data-stu-id="dfe6c-135">valueType</span></span>|[<span data-ttu-id="dfe6c-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="dfe6c-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="dfe6c-137">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="dfe6c-138">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="dfe6c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dfe6c-139">displayName</span></span>|<span data-ttu-id="dfe6c-140">String</span><span class="sxs-lookup"><span data-stu-id="dfe6c-140">String</span></span>|<span data-ttu-id="dfe6c-141">设置的显示名称继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dfe6c-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="dfe6c-142">isTopLevel</span></span>|<span data-ttu-id="dfe6c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfe6c-143">Boolean</span></span>|<span data-ttu-id="dfe6c-144">如果设置是顶级的, 则可以对其进行配置, 而无需将其包装在从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-145">说明</span><span class="sxs-lookup"><span data-stu-id="dfe6c-145">description</span></span>|<span data-ttu-id="dfe6c-146">String</span><span class="sxs-lookup"><span data-stu-id="dfe6c-146">String</span></span>|<span data-ttu-id="dfe6c-147">该设置的说明继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dfe6c-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="dfe6c-148">documentationUrl</span></span>|<span data-ttu-id="dfe6c-149">String</span><span class="sxs-lookup"><span data-stu-id="dfe6c-149">String</span></span>|<span data-ttu-id="dfe6c-150">设置从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url</span><span class="sxs-lookup"><span data-stu-id="dfe6c-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-151">keywords</span><span class="sxs-lookup"><span data-stu-id="dfe6c-151">keywords</span></span>|<span data-ttu-id="dfe6c-152">String collection</span><span class="sxs-lookup"><span data-stu-id="dfe6c-152">String collection</span></span>|<span data-ttu-id="dfe6c-153">与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字</span><span class="sxs-lookup"><span data-stu-id="dfe6c-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-154">施加</span><span class="sxs-lookup"><span data-stu-id="dfe6c-154">constraints</span></span>|<span data-ttu-id="dfe6c-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="dfe6c-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="dfe6c-156">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="dfe6c-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-157">依</span><span class="sxs-lookup"><span data-stu-id="dfe6c-157">dependencies</span></span>|<span data-ttu-id="dfe6c-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="dfe6c-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="dfe6c-159">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合</span><span class="sxs-lookup"><span data-stu-id="dfe6c-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dfe6c-160">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="dfe6c-160">propertyDefinitionIds</span></span>|<span data-ttu-id="dfe6c-161">String collection</span><span class="sxs-lookup"><span data-stu-id="dfe6c-161">String collection</span></span>|<span data-ttu-id="dfe6c-162">复杂设置的每个属性的定义</span><span class="sxs-lookup"><span data-stu-id="dfe6c-162">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="dfe6c-163">响应</span><span class="sxs-lookup"><span data-stu-id="dfe6c-163">Response</span></span>
<span data-ttu-id="dfe6c-164">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-164">If successful, this method returns a `201 Created` response code and a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfe6c-165">示例</span><span class="sxs-lookup"><span data-stu-id="dfe6c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfe6c-166">请求</span><span class="sxs-lookup"><span data-stu-id="dfe6c-166">Request</span></span>
<span data-ttu-id="dfe6c-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 808

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="dfe6c-168">响应</span><span class="sxs-lookup"><span data-stu-id="dfe6c-168">Response</span></span>
<span data-ttu-id="dfe6c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfe6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 857

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```





