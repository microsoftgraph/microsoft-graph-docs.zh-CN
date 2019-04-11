---
title: 更新 deviceManagementSettingDefinition
description: 更新 deviceManagementSettingDefinition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f11167524956ff3eddc9a5508fb30fdd81e2aa73
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801454"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="e35aa-103">更新 deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="e35aa-103">Update deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="e35aa-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e35aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e35aa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e35aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e35aa-106">更新[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e35aa-106">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e35aa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e35aa-107">Prerequisites</span></span>
<span data-ttu-id="e35aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e35aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e35aa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e35aa-110">Permission type</span></span>|<span data-ttu-id="e35aa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e35aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e35aa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e35aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e35aa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e35aa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e35aa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e35aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e35aa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e35aa-115">Not supported.</span></span>|
|<span data-ttu-id="e35aa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e35aa-116">Application</span></span>|<span data-ttu-id="e35aa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e35aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e35aa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e35aa-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e35aa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e35aa-119">Request headers</span></span>
|<span data-ttu-id="e35aa-120">标头</span><span class="sxs-lookup"><span data-stu-id="e35aa-120">Header</span></span>|<span data-ttu-id="e35aa-121">值</span><span class="sxs-lookup"><span data-stu-id="e35aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e35aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e35aa-122">Authorization</span></span>|<span data-ttu-id="e35aa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e35aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e35aa-124">接受</span><span class="sxs-lookup"><span data-stu-id="e35aa-124">Accept</span></span>|<span data-ttu-id="e35aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e35aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e35aa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e35aa-126">Request body</span></span>
<span data-ttu-id="e35aa-127">在请求正文中, 提供[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e35aa-127">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="e35aa-128">下表显示创建[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e35aa-128">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="e35aa-129">属性</span><span class="sxs-lookup"><span data-stu-id="e35aa-129">Property</span></span>|<span data-ttu-id="e35aa-130">类型</span><span class="sxs-lookup"><span data-stu-id="e35aa-130">Type</span></span>|<span data-ttu-id="e35aa-131">说明</span><span class="sxs-lookup"><span data-stu-id="e35aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e35aa-132">id</span><span class="sxs-lookup"><span data-stu-id="e35aa-132">id</span></span>|<span data-ttu-id="e35aa-133">String</span><span class="sxs-lookup"><span data-stu-id="e35aa-133">String</span></span>|<span data-ttu-id="e35aa-134">设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="e35aa-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="e35aa-135">valueType</span><span class="sxs-lookup"><span data-stu-id="e35aa-135">valueType</span></span>|[<span data-ttu-id="e35aa-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="e35aa-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="e35aa-137">值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="e35aa-137">The data type of the value.</span></span> <span data-ttu-id="e35aa-138">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="e35aa-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="e35aa-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e35aa-139">displayName</span></span>|<span data-ttu-id="e35aa-140">String</span><span class="sxs-lookup"><span data-stu-id="e35aa-140">String</span></span>|<span data-ttu-id="e35aa-141">设置的显示名称</span><span class="sxs-lookup"><span data-stu-id="e35aa-141">The setting's display name</span></span>|
|<span data-ttu-id="e35aa-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="e35aa-142">isTopLevel</span></span>|<span data-ttu-id="e35aa-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="e35aa-143">Boolean</span></span>|<span data-ttu-id="e35aa-144">如果设置是顶级的, 则可以对其进行配置, 而无需将其包装在集合或复杂设置中</span><span class="sxs-lookup"><span data-stu-id="e35aa-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="e35aa-145">description</span><span class="sxs-lookup"><span data-stu-id="e35aa-145">description</span></span>|<span data-ttu-id="e35aa-146">String</span><span class="sxs-lookup"><span data-stu-id="e35aa-146">String</span></span>|<span data-ttu-id="e35aa-147">设置的说明</span><span class="sxs-lookup"><span data-stu-id="e35aa-147">The setting's description</span></span>|
|<span data-ttu-id="e35aa-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="e35aa-148">documentationUrl</span></span>|<span data-ttu-id="e35aa-149">String</span><span class="sxs-lookup"><span data-stu-id="e35aa-149">String</span></span>|<span data-ttu-id="e35aa-150">设置文档的 Url</span><span class="sxs-lookup"><span data-stu-id="e35aa-150">Url to setting documentation</span></span>|
|<span data-ttu-id="e35aa-151">keywords</span><span class="sxs-lookup"><span data-stu-id="e35aa-151">keywords</span></span>|<span data-ttu-id="e35aa-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="e35aa-152">String collection</span></span>|<span data-ttu-id="e35aa-153">与设置相关联的关键字</span><span class="sxs-lookup"><span data-stu-id="e35aa-153">Keywords associated with the setting</span></span>|
|<span data-ttu-id="e35aa-154">施加</span><span class="sxs-lookup"><span data-stu-id="e35aa-154">constraints</span></span>|<span data-ttu-id="e35aa-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="e35aa-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="e35aa-156">设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="e35aa-156">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="e35aa-157">依</span><span class="sxs-lookup"><span data-stu-id="e35aa-157">dependencies</span></span>|<span data-ttu-id="e35aa-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="e35aa-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="e35aa-159">对其他设置的依赖项的集合</span><span class="sxs-lookup"><span data-stu-id="e35aa-159">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="e35aa-160">响应</span><span class="sxs-lookup"><span data-stu-id="e35aa-160">Response</span></span>
<span data-ttu-id="e35aa-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e35aa-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e35aa-162">示例</span><span class="sxs-lookup"><span data-stu-id="e35aa-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e35aa-163">请求</span><span class="sxs-lookup"><span data-stu-id="e35aa-163">Request</span></span>
<span data-ttu-id="e35aa-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e35aa-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="e35aa-165">响应</span><span class="sxs-lookup"><span data-stu-id="e35aa-165">Response</span></span>
<span data-ttu-id="e35aa-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e35aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
  ]
}
```





