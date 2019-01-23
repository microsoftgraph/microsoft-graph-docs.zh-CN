---
title: groupPolicyPresentationValueList 资源类型
description: 实体表示策略定义上的列表框演示文稿的名称/值对的集合。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a4ea5193edbf58a54da86f9478bfe9a51010d5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429479"
---
# <a name="grouppolicypresentationvaluelist-resource-type"></a><span data-ttu-id="b77d5-103">groupPolicyPresentationValueList 资源类型</span><span class="sxs-lookup"><span data-stu-id="b77d5-103">groupPolicyPresentationValueList resource type</span></span>

> <span data-ttu-id="b77d5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b77d5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b77d5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b77d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b77d5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b77d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b77d5-107">实体表示策略定义上的列表框演示文稿的名称/值对的集合。</span><span class="sxs-lookup"><span data-stu-id="b77d5-107">The entity represents a collection of name/value pairs of a list box presentation on a policy definition.</span></span>


<span data-ttu-id="b77d5-108">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b77d5-108">Inherits from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b77d5-109">方法</span><span class="sxs-lookup"><span data-stu-id="b77d5-109">Methods</span></span>
|<span data-ttu-id="b77d5-110">方法</span><span class="sxs-lookup"><span data-stu-id="b77d5-110">Method</span></span>|<span data-ttu-id="b77d5-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b77d5-111">Return Type</span></span>|<span data-ttu-id="b77d5-112">说明</span><span class="sxs-lookup"><span data-stu-id="b77d5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b77d5-113">列表 groupPolicyPresentationValueLists</span><span class="sxs-lookup"><span data-stu-id="b77d5-113">List groupPolicyPresentationValueLists</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-list.md)|<span data-ttu-id="b77d5-114">[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)集合</span><span class="sxs-lookup"><span data-stu-id="b77d5-114">[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) collection</span></span>|<span data-ttu-id="b77d5-115">列出属性和[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="b77d5-115">List properties and relationships of the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) objects.</span></span>|
|[<span data-ttu-id="b77d5-116">获取 groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b77d5-116">Get groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-get.md)|[<span data-ttu-id="b77d5-117">groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b77d5-117">groupPolicyPresentationValueList</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|<span data-ttu-id="b77d5-118">读取属性和[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="b77d5-118">Read properties and relationships of the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>|
|[<span data-ttu-id="b77d5-119">创建 groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b77d5-119">Create groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-create.md)|[<span data-ttu-id="b77d5-120">groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b77d5-120">groupPolicyPresentationValueList</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|<span data-ttu-id="b77d5-121">创建新的[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b77d5-121">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>|
|[<span data-ttu-id="b77d5-122">删除 groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b77d5-122">Delete groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-delete.md)|<span data-ttu-id="b77d5-123">无</span><span class="sxs-lookup"><span data-stu-id="b77d5-123">None</span></span>|<span data-ttu-id="b77d5-124">删除[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)。</span><span class="sxs-lookup"><span data-stu-id="b77d5-124">Deletes a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>|
|[<span data-ttu-id="b77d5-125">更新 groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b77d5-125">Update groupPolicyPresentationValueList</span></span>](../api/intune-grouppolicy-grouppolicypresentationvaluelist-update.md)|[<span data-ttu-id="b77d5-126">groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="b77d5-126">groupPolicyPresentationValueList</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|<span data-ttu-id="b77d5-127">更新[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b77d5-127">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b77d5-128">属性</span><span class="sxs-lookup"><span data-stu-id="b77d5-128">Properties</span></span>
|<span data-ttu-id="b77d5-129">属性</span><span class="sxs-lookup"><span data-stu-id="b77d5-129">Property</span></span>|<span data-ttu-id="b77d5-130">类型</span><span class="sxs-lookup"><span data-stu-id="b77d5-130">Type</span></span>|<span data-ttu-id="b77d5-131">说明</span><span class="sxs-lookup"><span data-stu-id="b77d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b77d5-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b77d5-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b77d5-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b77d5-133">DateTimeOffset</span></span>|<span data-ttu-id="b77d5-134">日期和时间上次修改对象。</span><span class="sxs-lookup"><span data-stu-id="b77d5-134">The date and time the object was last modified.</span></span> <span data-ttu-id="b77d5-135">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b77d5-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b77d5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b77d5-136">createdDateTime</span></span>|<span data-ttu-id="b77d5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b77d5-137">DateTimeOffset</span></span>|<span data-ttu-id="b77d5-138">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="b77d5-138">The date and time the object was created.</span></span> <span data-ttu-id="b77d5-139">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b77d5-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b77d5-140">id</span><span class="sxs-lookup"><span data-stu-id="b77d5-140">id</span></span>|<span data-ttu-id="b77d5-141">String</span><span class="sxs-lookup"><span data-stu-id="b77d5-141">String</span></span>|<span data-ttu-id="b77d5-142">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b77d5-142">Key of the entity.</span></span> <span data-ttu-id="b77d5-143">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b77d5-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b77d5-144">values</span><span class="sxs-lookup"><span data-stu-id="b77d5-144">values</span></span>|<span data-ttu-id="b77d5-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b77d5-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b77d5-146">对关联的演示文稿的列表。</span><span class="sxs-lookup"><span data-stu-id="b77d5-146">A list of pairs for the associated presentation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b77d5-147">关系</span><span class="sxs-lookup"><span data-stu-id="b77d5-147">Relationships</span></span>
|<span data-ttu-id="b77d5-148">关系</span><span class="sxs-lookup"><span data-stu-id="b77d5-148">Relationship</span></span>|<span data-ttu-id="b77d5-149">类型</span><span class="sxs-lookup"><span data-stu-id="b77d5-149">Type</span></span>|<span data-ttu-id="b77d5-150">说明</span><span class="sxs-lookup"><span data-stu-id="b77d5-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b77d5-151">definitionValue</span><span class="sxs-lookup"><span data-stu-id="b77d5-151">definitionValue</span></span>|[<span data-ttu-id="b77d5-152">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="b77d5-152">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="b77d5-153">关联的演示文稿值的组策略定义值。</span><span class="sxs-lookup"><span data-stu-id="b77d5-153">The group policy definition value associated with the presentation value.</span></span> <span data-ttu-id="b77d5-154">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b77d5-154">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b77d5-155">演示文稿</span><span class="sxs-lookup"><span data-stu-id="b77d5-155">presentation</span></span>|[<span data-ttu-id="b77d5-156">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="b77d5-156">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="b77d5-157">组策略演示的演示文稿值相关联。</span><span class="sxs-lookup"><span data-stu-id="b77d5-157">The group policy presentation associated with the presentation value.</span></span> <span data-ttu-id="b77d5-158">继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b77d5-158">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b77d5-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b77d5-159">JSON Representation</span></span>
<span data-ttu-id="b77d5-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b77d5-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




