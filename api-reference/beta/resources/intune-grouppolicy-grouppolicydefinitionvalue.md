---
title: groupPolicyDefinitionValue 资源类型
description: 定义值实体存储单个组策略定义的值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7e98a41409efba60ee1431fac82a49be2029039
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429538"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a><span data-ttu-id="27840-103">groupPolicyDefinitionValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="27840-103">groupPolicyDefinitionValue resource type</span></span>

> <span data-ttu-id="27840-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="27840-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27840-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27840-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27840-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27840-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27840-107">定义值实体存储单个组策略定义的值。</span><span class="sxs-lookup"><span data-stu-id="27840-107">The definition value entity stores the value for a single group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="27840-108">方法</span><span class="sxs-lookup"><span data-stu-id="27840-108">Methods</span></span>
|<span data-ttu-id="27840-109">方法</span><span class="sxs-lookup"><span data-stu-id="27840-109">Method</span></span>|<span data-ttu-id="27840-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="27840-110">Return Type</span></span>|<span data-ttu-id="27840-111">说明</span><span class="sxs-lookup"><span data-stu-id="27840-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27840-112">列表 groupPolicyDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="27840-112">List groupPolicyDefinitionValues</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|<span data-ttu-id="27840-113">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="27840-113">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="27840-114">列出属性和[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="27840-114">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>|
|[<span data-ttu-id="27840-115">获取 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="27840-115">Get groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[<span data-ttu-id="27840-116">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="27840-116">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="27840-117">读取属性和[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="27840-117">Read properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="27840-118">创建 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="27840-118">Create groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[<span data-ttu-id="27840-119">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="27840-119">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="27840-120">创建新的[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27840-120">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="27840-121">删除 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="27840-121">Delete groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|<span data-ttu-id="27840-122">无</span><span class="sxs-lookup"><span data-stu-id="27840-122">None</span></span>|<span data-ttu-id="27840-123">删除[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)。</span><span class="sxs-lookup"><span data-stu-id="27840-123">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>|
|[<span data-ttu-id="27840-124">更新 groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="27840-124">Update groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[<span data-ttu-id="27840-125">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="27840-125">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="27840-126">更新[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27840-126">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27840-127">属性</span><span class="sxs-lookup"><span data-stu-id="27840-127">Properties</span></span>
|<span data-ttu-id="27840-128">属性</span><span class="sxs-lookup"><span data-stu-id="27840-128">Property</span></span>|<span data-ttu-id="27840-129">类型</span><span class="sxs-lookup"><span data-stu-id="27840-129">Type</span></span>|<span data-ttu-id="27840-130">说明</span><span class="sxs-lookup"><span data-stu-id="27840-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27840-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27840-131">createdDateTime</span></span>|<span data-ttu-id="27840-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27840-132">DateTimeOffset</span></span>|<span data-ttu-id="27840-133">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="27840-133">The date and time the object was created.</span></span>|
|<span data-ttu-id="27840-134">enabled</span><span class="sxs-lookup"><span data-stu-id="27840-134">enabled</span></span>|<span data-ttu-id="27840-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="27840-135">Boolean</span></span>|<span data-ttu-id="27840-136">启用或禁用相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="27840-136">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="27840-137">configurationType</span><span class="sxs-lookup"><span data-stu-id="27840-137">configurationType</span></span>|[<span data-ttu-id="27840-138">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="27840-138">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="27840-139">指定应如何配置的值。</span><span class="sxs-lookup"><span data-stu-id="27840-139">Specifies how the value should be configured.</span></span> <span data-ttu-id="27840-140">这可以是一个策略作为或首选项。</span><span class="sxs-lookup"><span data-stu-id="27840-140">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="27840-141">可取值为：`policy`、`preference`。</span><span class="sxs-lookup"><span data-stu-id="27840-141">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="27840-142">id</span><span class="sxs-lookup"><span data-stu-id="27840-142">id</span></span>|<span data-ttu-id="27840-143">String</span><span class="sxs-lookup"><span data-stu-id="27840-143">String</span></span>|<span data-ttu-id="27840-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27840-144">Key of the entity.</span></span>|
|<span data-ttu-id="27840-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27840-145">lastModifiedDateTime</span></span>|<span data-ttu-id="27840-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27840-146">DateTimeOffset</span></span>|<span data-ttu-id="27840-147">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="27840-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27840-148">关系</span><span class="sxs-lookup"><span data-stu-id="27840-148">Relationships</span></span>
|<span data-ttu-id="27840-149">关系</span><span class="sxs-lookup"><span data-stu-id="27840-149">Relationship</span></span>|<span data-ttu-id="27840-150">类型</span><span class="sxs-lookup"><span data-stu-id="27840-150">Type</span></span>|<span data-ttu-id="27840-151">说明</span><span class="sxs-lookup"><span data-stu-id="27840-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27840-152">presentationValues</span><span class="sxs-lookup"><span data-stu-id="27840-152">presentationValues</span></span>|<span data-ttu-id="27840-153">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="27840-153">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="27840-154">相关联的组策略演示文稿的定义值的值。</span><span class="sxs-lookup"><span data-stu-id="27840-154">The associated group policy presentation values with the definition value.</span></span>|
|<span data-ttu-id="27840-155">definition</span><span class="sxs-lookup"><span data-stu-id="27840-155">definition</span></span>|[<span data-ttu-id="27840-156">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="27840-156">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="27840-157">相关联的组策略定义的值。</span><span class="sxs-lookup"><span data-stu-id="27840-157">The associated group policy definition with the value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27840-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27840-158">JSON Representation</span></span>
<span data-ttu-id="27840-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27840-159">Here is a JSON representation of the resource.</span></span>
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




