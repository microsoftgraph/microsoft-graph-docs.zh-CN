---
title: deviceManagementSettingDefinition 资源类型
description: 表示给定设置的定义的实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a37046b80ce51a698ba52f08c2693af821b7e52
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524482"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a><span data-ttu-id="69092-103">deviceManagementSettingDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="69092-103">deviceManagementSettingDefinition resource type</span></span>

> <span data-ttu-id="69092-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69092-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69092-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69092-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69092-106">表示给定设置的定义的实体</span><span class="sxs-lookup"><span data-stu-id="69092-106">Entity representing the defintion for a given setting</span></span>

## <a name="methods"></a><span data-ttu-id="69092-107">方法</span><span class="sxs-lookup"><span data-stu-id="69092-107">Methods</span></span>
|<span data-ttu-id="69092-108">方法</span><span class="sxs-lookup"><span data-stu-id="69092-108">Method</span></span>|<span data-ttu-id="69092-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="69092-109">Return Type</span></span>|<span data-ttu-id="69092-110">说明</span><span class="sxs-lookup"><span data-stu-id="69092-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69092-111">列出 deviceManagementSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="69092-111">List deviceManagementSettingDefinitions</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|<span data-ttu-id="69092-112">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="69092-112">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="69092-113">列出[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69092-113">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>|
|[<span data-ttu-id="69092-114">获取 deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="69092-114">Get deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[<span data-ttu-id="69092-115">deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="69092-115">deviceManagementSettingDefinition</span></span>](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|<span data-ttu-id="69092-116">读取[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69092-116">Read properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>|
|[<span data-ttu-id="69092-117">创建 deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="69092-117">Create deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[<span data-ttu-id="69092-118">deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="69092-118">deviceManagementSettingDefinition</span></span>](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|<span data-ttu-id="69092-119">创建新的[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69092-119">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>|
|[<span data-ttu-id="69092-120">删除 deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="69092-120">Delete deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|<span data-ttu-id="69092-121">无</span><span class="sxs-lookup"><span data-stu-id="69092-121">None</span></span>|<span data-ttu-id="69092-122">删除[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="69092-122">Deletes a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>|
|[<span data-ttu-id="69092-123">更新 deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="69092-123">Update deviceManagementSettingDefinition</span></span>](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[<span data-ttu-id="69092-124">deviceManagementSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="69092-124">deviceManagementSettingDefinition</span></span>](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|<span data-ttu-id="69092-125">更新[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69092-125">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69092-126">属性</span><span class="sxs-lookup"><span data-stu-id="69092-126">Properties</span></span>
|<span data-ttu-id="69092-127">属性</span><span class="sxs-lookup"><span data-stu-id="69092-127">Property</span></span>|<span data-ttu-id="69092-128">类型</span><span class="sxs-lookup"><span data-stu-id="69092-128">Type</span></span>|<span data-ttu-id="69092-129">说明</span><span class="sxs-lookup"><span data-stu-id="69092-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69092-130">id</span><span class="sxs-lookup"><span data-stu-id="69092-130">id</span></span>|<span data-ttu-id="69092-131">String</span><span class="sxs-lookup"><span data-stu-id="69092-131">String</span></span>|<span data-ttu-id="69092-132">设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="69092-132">The ID of the setting definition</span></span>|
|<span data-ttu-id="69092-133">valueType</span><span class="sxs-lookup"><span data-stu-id="69092-133">valueType</span></span>|[<span data-ttu-id="69092-134">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="69092-134">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="69092-135">值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="69092-135">The data type of the value.</span></span> <span data-ttu-id="69092-136">可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="69092-136">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="69092-137">displayName</span><span class="sxs-lookup"><span data-stu-id="69092-137">displayName</span></span>|<span data-ttu-id="69092-138">String</span><span class="sxs-lookup"><span data-stu-id="69092-138">String</span></span>|<span data-ttu-id="69092-139">设置的显示名称</span><span class="sxs-lookup"><span data-stu-id="69092-139">The setting's display name</span></span>|
|<span data-ttu-id="69092-140">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="69092-140">isTopLevel</span></span>|<span data-ttu-id="69092-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="69092-141">Boolean</span></span>|<span data-ttu-id="69092-142">如果设置是顶级的, 则可以对其进行配置, 而无需将其包装在集合或复杂设置中</span><span class="sxs-lookup"><span data-stu-id="69092-142">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="69092-143">description</span><span class="sxs-lookup"><span data-stu-id="69092-143">description</span></span>|<span data-ttu-id="69092-144">String</span><span class="sxs-lookup"><span data-stu-id="69092-144">String</span></span>|<span data-ttu-id="69092-145">设置的说明</span><span class="sxs-lookup"><span data-stu-id="69092-145">The setting's description</span></span>|
|<span data-ttu-id="69092-146">documentationUrl</span><span class="sxs-lookup"><span data-stu-id="69092-146">documentationUrl</span></span>|<span data-ttu-id="69092-147">String</span><span class="sxs-lookup"><span data-stu-id="69092-147">String</span></span>|<span data-ttu-id="69092-148">设置文档的 Url</span><span class="sxs-lookup"><span data-stu-id="69092-148">Url to setting documentation</span></span>|
|<span data-ttu-id="69092-149">keywords</span><span class="sxs-lookup"><span data-stu-id="69092-149">keywords</span></span>|<span data-ttu-id="69092-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="69092-150">String collection</span></span>|<span data-ttu-id="69092-151">与设置相关联的关键字</span><span class="sxs-lookup"><span data-stu-id="69092-151">Keywords associated with the setting</span></span>|
|<span data-ttu-id="69092-152">施加</span><span class="sxs-lookup"><span data-stu-id="69092-152">constraints</span></span>|<span data-ttu-id="69092-153">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="69092-153">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="69092-154">设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="69092-154">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="69092-155">依</span><span class="sxs-lookup"><span data-stu-id="69092-155">dependencies</span></span>|<span data-ttu-id="69092-156">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="69092-156">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="69092-157">对其他设置的依赖项的集合</span><span class="sxs-lookup"><span data-stu-id="69092-157">Collection of dependencies on other settings</span></span>|

## <a name="relationships"></a><span data-ttu-id="69092-158">关系</span><span class="sxs-lookup"><span data-stu-id="69092-158">Relationships</span></span>
<span data-ttu-id="69092-159">无</span><span class="sxs-lookup"><span data-stu-id="69092-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69092-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69092-160">JSON Representation</span></span>
<span data-ttu-id="69092-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69092-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```







