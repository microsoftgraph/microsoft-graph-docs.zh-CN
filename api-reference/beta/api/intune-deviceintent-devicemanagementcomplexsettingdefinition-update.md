---
title: 更新 deviceManagementComplexSettingDefinition
description: 更新 deviceManagementComplexSettingDefinition 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8e8b773e73701fe0de0de9601d0c55221b75d23
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946047"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="bb9bb-103">更新 deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="bb9bb-103">Update deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="bb9bb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb9bb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb9bb-106">更新[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-106">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb9bb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb9bb-107">Prerequisites</span></span>
<span data-ttu-id="bb9bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb9bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb9bb-110">Permission type</span></span>|<span data-ttu-id="bb9bb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb9bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb9bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb9bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb9bb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9bb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb9bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb9bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb9bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-115">Not supported.</span></span>|
|<span data-ttu-id="bb9bb-116">Application</span><span class="sxs-lookup"><span data-stu-id="bb9bb-116">Application</span></span>|<span data-ttu-id="bb9bb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9bb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb9bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb9bb-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bb9bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb9bb-119">Request headers</span></span>
|<span data-ttu-id="bb9bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="bb9bb-120">Header</span></span>|<span data-ttu-id="bb9bb-121">值</span><span class="sxs-lookup"><span data-stu-id="bb9bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb9bb-122">授权</span><span class="sxs-lookup"><span data-stu-id="bb9bb-122">Authorization</span></span>|<span data-ttu-id="bb9bb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb9bb-124">接受</span><span class="sxs-lookup"><span data-stu-id="bb9bb-124">Accept</span></span>|<span data-ttu-id="bb9bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb9bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb9bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb9bb-126">Request body</span></span>
<span data-ttu-id="bb9bb-127">在请求正文中，提供[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="bb9bb-128">下表显示创建[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="bb9bb-129">属性</span><span class="sxs-lookup"><span data-stu-id="bb9bb-129">Property</span></span>|<span data-ttu-id="bb9bb-130">类型</span><span class="sxs-lookup"><span data-stu-id="bb9bb-130">Type</span></span>|<span data-ttu-id="bb9bb-131">说明</span><span class="sxs-lookup"><span data-stu-id="bb9bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb9bb-132">id</span><span class="sxs-lookup"><span data-stu-id="bb9bb-132">id</span></span>|<span data-ttu-id="bb9bb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="bb9bb-133">String</span></span>|<span data-ttu-id="bb9bb-134">从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="bb9bb-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-135">valueType</span><span class="sxs-lookup"><span data-stu-id="bb9bb-135">valueType</span></span>|[<span data-ttu-id="bb9bb-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="bb9bb-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="bb9bb-137">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="bb9bb-138">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="bb9bb-139">displayName</span><span class="sxs-lookup"><span data-stu-id="bb9bb-139">displayName</span></span>|<span data-ttu-id="bb9bb-140">String</span><span class="sxs-lookup"><span data-stu-id="bb9bb-140">String</span></span>|<span data-ttu-id="bb9bb-141">设置的显示名称继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb9bb-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="bb9bb-142">isTopLevel</span></span>|<span data-ttu-id="bb9bb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb9bb-143">Boolean</span></span>|<span data-ttu-id="bb9bb-144">如果设置是顶级的，则可以对其进行配置，而无需将其包装在从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-145">说明</span><span class="sxs-lookup"><span data-stu-id="bb9bb-145">description</span></span>|<span data-ttu-id="bb9bb-146">String</span><span class="sxs-lookup"><span data-stu-id="bb9bb-146">String</span></span>|<span data-ttu-id="bb9bb-147">该设置的说明继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bb9bb-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="bb9bb-148">documentationUrl</span></span>|<span data-ttu-id="bb9bb-149">字符串</span><span class="sxs-lookup"><span data-stu-id="bb9bb-149">String</span></span>|<span data-ttu-id="bb9bb-150">设置从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url</span><span class="sxs-lookup"><span data-stu-id="bb9bb-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-151">keywords</span><span class="sxs-lookup"><span data-stu-id="bb9bb-151">keywords</span></span>|<span data-ttu-id="bb9bb-152">String collection</span><span class="sxs-lookup"><span data-stu-id="bb9bb-152">String collection</span></span>|<span data-ttu-id="bb9bb-153">与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字</span><span class="sxs-lookup"><span data-stu-id="bb9bb-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-154">施加</span><span class="sxs-lookup"><span data-stu-id="bb9bb-154">constraints</span></span>|<span data-ttu-id="bb9bb-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb9bb-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="bb9bb-156">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="bb9bb-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-157">依</span><span class="sxs-lookup"><span data-stu-id="bb9bb-157">dependencies</span></span>|<span data-ttu-id="bb9bb-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb9bb-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="bb9bb-159">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合</span><span class="sxs-lookup"><span data-stu-id="bb9bb-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="bb9bb-160">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="bb9bb-160">propertyDefinitionIds</span></span>|<span data-ttu-id="bb9bb-161">String collection</span><span class="sxs-lookup"><span data-stu-id="bb9bb-161">String collection</span></span>|<span data-ttu-id="bb9bb-162">复杂设置的每个属性的定义</span><span class="sxs-lookup"><span data-stu-id="bb9bb-162">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="bb9bb-163">响应</span><span class="sxs-lookup"><span data-stu-id="bb9bb-163">Response</span></span>
<span data-ttu-id="bb9bb-164">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb9bb-165">示例</span><span class="sxs-lookup"><span data-stu-id="bb9bb-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb9bb-166">请求</span><span class="sxs-lookup"><span data-stu-id="bb9bb-166">Request</span></span>
<span data-ttu-id="bb9bb-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="bb9bb-168">响应</span><span class="sxs-lookup"><span data-stu-id="bb9bb-168">Response</span></span>
<span data-ttu-id="bb9bb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb9bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





