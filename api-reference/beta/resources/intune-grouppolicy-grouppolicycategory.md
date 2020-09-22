---
title: groupPolicyCategory 资源类型
description: Category 实体存储组策略定义的类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc4eed4c7450c8e6803d4cd064a26c7b4919ea95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031093"
---
# <a name="grouppolicycategory-resource-type"></a><span data-ttu-id="db0ba-103">groupPolicyCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="db0ba-103">groupPolicyCategory resource type</span></span>

<span data-ttu-id="db0ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db0ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db0ba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db0ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db0ba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db0ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db0ba-107">Category 实体存储组策略定义的类别</span><span class="sxs-lookup"><span data-stu-id="db0ba-107">The category entity stores the category of a group policy definition</span></span>

## <a name="methods"></a><span data-ttu-id="db0ba-108">方法</span><span class="sxs-lookup"><span data-stu-id="db0ba-108">Methods</span></span>
|<span data-ttu-id="db0ba-109">方法</span><span class="sxs-lookup"><span data-stu-id="db0ba-109">Method</span></span>|<span data-ttu-id="db0ba-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="db0ba-110">Return Type</span></span>|<span data-ttu-id="db0ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="db0ba-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="db0ba-112">获取 groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="db0ba-112">Get groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-get.md)|[<span data-ttu-id="db0ba-113">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="db0ba-113">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="db0ba-114">读取 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db0ba-114">Read properties and relationships of the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|
|[<span data-ttu-id="db0ba-115">更新 groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="db0ba-115">Update groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-update.md)|[<span data-ttu-id="db0ba-116">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="db0ba-116">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="db0ba-117">更新 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="db0ba-117">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="db0ba-118">属性</span><span class="sxs-lookup"><span data-stu-id="db0ba-118">Properties</span></span>
|<span data-ttu-id="db0ba-119">属性</span><span class="sxs-lookup"><span data-stu-id="db0ba-119">Property</span></span>|<span data-ttu-id="db0ba-120">类型</span><span class="sxs-lookup"><span data-stu-id="db0ba-120">Type</span></span>|<span data-ttu-id="db0ba-121">说明</span><span class="sxs-lookup"><span data-stu-id="db0ba-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db0ba-122">displayName</span><span class="sxs-lookup"><span data-stu-id="db0ba-122">displayName</span></span>|<span data-ttu-id="db0ba-123">String</span><span class="sxs-lookup"><span data-stu-id="db0ba-123">String</span></span>|<span data-ttu-id="db0ba-124">类别的显示名称的字符串 id</span><span class="sxs-lookup"><span data-stu-id="db0ba-124">The string id of the category's display name</span></span>|
|<span data-ttu-id="db0ba-125">isRoot</span><span class="sxs-lookup"><span data-stu-id="db0ba-125">isRoot</span></span>|<span data-ttu-id="db0ba-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="db0ba-126">Boolean</span></span>|<span data-ttu-id="db0ba-127">定义类别是否为根类别</span><span class="sxs-lookup"><span data-stu-id="db0ba-127">Defines if the category is a root category</span></span>|
|<span data-ttu-id="db0ba-128">id</span><span class="sxs-lookup"><span data-stu-id="db0ba-128">id</span></span>|<span data-ttu-id="db0ba-129">String</span><span class="sxs-lookup"><span data-stu-id="db0ba-129">String</span></span>|<span data-ttu-id="db0ba-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db0ba-130">Key of the entity.</span></span>|
|<span data-ttu-id="db0ba-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db0ba-131">lastModifiedDateTime</span></span>|<span data-ttu-id="db0ba-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db0ba-132">DateTimeOffset</span></span>|<span data-ttu-id="db0ba-133">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="db0ba-133">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db0ba-134">关系</span><span class="sxs-lookup"><span data-stu-id="db0ba-134">Relationships</span></span>
|<span data-ttu-id="db0ba-135">关系</span><span class="sxs-lookup"><span data-stu-id="db0ba-135">Relationship</span></span>|<span data-ttu-id="db0ba-136">类型</span><span class="sxs-lookup"><span data-stu-id="db0ba-136">Type</span></span>|<span data-ttu-id="db0ba-137">说明</span><span class="sxs-lookup"><span data-stu-id="db0ba-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db0ba-138">父级</span><span class="sxs-lookup"><span data-stu-id="db0ba-138">parent</span></span>|[<span data-ttu-id="db0ba-139">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="db0ba-139">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="db0ba-140">父类别</span><span class="sxs-lookup"><span data-stu-id="db0ba-140">The parent category</span></span>|
|<span data-ttu-id="db0ba-141">children</span><span class="sxs-lookup"><span data-stu-id="db0ba-141">children</span></span>|<span data-ttu-id="db0ba-142">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db0ba-142">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) collection</span></span>|<span data-ttu-id="db0ba-143">子类别</span><span class="sxs-lookup"><span data-stu-id="db0ba-143">The children categories</span></span>|
|<span data-ttu-id="db0ba-144">限定</span><span class="sxs-lookup"><span data-stu-id="db0ba-144">definitions</span></span>|<span data-ttu-id="db0ba-145">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db0ba-145">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="db0ba-146">类别的直接 GroupPolicyDefinition 子类别</span><span class="sxs-lookup"><span data-stu-id="db0ba-146">The immediate GroupPolicyDefinition children of the category</span></span>|
|<span data-ttu-id="db0ba-147">definitionFile</span><span class="sxs-lookup"><span data-stu-id="db0ba-147">definitionFile</span></span>|[<span data-ttu-id="db0ba-148">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="db0ba-148">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="db0ba-149">类别所属的定义文件的 id</span><span class="sxs-lookup"><span data-stu-id="db0ba-149">The id of the definition file the category came from</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db0ba-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db0ba-150">JSON Representation</span></span>
<span data-ttu-id="db0ba-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db0ba-151">Here is a JSON representation of the resource.</span></span>
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






