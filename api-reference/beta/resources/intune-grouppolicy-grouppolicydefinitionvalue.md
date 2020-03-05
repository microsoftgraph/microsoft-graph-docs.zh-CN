---
title: groupPolicyDefinitionValue 资源类型
description: "\"定义值\" 实体存储单个组策略定义的值。"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9ad80f427061da8813f3d63f0cfc1be424c27f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524446"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a><span data-ttu-id="5c237-103">groupPolicyDefinitionValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c237-103">groupPolicyDefinitionValue resource type</span></span>

<span data-ttu-id="5c237-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5c237-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c237-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c237-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c237-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c237-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c237-107">"定义值" 实体存储单个组策略定义的值。</span><span class="sxs-lookup"><span data-stu-id="5c237-107">The definition value entity stores the value for a single group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="5c237-108">方法</span><span class="sxs-lookup"><span data-stu-id="5c237-108">Methods</span></span>
|<span data-ttu-id="5c237-109">方法</span><span class="sxs-lookup"><span data-stu-id="5c237-109">Method</span></span>|<span data-ttu-id="5c237-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5c237-110">Return Type</span></span>|<span data-ttu-id="5c237-111">说明</span><span class="sxs-lookup"><span data-stu-id="5c237-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c237-112">列出 groupPolicyDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="5c237-112">List groupPolicyDefinitionValues</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|<span data-ttu-id="5c237-113">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c237-113">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="5c237-114">列出[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c237-114">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>|
|[<span data-ttu-id="5c237-115">获取 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5c237-115">Get groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[<span data-ttu-id="5c237-116">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5c237-116">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="5c237-117">读取[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c237-117">Read properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="5c237-118">创建 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5c237-118">Create groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[<span data-ttu-id="5c237-119">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5c237-119">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="5c237-120">创建新的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5c237-120">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="5c237-121">删除 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5c237-121">Delete groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|<span data-ttu-id="5c237-122">无</span><span class="sxs-lookup"><span data-stu-id="5c237-122">None</span></span>|<span data-ttu-id="5c237-123">删除[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="5c237-123">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>|
|[<span data-ttu-id="5c237-124">更新 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5c237-124">Update groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[<span data-ttu-id="5c237-125">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5c237-125">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="5c237-126">更新[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5c237-126">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c237-127">属性</span><span class="sxs-lookup"><span data-stu-id="5c237-127">Properties</span></span>
|<span data-ttu-id="5c237-128">属性</span><span class="sxs-lookup"><span data-stu-id="5c237-128">Property</span></span>|<span data-ttu-id="5c237-129">类型</span><span class="sxs-lookup"><span data-stu-id="5c237-129">Type</span></span>|<span data-ttu-id="5c237-130">说明</span><span class="sxs-lookup"><span data-stu-id="5c237-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c237-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c237-131">createdDateTime</span></span>|<span data-ttu-id="5c237-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c237-132">DateTimeOffset</span></span>|<span data-ttu-id="5c237-133">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5c237-133">The date and time the object was created.</span></span>|
|<span data-ttu-id="5c237-134">enabled</span><span class="sxs-lookup"><span data-stu-id="5c237-134">enabled</span></span>|<span data-ttu-id="5c237-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c237-135">Boolean</span></span>|<span data-ttu-id="5c237-136">启用或禁用关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="5c237-136">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="5c237-137">configurationType</span><span class="sxs-lookup"><span data-stu-id="5c237-137">configurationType</span></span>|[<span data-ttu-id="5c237-138">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="5c237-138">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="5c237-139">指定应如何配置值。</span><span class="sxs-lookup"><span data-stu-id="5c237-139">Specifies how the value should be configured.</span></span> <span data-ttu-id="5c237-140">这可以是策略，也可以是首选项。</span><span class="sxs-lookup"><span data-stu-id="5c237-140">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="5c237-141">可能的值是：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="5c237-141">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="5c237-142">id</span><span class="sxs-lookup"><span data-stu-id="5c237-142">id</span></span>|<span data-ttu-id="5c237-143">String</span><span class="sxs-lookup"><span data-stu-id="5c237-143">String</span></span>|<span data-ttu-id="5c237-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5c237-144">Key of the entity.</span></span>|
|<span data-ttu-id="5c237-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c237-145">lastModifiedDateTime</span></span>|<span data-ttu-id="5c237-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c237-146">DateTimeOffset</span></span>|<span data-ttu-id="5c237-147">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5c237-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c237-148">关系</span><span class="sxs-lookup"><span data-stu-id="5c237-148">Relationships</span></span>
|<span data-ttu-id="5c237-149">关系</span><span class="sxs-lookup"><span data-stu-id="5c237-149">Relationship</span></span>|<span data-ttu-id="5c237-150">类型</span><span class="sxs-lookup"><span data-stu-id="5c237-150">Type</span></span>|<span data-ttu-id="5c237-151">说明</span><span class="sxs-lookup"><span data-stu-id="5c237-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c237-152">presentationValues</span><span class="sxs-lookup"><span data-stu-id="5c237-152">presentationValues</span></span>|<span data-ttu-id="5c237-153">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="5c237-153">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="5c237-154">与定义值关联的组策略呈现值值。</span><span class="sxs-lookup"><span data-stu-id="5c237-154">The associated group policy presentation values with the definition value.</span></span>|
|<span data-ttu-id="5c237-155">定义</span><span class="sxs-lookup"><span data-stu-id="5c237-155">definition</span></span>|[<span data-ttu-id="5c237-156">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="5c237-156">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="5c237-157">与值关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="5c237-157">The associated group policy definition with the value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c237-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c237-158">JSON Representation</span></span>
<span data-ttu-id="5c237-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c237-159">Here is a JSON representation of the resource.</span></span>
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



