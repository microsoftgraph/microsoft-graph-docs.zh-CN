---
title: groupPolicyDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e99b32687c0a93673cdbf8889b05e6423cc73c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783021"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="21bb2-103">groupPolicyDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="21bb2-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="21bb2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21bb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bb2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21bb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bb2-106">实体描述有关单个组策略的所有信息。</span><span class="sxs-lookup"><span data-stu-id="21bb2-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="21bb2-107">方法</span><span class="sxs-lookup"><span data-stu-id="21bb2-107">Methods</span></span>
|<span data-ttu-id="21bb2-108">方法</span><span class="sxs-lookup"><span data-stu-id="21bb2-108">Method</span></span>|<span data-ttu-id="21bb2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="21bb2-109">Return Type</span></span>|<span data-ttu-id="21bb2-110">说明</span><span class="sxs-lookup"><span data-stu-id="21bb2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21bb2-111">获取 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="21bb2-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="21bb2-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="21bb2-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="21bb2-113">读取[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21bb2-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="21bb2-114">更新 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="21bb2-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="21bb2-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="21bb2-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="21bb2-116">更新[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="21bb2-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21bb2-117">属性</span><span class="sxs-lookup"><span data-stu-id="21bb2-117">Properties</span></span>
|<span data-ttu-id="21bb2-118">属性</span><span class="sxs-lookup"><span data-stu-id="21bb2-118">Property</span></span>|<span data-ttu-id="21bb2-119">类型</span><span class="sxs-lookup"><span data-stu-id="21bb2-119">Type</span></span>|<span data-ttu-id="21bb2-120">说明</span><span class="sxs-lookup"><span data-stu-id="21bb2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bb2-121">classType</span><span class="sxs-lookup"><span data-stu-id="21bb2-121">classType</span></span>|[<span data-ttu-id="21bb2-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="21bb2-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="21bb2-123">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="21bb2-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="21bb2-124">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="21bb2-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="21bb2-125">displayName</span><span class="sxs-lookup"><span data-stu-id="21bb2-125">displayName</span></span>|<span data-ttu-id="21bb2-126">String</span><span class="sxs-lookup"><span data-stu-id="21bb2-126">String</span></span>|<span data-ttu-id="21bb2-127">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="21bb2-127">The localized policy name.</span></span>|
|<span data-ttu-id="21bb2-128">explainText</span><span class="sxs-lookup"><span data-stu-id="21bb2-128">explainText</span></span>|<span data-ttu-id="21bb2-129">String</span><span class="sxs-lookup"><span data-stu-id="21bb2-129">String</span></span>|<span data-ttu-id="21bb2-130">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="21bb2-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="21bb2-131">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="21bb2-131">The default value is empty.</span></span>|
|<span data-ttu-id="21bb2-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="21bb2-132">categoryPath</span></span>|<span data-ttu-id="21bb2-133">String</span><span class="sxs-lookup"><span data-stu-id="21bb2-133">String</span></span>|<span data-ttu-id="21bb2-134">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="21bb2-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="21bb2-135">supportedOn</span><span class="sxs-lookup"><span data-stu-id="21bb2-135">supportedOn</span></span>|<span data-ttu-id="21bb2-136">String</span><span class="sxs-lookup"><span data-stu-id="21bb2-136">String</span></span>|<span data-ttu-id="21bb2-137">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="21bb2-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="21bb2-138">policyType</span><span class="sxs-lookup"><span data-stu-id="21bb2-138">policyType</span></span>|[<span data-ttu-id="21bb2-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="21bb2-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="21bb2-140">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="21bb2-140">Specifies the type of group policy.</span></span> <span data-ttu-id="21bb2-141">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="21bb2-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="21bb2-142">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="21bb2-142">groupPolicyCategoryId</span></span>|<span data-ttu-id="21bb2-143">Guid</span><span class="sxs-lookup"><span data-stu-id="21bb2-143">Guid</span></span>|<span data-ttu-id="21bb2-144">父类别的类别 id</span><span class="sxs-lookup"><span data-stu-id="21bb2-144">The category id of the parent category</span></span>|
|<span data-ttu-id="21bb2-145">id</span><span class="sxs-lookup"><span data-stu-id="21bb2-145">id</span></span>|<span data-ttu-id="21bb2-146">String</span><span class="sxs-lookup"><span data-stu-id="21bb2-146">String</span></span>|<span data-ttu-id="21bb2-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="21bb2-147">Key of the entity.</span></span>|
|<span data-ttu-id="21bb2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21bb2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="21bb2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21bb2-149">DateTimeOffset</span></span>|<span data-ttu-id="21bb2-150">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="21bb2-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21bb2-151">关系</span><span class="sxs-lookup"><span data-stu-id="21bb2-151">Relationships</span></span>
|<span data-ttu-id="21bb2-152">关系</span><span class="sxs-lookup"><span data-stu-id="21bb2-152">Relationship</span></span>|<span data-ttu-id="21bb2-153">类型</span><span class="sxs-lookup"><span data-stu-id="21bb2-153">Type</span></span>|<span data-ttu-id="21bb2-154">说明</span><span class="sxs-lookup"><span data-stu-id="21bb2-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bb2-155">definitionFile</span><span class="sxs-lookup"><span data-stu-id="21bb2-155">definitionFile</span></span>|[<span data-ttu-id="21bb2-156">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="21bb2-156">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="21bb2-157">与定义关联的组策略文件。</span><span class="sxs-lookup"><span data-stu-id="21bb2-157">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="21bb2-158">“类别”</span><span class="sxs-lookup"><span data-stu-id="21bb2-158">category</span></span>|[<span data-ttu-id="21bb2-159">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="21bb2-159">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="21bb2-160">与定义关联的组策略类别。</span><span class="sxs-lookup"><span data-stu-id="21bb2-160">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="21bb2-161">文稿</span><span class="sxs-lookup"><span data-stu-id="21bb2-161">presentations</span></span>|<span data-ttu-id="21bb2-162">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)集合</span><span class="sxs-lookup"><span data-stu-id="21bb2-162">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="21bb2-163">与定义关联的组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="21bb2-163">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21bb2-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21bb2-164">JSON Representation</span></span>
<span data-ttu-id="21bb2-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21bb2-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "groupPolicyCategoryId": "Guid",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



