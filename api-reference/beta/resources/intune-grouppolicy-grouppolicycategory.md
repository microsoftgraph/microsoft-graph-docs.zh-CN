---
title: groupPolicyCategory 资源类型
description: Category 实体存储组策略定义的类别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b754020cc4a7c4f7e9fdf7cc35f74d9dcc4c4c1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783121"
---
# <a name="grouppolicycategory-resource-type"></a><span data-ttu-id="c0288-103">groupPolicyCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0288-103">groupPolicyCategory resource type</span></span>

> <span data-ttu-id="c0288-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0288-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0288-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0288-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0288-106">Category 实体存储组策略定义的类别</span><span class="sxs-lookup"><span data-stu-id="c0288-106">The category entity stores the category of a group policy definition</span></span>

## <a name="methods"></a><span data-ttu-id="c0288-107">方法</span><span class="sxs-lookup"><span data-stu-id="c0288-107">Methods</span></span>
|<span data-ttu-id="c0288-108">方法</span><span class="sxs-lookup"><span data-stu-id="c0288-108">Method</span></span>|<span data-ttu-id="c0288-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c0288-109">Return Type</span></span>|<span data-ttu-id="c0288-110">说明</span><span class="sxs-lookup"><span data-stu-id="c0288-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0288-111">获取 groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="c0288-111">Get groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-get.md)|[<span data-ttu-id="c0288-112">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="c0288-112">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="c0288-113">读取[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0288-113">Read properties and relationships of the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|
|[<span data-ttu-id="c0288-114">更新 groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="c0288-114">Update groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-update.md)|[<span data-ttu-id="c0288-115">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="c0288-115">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="c0288-116">更新[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c0288-116">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0288-117">属性</span><span class="sxs-lookup"><span data-stu-id="c0288-117">Properties</span></span>
|<span data-ttu-id="c0288-118">属性</span><span class="sxs-lookup"><span data-stu-id="c0288-118">Property</span></span>|<span data-ttu-id="c0288-119">类型</span><span class="sxs-lookup"><span data-stu-id="c0288-119">Type</span></span>|<span data-ttu-id="c0288-120">说明</span><span class="sxs-lookup"><span data-stu-id="c0288-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0288-121">displayName</span><span class="sxs-lookup"><span data-stu-id="c0288-121">displayName</span></span>|<span data-ttu-id="c0288-122">String</span><span class="sxs-lookup"><span data-stu-id="c0288-122">String</span></span>|<span data-ttu-id="c0288-123">类别的显示名称的字符串 id</span><span class="sxs-lookup"><span data-stu-id="c0288-123">The string id of the category's display name</span></span>|
|<span data-ttu-id="c0288-124">isRoot</span><span class="sxs-lookup"><span data-stu-id="c0288-124">isRoot</span></span>|<span data-ttu-id="c0288-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="c0288-125">Boolean</span></span>|<span data-ttu-id="c0288-126">定义类别是否为根类别</span><span class="sxs-lookup"><span data-stu-id="c0288-126">Defines if the category is a root category</span></span>|
|<span data-ttu-id="c0288-127">id</span><span class="sxs-lookup"><span data-stu-id="c0288-127">id</span></span>|<span data-ttu-id="c0288-128">String</span><span class="sxs-lookup"><span data-stu-id="c0288-128">String</span></span>|<span data-ttu-id="c0288-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c0288-129">Key of the entity.</span></span>|
|<span data-ttu-id="c0288-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0288-130">lastModifiedDateTime</span></span>|<span data-ttu-id="c0288-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0288-131">DateTimeOffset</span></span>|<span data-ttu-id="c0288-132">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c0288-132">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0288-133">关系</span><span class="sxs-lookup"><span data-stu-id="c0288-133">Relationships</span></span>
|<span data-ttu-id="c0288-134">关系</span><span class="sxs-lookup"><span data-stu-id="c0288-134">Relationship</span></span>|<span data-ttu-id="c0288-135">类型</span><span class="sxs-lookup"><span data-stu-id="c0288-135">Type</span></span>|<span data-ttu-id="c0288-136">说明</span><span class="sxs-lookup"><span data-stu-id="c0288-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0288-137">母语</span><span class="sxs-lookup"><span data-stu-id="c0288-137">parent</span></span>|[<span data-ttu-id="c0288-138">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="c0288-138">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="c0288-139">父类别</span><span class="sxs-lookup"><span data-stu-id="c0288-139">The parent category</span></span>|
|<span data-ttu-id="c0288-140">children</span><span class="sxs-lookup"><span data-stu-id="c0288-140">children</span></span>|<span data-ttu-id="c0288-141">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0288-141">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) collection</span></span>|<span data-ttu-id="c0288-142">子类别</span><span class="sxs-lookup"><span data-stu-id="c0288-142">The children categories</span></span>|
|<span data-ttu-id="c0288-143">限定</span><span class="sxs-lookup"><span data-stu-id="c0288-143">definitions</span></span>|<span data-ttu-id="c0288-144">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0288-144">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="c0288-145">类别的直接 GroupPolicyDefinition 子类别</span><span class="sxs-lookup"><span data-stu-id="c0288-145">The immediate GroupPolicyDefinition children of the category</span></span>|
|<span data-ttu-id="c0288-146">definitionFile</span><span class="sxs-lookup"><span data-stu-id="c0288-146">definitionFile</span></span>|[<span data-ttu-id="c0288-147">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="c0288-147">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="c0288-148">类别所属的定义文件的 id</span><span class="sxs-lookup"><span data-stu-id="c0288-148">The id of the definition file the category came from</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0288-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0288-149">JSON Representation</span></span>
<span data-ttu-id="c0288-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0288-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



