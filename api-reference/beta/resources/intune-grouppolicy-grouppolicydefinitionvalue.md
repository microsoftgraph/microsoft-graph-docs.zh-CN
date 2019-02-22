---
title: groupPolicyDefinitionValue 资源类型
description: "\"定义值\" 实体存储单个组策略定义的值。"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e822cb4ce46a0fa9492f7624904588fd1b10a7c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142614"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a><span data-ttu-id="e3d98-103">groupPolicyDefinitionValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3d98-103">groupPolicyDefinitionValue resource type</span></span>

> <span data-ttu-id="e3d98-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3d98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3d98-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3d98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3d98-106">"定义值" 实体存储单个组策略定义的值。</span><span class="sxs-lookup"><span data-stu-id="e3d98-106">The definition value entity stores the value for a single group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="e3d98-107">方法</span><span class="sxs-lookup"><span data-stu-id="e3d98-107">Methods</span></span>
|<span data-ttu-id="e3d98-108">方法</span><span class="sxs-lookup"><span data-stu-id="e3d98-108">Method</span></span>|<span data-ttu-id="e3d98-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3d98-109">Return Type</span></span>|<span data-ttu-id="e3d98-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3d98-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3d98-111">列出 groupPolicyDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="e3d98-111">List groupPolicyDefinitionValues</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|<span data-ttu-id="e3d98-112">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3d98-112">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="e3d98-113">列出[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3d98-113">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>|
|[<span data-ttu-id="e3d98-114">获取 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e3d98-114">Get groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[<span data-ttu-id="e3d98-115">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e3d98-115">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="e3d98-116">读取[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3d98-116">Read properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="e3d98-117">创建 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e3d98-117">Create groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[<span data-ttu-id="e3d98-118">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e3d98-118">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="e3d98-119">创建新的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3d98-119">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="e3d98-120">删除 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e3d98-120">Delete groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|<span data-ttu-id="e3d98-121">无</span><span class="sxs-lookup"><span data-stu-id="e3d98-121">None</span></span>|<span data-ttu-id="e3d98-122">删除[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="e3d98-122">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>|
|[<span data-ttu-id="e3d98-123">更新 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e3d98-123">Update groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[<span data-ttu-id="e3d98-124">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="e3d98-124">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="e3d98-125">更新[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e3d98-125">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3d98-126">属性</span><span class="sxs-lookup"><span data-stu-id="e3d98-126">Properties</span></span>
|<span data-ttu-id="e3d98-127">属性</span><span class="sxs-lookup"><span data-stu-id="e3d98-127">Property</span></span>|<span data-ttu-id="e3d98-128">类型</span><span class="sxs-lookup"><span data-stu-id="e3d98-128">Type</span></span>|<span data-ttu-id="e3d98-129">说明</span><span class="sxs-lookup"><span data-stu-id="e3d98-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d98-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3d98-130">createdDateTime</span></span>|<span data-ttu-id="e3d98-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3d98-131">DateTimeOffset</span></span>|<span data-ttu-id="e3d98-132">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e3d98-132">The date and time the object was created.</span></span>|
|<span data-ttu-id="e3d98-133">enabled</span><span class="sxs-lookup"><span data-stu-id="e3d98-133">enabled</span></span>|<span data-ttu-id="e3d98-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3d98-134">Boolean</span></span>|<span data-ttu-id="e3d98-135">启用或禁用关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="e3d98-135">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="e3d98-136">configurationType</span><span class="sxs-lookup"><span data-stu-id="e3d98-136">configurationType</span></span>|[<span data-ttu-id="e3d98-137">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="e3d98-137">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="e3d98-138">指定应如何配置值。</span><span class="sxs-lookup"><span data-stu-id="e3d98-138">Specifies how the value should be configured.</span></span> <span data-ttu-id="e3d98-139">这可以是策略, 也可以是首选项。</span><span class="sxs-lookup"><span data-stu-id="e3d98-139">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="e3d98-140">可取值为：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="e3d98-140">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="e3d98-141">id</span><span class="sxs-lookup"><span data-stu-id="e3d98-141">id</span></span>|<span data-ttu-id="e3d98-142">String</span><span class="sxs-lookup"><span data-stu-id="e3d98-142">String</span></span>|<span data-ttu-id="e3d98-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e3d98-143">Key of the entity.</span></span>|
|<span data-ttu-id="e3d98-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3d98-144">lastModifiedDateTime</span></span>|<span data-ttu-id="e3d98-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3d98-145">DateTimeOffset</span></span>|<span data-ttu-id="e3d98-146">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e3d98-146">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3d98-147">关系</span><span class="sxs-lookup"><span data-stu-id="e3d98-147">Relationships</span></span>
|<span data-ttu-id="e3d98-148">关系</span><span class="sxs-lookup"><span data-stu-id="e3d98-148">Relationship</span></span>|<span data-ttu-id="e3d98-149">类型</span><span class="sxs-lookup"><span data-stu-id="e3d98-149">Type</span></span>|<span data-ttu-id="e3d98-150">说明</span><span class="sxs-lookup"><span data-stu-id="e3d98-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d98-151">presentationValues</span><span class="sxs-lookup"><span data-stu-id="e3d98-151">presentationValues</span></span>|<span data-ttu-id="e3d98-152">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3d98-152">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="e3d98-153">与定义值关联的组策略呈现值值。</span><span class="sxs-lookup"><span data-stu-id="e3d98-153">The associated group policy presentation values with the definition value.</span></span>|
|<span data-ttu-id="e3d98-154">definition</span><span class="sxs-lookup"><span data-stu-id="e3d98-154">definition</span></span>|[<span data-ttu-id="e3d98-155">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="e3d98-155">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="e3d98-156">与值关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="e3d98-156">The associated group policy definition with the value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3d98-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3d98-157">JSON Representation</span></span>
<span data-ttu-id="e3d98-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3d98-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




