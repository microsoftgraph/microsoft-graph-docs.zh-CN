---
title: 更新 deviceManagementAbstractComplexSettingDefinition
description: 更新 deviceManagementAbstractComplexSettingDefinition 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a01cd287d5616e8cdc1bc29a383e2fc5b9cb9db4
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522683"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="5fd49-103">更新 deviceManagementAbstractComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="5fd49-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="5fd49-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5fd49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fd49-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fd49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fd49-106">更新[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5fd49-106">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fd49-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5fd49-107">Prerequisites</span></span>
<span data-ttu-id="5fd49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5fd49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fd49-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fd49-110">Permission type</span></span>|<span data-ttu-id="5fd49-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5fd49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fd49-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fd49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5fd49-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fd49-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fd49-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fd49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fd49-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fd49-115">Not supported.</span></span>|
|<span data-ttu-id="5fd49-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fd49-116">Application</span></span>|<span data-ttu-id="5fd49-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fd49-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fd49-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fd49-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5fd49-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fd49-119">Request headers</span></span>
|<span data-ttu-id="5fd49-120">标头</span><span class="sxs-lookup"><span data-stu-id="5fd49-120">Header</span></span>|<span data-ttu-id="5fd49-121">值</span><span class="sxs-lookup"><span data-stu-id="5fd49-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fd49-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fd49-122">Authorization</span></span>|<span data-ttu-id="5fd49-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5fd49-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fd49-124">接受</span><span class="sxs-lookup"><span data-stu-id="5fd49-124">Accept</span></span>|<span data-ttu-id="5fd49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5fd49-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fd49-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fd49-126">Request body</span></span>
<span data-ttu-id="5fd49-127">在请求正文中, 提供[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fd49-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="5fd49-128">下表显示创建[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5fd49-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="5fd49-129">属性</span><span class="sxs-lookup"><span data-stu-id="5fd49-129">Property</span></span>|<span data-ttu-id="5fd49-130">类型</span><span class="sxs-lookup"><span data-stu-id="5fd49-130">Type</span></span>|<span data-ttu-id="5fd49-131">说明</span><span class="sxs-lookup"><span data-stu-id="5fd49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fd49-132">id</span><span class="sxs-lookup"><span data-stu-id="5fd49-132">id</span></span>|<span data-ttu-id="5fd49-133">String</span><span class="sxs-lookup"><span data-stu-id="5fd49-133">String</span></span>|<span data-ttu-id="5fd49-134">从[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="5fd49-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-135">valueType</span><span class="sxs-lookup"><span data-stu-id="5fd49-135">valueType</span></span>|[<span data-ttu-id="5fd49-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="5fd49-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="5fd49-137">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="5fd49-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="5fd49-138">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="5fd49-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="5fd49-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5fd49-139">displayName</span></span>|<span data-ttu-id="5fd49-140">String</span><span class="sxs-lookup"><span data-stu-id="5fd49-140">String</span></span>|<span data-ttu-id="5fd49-141">设置的显示名称继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5fd49-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="5fd49-142">isTopLevel</span></span>|<span data-ttu-id="5fd49-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fd49-143">Boolean</span></span>|<span data-ttu-id="5fd49-144">如果设置是顶级的, 则可以对其进行配置, 而无需将其包装在从[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。</span><span class="sxs-lookup"><span data-stu-id="5fd49-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-145">description</span><span class="sxs-lookup"><span data-stu-id="5fd49-145">description</span></span>|<span data-ttu-id="5fd49-146">String</span><span class="sxs-lookup"><span data-stu-id="5fd49-146">String</span></span>|<span data-ttu-id="5fd49-147">该设置的说明继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5fd49-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-148">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="5fd49-148">documentationUrl</span></span>|<span data-ttu-id="5fd49-149">String</span><span class="sxs-lookup"><span data-stu-id="5fd49-149">String</span></span>|<span data-ttu-id="5fd49-150">设置从[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url</span><span class="sxs-lookup"><span data-stu-id="5fd49-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-151">keywords</span><span class="sxs-lookup"><span data-stu-id="5fd49-151">keywords</span></span>|<span data-ttu-id="5fd49-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="5fd49-152">String collection</span></span>|<span data-ttu-id="5fd49-153">与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字</span><span class="sxs-lookup"><span data-stu-id="5fd49-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-154">施加</span><span class="sxs-lookup"><span data-stu-id="5fd49-154">constraints</span></span>|<span data-ttu-id="5fd49-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="5fd49-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="5fd49-156">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="5fd49-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-157">依</span><span class="sxs-lookup"><span data-stu-id="5fd49-157">dependencies</span></span>|<span data-ttu-id="5fd49-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="5fd49-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="5fd49-159">继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合</span><span class="sxs-lookup"><span data-stu-id="5fd49-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="5fd49-160">60,000</span><span class="sxs-lookup"><span data-stu-id="5fd49-160">implementations</span></span>|<span data-ttu-id="5fd49-161">String 集合</span><span class="sxs-lookup"><span data-stu-id="5fd49-161">String collection</span></span>|<span data-ttu-id="5fd49-162">此抽象复杂设置的所有可能实现的定义 id 的列表</span><span class="sxs-lookup"><span data-stu-id="5fd49-162">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="5fd49-163">响应</span><span class="sxs-lookup"><span data-stu-id="5fd49-163">Response</span></span>
<span data-ttu-id="5fd49-164">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5fd49-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fd49-165">示例</span><span class="sxs-lookup"><span data-stu-id="5fd49-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fd49-166">请求</span><span class="sxs-lookup"><span data-stu-id="5fd49-166">Request</span></span>
<span data-ttu-id="5fd49-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5fd49-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 802

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5fd49-168">响应</span><span class="sxs-lookup"><span data-stu-id="5fd49-168">Response</span></span>
<span data-ttu-id="5fd49-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fd49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 851

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
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
  "implementations": [
    "Implementations value"
  ]
}
```







