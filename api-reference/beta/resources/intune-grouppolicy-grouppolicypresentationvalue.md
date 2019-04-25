---
title: groupPolicyPresentationValue 资源类型
description: 用于存储单个组策略演示文稿的值的基本演示文稿值实体。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d4f3d1493e85708335797252301b451f5e41520
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575847"
---
# <a name="grouppolicypresentationvalue-resource-type"></a><span data-ttu-id="90e9b-103">groupPolicyPresentationValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="90e9b-103">groupPolicyPresentationValue resource type</span></span>

> <span data-ttu-id="90e9b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90e9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90e9b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90e9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90e9b-106">用于存储单个组策略演示文稿的值的基本演示文稿值实体。</span><span class="sxs-lookup"><span data-stu-id="90e9b-106">The base presentation value entity that stores the value for a single group policy presentation.</span></span>

## <a name="methods"></a><span data-ttu-id="90e9b-107">方法</span><span class="sxs-lookup"><span data-stu-id="90e9b-107">Methods</span></span>
|<span data-ttu-id="90e9b-108">方法</span><span class="sxs-lookup"><span data-stu-id="90e9b-108">Method</span></span>|<span data-ttu-id="90e9b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="90e9b-109">Return Type</span></span>|<span data-ttu-id="90e9b-110">说明</span><span class="sxs-lookup"><span data-stu-id="90e9b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90e9b-111">列出 groupPolicyPresentationValues</span><span class="sxs-lookup"><span data-stu-id="90e9b-111">List groupPolicyPresentationValues</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|<span data-ttu-id="90e9b-112">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="90e9b-112">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="90e9b-113">列出[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90e9b-113">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>|
|[<span data-ttu-id="90e9b-114">获取 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-114">Get groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[<span data-ttu-id="90e9b-115">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-115">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="90e9b-116">读取[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90e9b-116">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="90e9b-117">创建 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-117">Create groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[<span data-ttu-id="90e9b-118">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-118">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="90e9b-119">创建新的[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="90e9b-119">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="90e9b-120">删除 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-120">Delete groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|<span data-ttu-id="90e9b-121">无</span><span class="sxs-lookup"><span data-stu-id="90e9b-121">None</span></span>|<span data-ttu-id="90e9b-122">删除[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="90e9b-122">Deletes a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>|
|[<span data-ttu-id="90e9b-123">更新 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-123">Update groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[<span data-ttu-id="90e9b-124">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-124">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="90e9b-125">更新[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="90e9b-125">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90e9b-126">属性</span><span class="sxs-lookup"><span data-stu-id="90e9b-126">Properties</span></span>
|<span data-ttu-id="90e9b-127">属性</span><span class="sxs-lookup"><span data-stu-id="90e9b-127">Property</span></span>|<span data-ttu-id="90e9b-128">类型</span><span class="sxs-lookup"><span data-stu-id="90e9b-128">Type</span></span>|<span data-ttu-id="90e9b-129">说明</span><span class="sxs-lookup"><span data-stu-id="90e9b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90e9b-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90e9b-130">lastModifiedDateTime</span></span>|<span data-ttu-id="90e9b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90e9b-131">DateTimeOffset</span></span>|<span data-ttu-id="90e9b-132">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90e9b-132">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="90e9b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90e9b-133">createdDateTime</span></span>|<span data-ttu-id="90e9b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90e9b-134">DateTimeOffset</span></span>|<span data-ttu-id="90e9b-135">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90e9b-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="90e9b-136">id</span><span class="sxs-lookup"><span data-stu-id="90e9b-136">id</span></span>|<span data-ttu-id="90e9b-137">String</span><span class="sxs-lookup"><span data-stu-id="90e9b-137">String</span></span>|<span data-ttu-id="90e9b-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="90e9b-138">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90e9b-139">关系</span><span class="sxs-lookup"><span data-stu-id="90e9b-139">Relationships</span></span>
|<span data-ttu-id="90e9b-140">关系</span><span class="sxs-lookup"><span data-stu-id="90e9b-140">Relationship</span></span>|<span data-ttu-id="90e9b-141">类型</span><span class="sxs-lookup"><span data-stu-id="90e9b-141">Type</span></span>|<span data-ttu-id="90e9b-142">说明</span><span class="sxs-lookup"><span data-stu-id="90e9b-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90e9b-143">definitionValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-143">definitionValue</span></span>|[<span data-ttu-id="90e9b-144">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="90e9b-144">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="90e9b-145">与演示文稿值关联的组策略定义值。</span><span class="sxs-lookup"><span data-stu-id="90e9b-145">The group policy definition value associated with the presentation value.</span></span>|
|<span data-ttu-id="90e9b-146">变形</span><span class="sxs-lookup"><span data-stu-id="90e9b-146">presentation</span></span>|[<span data-ttu-id="90e9b-147">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="90e9b-147">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="90e9b-148">与演示文稿值关联的组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="90e9b-148">The group policy presentation associated with the presentation value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90e9b-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90e9b-149">JSON Representation</span></span>
<span data-ttu-id="90e9b-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90e9b-150">Here is a JSON representation of the resource.</span></span>
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





