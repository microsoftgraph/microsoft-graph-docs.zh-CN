---
title: 更新 deviceManagementSettingDefinition
description: 更新 deviceManagementSettingDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343971cccdbcf64bbb04279de069ac3e0020362f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146571"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="46351-103">更新 deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="46351-103">Update deviceManagementSettingDefinition</span></span>

<span data-ttu-id="46351-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46351-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46351-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46351-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46351-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46351-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46351-107">更新 [deviceManagementSettingDefinition 对象](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="46351-107">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46351-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="46351-108">Prerequisites</span></span>
<span data-ttu-id="46351-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46351-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46351-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="46351-111">Permission type</span></span>|<span data-ttu-id="46351-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46351-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46351-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46351-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46351-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46351-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46351-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46351-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46351-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46351-116">Not supported.</span></span>|
|<span data-ttu-id="46351-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="46351-117">Application</span></span>|<span data-ttu-id="46351-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46351-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46351-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46351-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="46351-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="46351-120">Request headers</span></span>
|<span data-ttu-id="46351-121">标头</span><span class="sxs-lookup"><span data-stu-id="46351-121">Header</span></span>|<span data-ttu-id="46351-122">值</span><span class="sxs-lookup"><span data-stu-id="46351-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46351-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46351-123">Authorization</span></span>|<span data-ttu-id="46351-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46351-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46351-125">接受</span><span class="sxs-lookup"><span data-stu-id="46351-125">Accept</span></span>|<span data-ttu-id="46351-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46351-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46351-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="46351-127">Request body</span></span>
<span data-ttu-id="46351-128">在请求正文中，提供 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46351-128">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="46351-129">下表显示创建 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="46351-129">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="46351-130">属性</span><span class="sxs-lookup"><span data-stu-id="46351-130">Property</span></span>|<span data-ttu-id="46351-131">类型</span><span class="sxs-lookup"><span data-stu-id="46351-131">Type</span></span>|<span data-ttu-id="46351-132">说明</span><span class="sxs-lookup"><span data-stu-id="46351-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46351-133">id</span><span class="sxs-lookup"><span data-stu-id="46351-133">id</span></span>|<span data-ttu-id="46351-134">String</span><span class="sxs-lookup"><span data-stu-id="46351-134">String</span></span>|<span data-ttu-id="46351-135">设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="46351-135">The ID of the setting definition</span></span>|
|<span data-ttu-id="46351-136">valueType</span><span class="sxs-lookup"><span data-stu-id="46351-136">valueType</span></span>|[<span data-ttu-id="46351-137">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="46351-137">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="46351-138">值的 数据类型。</span><span class="sxs-lookup"><span data-stu-id="46351-138">The data type of the value.</span></span> <span data-ttu-id="46351-139">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="46351-139">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="46351-140">displayName</span><span class="sxs-lookup"><span data-stu-id="46351-140">displayName</span></span>|<span data-ttu-id="46351-141">String</span><span class="sxs-lookup"><span data-stu-id="46351-141">String</span></span>|<span data-ttu-id="46351-142">设置显示名称</span><span class="sxs-lookup"><span data-stu-id="46351-142">The setting's display name</span></span>|
|<span data-ttu-id="46351-143">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="46351-143">isTopLevel</span></span>|<span data-ttu-id="46351-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="46351-144">Boolean</span></span>|<span data-ttu-id="46351-145">如果设置是顶级设置，则无需封装在集合或复杂设置中即可进行配置</span><span class="sxs-lookup"><span data-stu-id="46351-145">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="46351-146">说明</span><span class="sxs-lookup"><span data-stu-id="46351-146">description</span></span>|<span data-ttu-id="46351-147">String</span><span class="sxs-lookup"><span data-stu-id="46351-147">String</span></span>|<span data-ttu-id="46351-148">设置的说明</span><span class="sxs-lookup"><span data-stu-id="46351-148">The setting's description</span></span>|
|<span data-ttu-id="46351-149">placeholderText</span><span class="sxs-lookup"><span data-stu-id="46351-149">placeholderText</span></span>|<span data-ttu-id="46351-150">String</span><span class="sxs-lookup"><span data-stu-id="46351-150">String</span></span>|<span data-ttu-id="46351-151">占位符文本作为有效输入的示例</span><span class="sxs-lookup"><span data-stu-id="46351-151">Placeholder text as an example of valid input</span></span>|
|<span data-ttu-id="46351-152">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="46351-152">documentationUrl</span></span>|<span data-ttu-id="46351-153">String</span><span class="sxs-lookup"><span data-stu-id="46351-153">String</span></span>|<span data-ttu-id="46351-154">设置文档的 URL</span><span class="sxs-lookup"><span data-stu-id="46351-154">Url to setting documentation</span></span>|
|<span data-ttu-id="46351-155">headerTitle</span><span class="sxs-lookup"><span data-stu-id="46351-155">headerTitle</span></span>|<span data-ttu-id="46351-156">String</span><span class="sxs-lookup"><span data-stu-id="46351-156">String</span></span>|<span data-ttu-id="46351-157">设置标头的标题表示设置/设置的类别/部分</span><span class="sxs-lookup"><span data-stu-id="46351-157">title of the setting header represents a category/section of a setting/settings</span></span>|
|<span data-ttu-id="46351-158">headerSubtitle</span><span class="sxs-lookup"><span data-stu-id="46351-158">headerSubtitle</span></span>|<span data-ttu-id="46351-159">String</span><span class="sxs-lookup"><span data-stu-id="46351-159">String</span></span>|<span data-ttu-id="46351-160">有关类别/节的更多详细信息，请参阅设置标题的副标题</span><span class="sxs-lookup"><span data-stu-id="46351-160">subtitle of the setting header for more details about the category/section</span></span>|
|<span data-ttu-id="46351-161">keywords</span><span class="sxs-lookup"><span data-stu-id="46351-161">keywords</span></span>|<span data-ttu-id="46351-162">String collection</span><span class="sxs-lookup"><span data-stu-id="46351-162">String collection</span></span>|<span data-ttu-id="46351-163">与设置关联的关键字</span><span class="sxs-lookup"><span data-stu-id="46351-163">Keywords associated with the setting</span></span>|
|<span data-ttu-id="46351-164">约束</span><span class="sxs-lookup"><span data-stu-id="46351-164">constraints</span></span>|<span data-ttu-id="46351-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46351-165">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="46351-166">设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="46351-166">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="46351-167">依赖项</span><span class="sxs-lookup"><span data-stu-id="46351-167">dependencies</span></span>|<span data-ttu-id="46351-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46351-168">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="46351-169">其他设置上依赖项的集合</span><span class="sxs-lookup"><span data-stu-id="46351-169">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="46351-170">响应</span><span class="sxs-lookup"><span data-stu-id="46351-170">Response</span></span>
<span data-ttu-id="46351-171">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46351-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46351-172">示例</span><span class="sxs-lookup"><span data-stu-id="46351-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="46351-173">请求</span><span class="sxs-lookup"><span data-stu-id="46351-173">Request</span></span>
<span data-ttu-id="46351-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46351-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 1014

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="46351-175">响应</span><span class="sxs-lookup"><span data-stu-id="46351-175">Response</span></span>
<span data-ttu-id="46351-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46351-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1063

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
  ]
}
```




