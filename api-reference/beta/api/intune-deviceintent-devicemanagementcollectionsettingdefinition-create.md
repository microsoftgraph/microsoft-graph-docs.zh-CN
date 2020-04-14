---
title: 创建 deviceManagementCollectionSettingDefinition
description: 创建新的 deviceManagementCollectionSettingDefinition 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bc3ba3f8450a9c718c64f70fa4872fce89a7dc0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43329862"
---
# <a name="create-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="7bb2c-103">创建 deviceManagementCollectionSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="7bb2c-103">Create deviceManagementCollectionSettingDefinition</span></span>

<span data-ttu-id="7bb2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bb2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bb2c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bb2c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bb2c-107">创建新的[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-107">Create a new [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bb2c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7bb2c-108">Prerequisites</span></span>
<span data-ttu-id="7bb2c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bb2c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bb2c-111">Permission type</span></span>|<span data-ttu-id="7bb2c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7bb2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bb2c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bb2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bb2c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb2c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7bb2c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bb2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bb2c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-116">Not supported.</span></span>|
|<span data-ttu-id="7bb2c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bb2c-117">Application</span></span>|<span data-ttu-id="7bb2c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb2c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bb2c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bb2c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7bb2c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bb2c-120">Request headers</span></span>
|<span data-ttu-id="7bb2c-121">标头</span><span class="sxs-lookup"><span data-stu-id="7bb2c-121">Header</span></span>|<span data-ttu-id="7bb2c-122">值</span><span class="sxs-lookup"><span data-stu-id="7bb2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bb2c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bb2c-123">Authorization</span></span>|<span data-ttu-id="7bb2c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bb2c-125">接受</span><span class="sxs-lookup"><span data-stu-id="7bb2c-125">Accept</span></span>|<span data-ttu-id="7bb2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bb2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bb2c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bb2c-127">Request body</span></span>
<span data-ttu-id="7bb2c-128">在请求正文中，提供 deviceManagementCollectionSettingDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-128">In the request body, supply a JSON representation for the deviceManagementCollectionSettingDefinition object.</span></span>

<span data-ttu-id="7bb2c-129">下表显示创建 deviceManagementCollectionSettingDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-129">The following table shows the properties that are required when you create the deviceManagementCollectionSettingDefinition.</span></span>

|<span data-ttu-id="7bb2c-130">属性</span><span class="sxs-lookup"><span data-stu-id="7bb2c-130">Property</span></span>|<span data-ttu-id="7bb2c-131">类型</span><span class="sxs-lookup"><span data-stu-id="7bb2c-131">Type</span></span>|<span data-ttu-id="7bb2c-132">说明</span><span class="sxs-lookup"><span data-stu-id="7bb2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb2c-133">id</span><span class="sxs-lookup"><span data-stu-id="7bb2c-133">id</span></span>|<span data-ttu-id="7bb2c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7bb2c-134">String</span></span>|<span data-ttu-id="7bb2c-135">从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="7bb2c-135">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-136">valueType</span><span class="sxs-lookup"><span data-stu-id="7bb2c-136">valueType</span></span>|[<span data-ttu-id="7bb2c-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="7bb2c-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="7bb2c-138">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-138">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="7bb2c-139">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="7bb2c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7bb2c-140">displayName</span></span>|<span data-ttu-id="7bb2c-141">String</span><span class="sxs-lookup"><span data-stu-id="7bb2c-141">String</span></span>|<span data-ttu-id="7bb2c-142">设置的显示名称继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7bb2c-142">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="7bb2c-143">isTopLevel</span></span>|<span data-ttu-id="7bb2c-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="7bb2c-144">Boolean</span></span>|<span data-ttu-id="7bb2c-145">如果设置是顶级的，则可以对其进行配置，而无需将其包装在从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-146">description</span><span class="sxs-lookup"><span data-stu-id="7bb2c-146">description</span></span>|<span data-ttu-id="7bb2c-147">String</span><span class="sxs-lookup"><span data-stu-id="7bb2c-147">String</span></span>|<span data-ttu-id="7bb2c-148">该设置的说明继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7bb2c-148">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="7bb2c-149">placeholderText</span></span>|<span data-ttu-id="7bb2c-150">字符串</span><span class="sxs-lookup"><span data-stu-id="7bb2c-150">String</span></span>|<span data-ttu-id="7bb2c-151">占位符文本作为从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的有效输入的示例</span><span class="sxs-lookup"><span data-stu-id="7bb2c-151">Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="7bb2c-152">documentationUrl</span></span>|<span data-ttu-id="7bb2c-153">字符串</span><span class="sxs-lookup"><span data-stu-id="7bb2c-153">String</span></span>|<span data-ttu-id="7bb2c-154">设置从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url</span><span class="sxs-lookup"><span data-stu-id="7bb2c-154">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-155">keywords</span><span class="sxs-lookup"><span data-stu-id="7bb2c-155">keywords</span></span>|<span data-ttu-id="7bb2c-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="7bb2c-156">String collection</span></span>|<span data-ttu-id="7bb2c-157">与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字</span><span class="sxs-lookup"><span data-stu-id="7bb2c-157">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-158">施加</span><span class="sxs-lookup"><span data-stu-id="7bb2c-158">constraints</span></span>|<span data-ttu-id="7bb2c-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bb2c-159">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="7bb2c-160">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="7bb2c-160">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-161">依</span><span class="sxs-lookup"><span data-stu-id="7bb2c-161">dependencies</span></span>|<span data-ttu-id="7bb2c-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bb2c-162">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="7bb2c-163">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合</span><span class="sxs-lookup"><span data-stu-id="7bb2c-163">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="7bb2c-164">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bb2c-164">elementDefinitionId</span></span>|<span data-ttu-id="7bb2c-165">字符串</span><span class="sxs-lookup"><span data-stu-id="7bb2c-165">String</span></span>|<span data-ttu-id="7bb2c-166">描述集合的每个元素外观的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="7bb2c-166">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="7bb2c-167">响应</span><span class="sxs-lookup"><span data-stu-id="7bb2c-167">Response</span></span>
<span data-ttu-id="7bb2c-168">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-168">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bb2c-169">示例</span><span class="sxs-lookup"><span data-stu-id="7bb2c-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bb2c-170">请求</span><span class="sxs-lookup"><span data-stu-id="7bb2c-170">Request</span></span>
<span data-ttu-id="7bb2c-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 995

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="7bb2c-172">响应</span><span class="sxs-lookup"><span data-stu-id="7bb2c-172">Response</span></span>
<span data-ttu-id="7bb2c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bb2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1044

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  "elementDefinitionId": "Element Definition Id value"
}
```



