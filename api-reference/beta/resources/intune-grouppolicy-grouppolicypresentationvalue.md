---
title: groupPolicyPresentationValue 资源类型
description: 基本演示文稿值实体存储的一个组策略演示文稿的值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec299eccc29ddcb39ece0d1f6c0e063a02192909
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429287"
---
# <a name="grouppolicypresentationvalue-resource-type"></a><span data-ttu-id="ca75e-103">groupPolicyPresentationValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca75e-103">groupPolicyPresentationValue resource type</span></span>

> <span data-ttu-id="ca75e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ca75e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca75e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca75e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca75e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca75e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca75e-107">基本演示文稿值实体存储的一个组策略演示文稿的值。</span><span class="sxs-lookup"><span data-stu-id="ca75e-107">The base presentation value entity that stores the value for a single group policy presentation.</span></span>

## <a name="methods"></a><span data-ttu-id="ca75e-108">方法</span><span class="sxs-lookup"><span data-stu-id="ca75e-108">Methods</span></span>
|<span data-ttu-id="ca75e-109">方法</span><span class="sxs-lookup"><span data-stu-id="ca75e-109">Method</span></span>|<span data-ttu-id="ca75e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca75e-110">Return Type</span></span>|<span data-ttu-id="ca75e-111">说明</span><span class="sxs-lookup"><span data-stu-id="ca75e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca75e-112">列表 groupPolicyPresentationValues</span><span class="sxs-lookup"><span data-stu-id="ca75e-112">List groupPolicyPresentationValues</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|<span data-ttu-id="ca75e-113">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca75e-113">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="ca75e-114">列出属性和[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="ca75e-114">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>|
|[<span data-ttu-id="ca75e-115">获取 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-115">Get groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[<span data-ttu-id="ca75e-116">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-116">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="ca75e-117">读取属性和[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ca75e-117">Read properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="ca75e-118">创建 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-118">Create groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[<span data-ttu-id="ca75e-119">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-119">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="ca75e-120">创建新的[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca75e-120">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|
|[<span data-ttu-id="ca75e-121">删除 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-121">Delete groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|<span data-ttu-id="ca75e-122">无</span><span class="sxs-lookup"><span data-stu-id="ca75e-122">None</span></span>|<span data-ttu-id="ca75e-123">删除[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="ca75e-123">Deletes a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>|
|[<span data-ttu-id="ca75e-124">更新 groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-124">Update groupPolicyPresentationValue</span></span>](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[<span data-ttu-id="ca75e-125">groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-125">groupPolicyPresentationValue</span></span>](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|<span data-ttu-id="ca75e-126">更新[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ca75e-126">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca75e-127">属性</span><span class="sxs-lookup"><span data-stu-id="ca75e-127">Properties</span></span>
|<span data-ttu-id="ca75e-128">属性</span><span class="sxs-lookup"><span data-stu-id="ca75e-128">Property</span></span>|<span data-ttu-id="ca75e-129">类型</span><span class="sxs-lookup"><span data-stu-id="ca75e-129">Type</span></span>|<span data-ttu-id="ca75e-130">说明</span><span class="sxs-lookup"><span data-stu-id="ca75e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca75e-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca75e-131">lastModifiedDateTime</span></span>|<span data-ttu-id="ca75e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca75e-132">DateTimeOffset</span></span>|<span data-ttu-id="ca75e-133">日期和时间上次修改对象。</span><span class="sxs-lookup"><span data-stu-id="ca75e-133">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="ca75e-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca75e-134">createdDateTime</span></span>|<span data-ttu-id="ca75e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca75e-135">DateTimeOffset</span></span>|<span data-ttu-id="ca75e-136">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="ca75e-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="ca75e-137">id</span><span class="sxs-lookup"><span data-stu-id="ca75e-137">id</span></span>|<span data-ttu-id="ca75e-138">String</span><span class="sxs-lookup"><span data-stu-id="ca75e-138">String</span></span>|<span data-ttu-id="ca75e-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ca75e-139">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca75e-140">关系</span><span class="sxs-lookup"><span data-stu-id="ca75e-140">Relationships</span></span>
|<span data-ttu-id="ca75e-141">关系</span><span class="sxs-lookup"><span data-stu-id="ca75e-141">Relationship</span></span>|<span data-ttu-id="ca75e-142">类型</span><span class="sxs-lookup"><span data-stu-id="ca75e-142">Type</span></span>|<span data-ttu-id="ca75e-143">说明</span><span class="sxs-lookup"><span data-stu-id="ca75e-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca75e-144">definitionValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-144">definitionValue</span></span>|[<span data-ttu-id="ca75e-145">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="ca75e-145">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="ca75e-146">关联的演示文稿值的组策略定义值。</span><span class="sxs-lookup"><span data-stu-id="ca75e-146">The group policy definition value associated with the presentation value.</span></span>|
|<span data-ttu-id="ca75e-147">演示文稿</span><span class="sxs-lookup"><span data-stu-id="ca75e-147">presentation</span></span>|[<span data-ttu-id="ca75e-148">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="ca75e-148">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="ca75e-149">组策略演示的演示文稿值相关联。</span><span class="sxs-lookup"><span data-stu-id="ca75e-149">The group policy presentation associated with the presentation value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca75e-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca75e-150">JSON Representation</span></span>
<span data-ttu-id="ca75e-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca75e-151">Here is a JSON representation of the resource.</span></span>
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




