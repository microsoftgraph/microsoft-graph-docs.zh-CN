---
title: groupPolicyPresentationValue 资源类型
description: 用于存储单个组策略演示文稿的值的基本演示文稿值实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a1cb9d8cad31faf2dc888082f491c0df51ba01e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524404"
---
# <a name="grouppolicypresentationvalue-resource-type"></a><span data-ttu-id="7b74c-103">groupPolicyPresentationValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b74c-103">groupPolicyPresentationValue resource type</span></span>

<span data-ttu-id="7b74c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7b74c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b74c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b74c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b74c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b74c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b74c-107">用于存储单个组策略演示文稿的值的基本演示文稿值实体。</span><span class="sxs-lookup"><span data-stu-id="7b74c-107">The base presentation value entity that stores the value for a single group policy presentation.</span></span>

## <a name="methods"></a><span data-ttu-id="7b74c-108">方法</span><span class="sxs-lookup"><span data-stu-id="7b74c-108">Methods</span></span>
|<span data-ttu-id="7b74c-109">方法</span><span class="sxs-lookup"><span data-stu-id="7b74c-109">Method</span></span>|<span data-ttu-id="7b74c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7b74c-110">Return Type</span></span>|<span data-ttu-id="7b74c-111">说明</span><span class="sxs-lookup"><span data-stu-id="7b74c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b74c-112">列出 groupPolicyPresentationValues</span><span class="sxs-lookup"><span data-stu-id="7b74c-112">List groupPolicyPresentationValues</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|<span data-ttu-id="7b74c-113">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="7b74c-113">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="7b74c-114">列出[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b74c-114">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>|
|[<span data-ttu-id="7b74c-115">获取 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-115">Get groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[<span data-ttu-id="7b74c-116">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-116">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="7b74c-117">读取[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b74c-117">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="7b74c-118">创建 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-118">Create groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[<span data-ttu-id="7b74c-119">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-119">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="7b74c-120">创建新的[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b74c-120">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="7b74c-121">删除 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-121">Delete groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|<span data-ttu-id="7b74c-122">无</span><span class="sxs-lookup"><span data-stu-id="7b74c-122">None</span></span>|<span data-ttu-id="7b74c-123">删除[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="7b74c-123">Deletes a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>|
|[<span data-ttu-id="7b74c-124">更新 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-124">Update groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[<span data-ttu-id="7b74c-125">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-125">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="7b74c-126">更新[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7b74c-126">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b74c-127">属性</span><span class="sxs-lookup"><span data-stu-id="7b74c-127">Properties</span></span>
|<span data-ttu-id="7b74c-128">属性</span><span class="sxs-lookup"><span data-stu-id="7b74c-128">Property</span></span>|<span data-ttu-id="7b74c-129">类型</span><span class="sxs-lookup"><span data-stu-id="7b74c-129">Type</span></span>|<span data-ttu-id="7b74c-130">说明</span><span class="sxs-lookup"><span data-stu-id="7b74c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b74c-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b74c-131">lastModifiedDateTime</span></span>|<span data-ttu-id="7b74c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b74c-132">DateTimeOffset</span></span>|<span data-ttu-id="7b74c-133">上次修改对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7b74c-133">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="7b74c-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b74c-134">createdDateTime</span></span>|<span data-ttu-id="7b74c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b74c-135">DateTimeOffset</span></span>|<span data-ttu-id="7b74c-136">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7b74c-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="7b74c-137">id</span><span class="sxs-lookup"><span data-stu-id="7b74c-137">id</span></span>|<span data-ttu-id="7b74c-138">String</span><span class="sxs-lookup"><span data-stu-id="7b74c-138">String</span></span>|<span data-ttu-id="7b74c-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7b74c-139">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b74c-140">关系</span><span class="sxs-lookup"><span data-stu-id="7b74c-140">Relationships</span></span>
|<span data-ttu-id="7b74c-141">关系</span><span class="sxs-lookup"><span data-stu-id="7b74c-141">Relationship</span></span>|<span data-ttu-id="7b74c-142">类型</span><span class="sxs-lookup"><span data-stu-id="7b74c-142">Type</span></span>|<span data-ttu-id="7b74c-143">说明</span><span class="sxs-lookup"><span data-stu-id="7b74c-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b74c-144">definitionValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-144">definitionValue</span></span>|[<span data-ttu-id="7b74c-145">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="7b74c-145">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="7b74c-146">与演示文稿值关联的组策略定义值。</span><span class="sxs-lookup"><span data-stu-id="7b74c-146">The group policy definition value associated with the presentation value.</span></span>|
|<span data-ttu-id="7b74c-147">变形</span><span class="sxs-lookup"><span data-stu-id="7b74c-147">presentation</span></span>|[<span data-ttu-id="7b74c-148">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="7b74c-148">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="7b74c-149">与演示文稿值关联的组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="7b74c-149">The group policy presentation associated with the presentation value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b74c-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b74c-150">JSON Representation</span></span>
<span data-ttu-id="7b74c-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b74c-151">Here is a JSON representation of the resource.</span></span>
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



