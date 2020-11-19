---
title: groupPolicyPresentationValue 资源类型
description: 用于存储单个组策略演示文稿的值的基本演示文稿值实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d44ce8e11ae1f44d10518ea2b1b0c990153923cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222805"
---
# <a name="grouppolicypresentationvalue-resource-type"></a><span data-ttu-id="5df81-103">groupPolicyPresentationValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="5df81-103">groupPolicyPresentationValue resource type</span></span>

<span data-ttu-id="5df81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5df81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5df81-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5df81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5df81-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5df81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5df81-107">用于存储单个组策略演示文稿的值的基本演示文稿值实体。</span><span class="sxs-lookup"><span data-stu-id="5df81-107">The base presentation value entity that stores the value for a single group policy presentation.</span></span>

## <a name="methods"></a><span data-ttu-id="5df81-108">方法</span><span class="sxs-lookup"><span data-stu-id="5df81-108">Methods</span></span>
|<span data-ttu-id="5df81-109">方法</span><span class="sxs-lookup"><span data-stu-id="5df81-109">Method</span></span>|<span data-ttu-id="5df81-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5df81-110">Return Type</span></span>|<span data-ttu-id="5df81-111">说明</span><span class="sxs-lookup"><span data-stu-id="5df81-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5df81-112">列出 groupPolicyPresentationValues</span><span class="sxs-lookup"><span data-stu-id="5df81-112">List groupPolicyPresentationValues</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|<span data-ttu-id="5df81-113">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5df81-113">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="5df81-114">列出 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5df81-114">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>|
|[<span data-ttu-id="5df81-115">获取 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="5df81-115">Get groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[<span data-ttu-id="5df81-116">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="5df81-116">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="5df81-117">读取 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5df81-117">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="5df81-118">创建 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="5df81-118">Create groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[<span data-ttu-id="5df81-119">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="5df81-119">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="5df81-120">创建新的 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5df81-120">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="5df81-121">删除 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="5df81-121">Delete groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|<span data-ttu-id="5df81-122">无</span><span class="sxs-lookup"><span data-stu-id="5df81-122">None</span></span>|<span data-ttu-id="5df81-123">删除 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="5df81-123">Deletes a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>|
|[<span data-ttu-id="5df81-124">更新 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="5df81-124">Update groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[<span data-ttu-id="5df81-125">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="5df81-125">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="5df81-126">更新 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5df81-126">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5df81-127">属性</span><span class="sxs-lookup"><span data-stu-id="5df81-127">Properties</span></span>
|<span data-ttu-id="5df81-128">属性</span><span class="sxs-lookup"><span data-stu-id="5df81-128">Property</span></span>|<span data-ttu-id="5df81-129">类型</span><span class="sxs-lookup"><span data-stu-id="5df81-129">Type</span></span>|<span data-ttu-id="5df81-130">说明</span><span class="sxs-lookup"><span data-stu-id="5df81-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df81-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5df81-131">lastModifiedDateTime</span></span>|<span data-ttu-id="5df81-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df81-132">DateTimeOffset</span></span>|<span data-ttu-id="5df81-133">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5df81-133">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="5df81-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5df81-134">createdDateTime</span></span>|<span data-ttu-id="5df81-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df81-135">DateTimeOffset</span></span>|<span data-ttu-id="5df81-136">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5df81-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="5df81-137">id</span><span class="sxs-lookup"><span data-stu-id="5df81-137">id</span></span>|<span data-ttu-id="5df81-138">String</span><span class="sxs-lookup"><span data-stu-id="5df81-138">String</span></span>|<span data-ttu-id="5df81-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5df81-139">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5df81-140">关系</span><span class="sxs-lookup"><span data-stu-id="5df81-140">Relationships</span></span>
|<span data-ttu-id="5df81-141">关系</span><span class="sxs-lookup"><span data-stu-id="5df81-141">Relationship</span></span>|<span data-ttu-id="5df81-142">类型</span><span class="sxs-lookup"><span data-stu-id="5df81-142">Type</span></span>|<span data-ttu-id="5df81-143">说明</span><span class="sxs-lookup"><span data-stu-id="5df81-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df81-144">definitionValue</span><span class="sxs-lookup"><span data-stu-id="5df81-144">definitionValue</span></span>|[<span data-ttu-id="5df81-145">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="5df81-145">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="5df81-146">与演示文稿值关联的组策略定义值。</span><span class="sxs-lookup"><span data-stu-id="5df81-146">The group policy definition value associated with the presentation value.</span></span>|
|<span data-ttu-id="5df81-147">变形</span><span class="sxs-lookup"><span data-stu-id="5df81-147">presentation</span></span>|[<span data-ttu-id="5df81-148">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="5df81-148">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="5df81-149">与演示文稿值关联的组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="5df81-149">The group policy presentation associated with the presentation value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5df81-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5df81-150">JSON Representation</span></span>
<span data-ttu-id="5df81-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5df81-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```




