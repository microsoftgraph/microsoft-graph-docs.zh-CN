---
title: groupPolicyDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9ba5a4c415b0bc94b60479530ac6a7ca35f3c75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031009"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="9f8cb-103">groupPolicyDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f8cb-103">groupPolicyDefinition resource type</span></span>

<span data-ttu-id="9f8cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f8cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f8cb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f8cb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f8cb-107">实体描述有关单个组策略的所有信息。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="9f8cb-108">方法</span><span class="sxs-lookup"><span data-stu-id="9f8cb-108">Methods</span></span>
|<span data-ttu-id="9f8cb-109">方法</span><span class="sxs-lookup"><span data-stu-id="9f8cb-109">Method</span></span>|<span data-ttu-id="9f8cb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f8cb-110">Return Type</span></span>|<span data-ttu-id="9f8cb-111">说明</span><span class="sxs-lookup"><span data-stu-id="9f8cb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f8cb-112">获取 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9f8cb-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="9f8cb-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9f8cb-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9f8cb-114">读取 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="9f8cb-115">更新 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9f8cb-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="9f8cb-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9f8cb-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9f8cb-117">更新 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f8cb-118">属性</span><span class="sxs-lookup"><span data-stu-id="9f8cb-118">Properties</span></span>
|<span data-ttu-id="9f8cb-119">属性</span><span class="sxs-lookup"><span data-stu-id="9f8cb-119">Property</span></span>|<span data-ttu-id="9f8cb-120">类型</span><span class="sxs-lookup"><span data-stu-id="9f8cb-120">Type</span></span>|<span data-ttu-id="9f8cb-121">说明</span><span class="sxs-lookup"><span data-stu-id="9f8cb-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f8cb-122">classType</span><span class="sxs-lookup"><span data-stu-id="9f8cb-122">classType</span></span>|[<span data-ttu-id="9f8cb-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="9f8cb-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="9f8cb-124">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="9f8cb-125">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-125">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9f8cb-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9f8cb-126">displayName</span></span>|<span data-ttu-id="9f8cb-127">String</span><span class="sxs-lookup"><span data-stu-id="9f8cb-127">String</span></span>|<span data-ttu-id="9f8cb-128">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-128">The localized policy name.</span></span>|
|<span data-ttu-id="9f8cb-129">explainText</span><span class="sxs-lookup"><span data-stu-id="9f8cb-129">explainText</span></span>|<span data-ttu-id="9f8cb-130">String</span><span class="sxs-lookup"><span data-stu-id="9f8cb-130">String</span></span>|<span data-ttu-id="9f8cb-131">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="9f8cb-132">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-132">The default value is empty.</span></span>|
|<span data-ttu-id="9f8cb-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="9f8cb-133">categoryPath</span></span>|<span data-ttu-id="9f8cb-134">String</span><span class="sxs-lookup"><span data-stu-id="9f8cb-134">String</span></span>|<span data-ttu-id="9f8cb-135">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="9f8cb-136">supportedOn</span><span class="sxs-lookup"><span data-stu-id="9f8cb-136">supportedOn</span></span>|<span data-ttu-id="9f8cb-137">String</span><span class="sxs-lookup"><span data-stu-id="9f8cb-137">String</span></span>|<span data-ttu-id="9f8cb-138">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="9f8cb-139">policyType</span><span class="sxs-lookup"><span data-stu-id="9f8cb-139">policyType</span></span>|[<span data-ttu-id="9f8cb-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="9f8cb-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9f8cb-141">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-141">Specifies the type of group policy.</span></span> <span data-ttu-id="9f8cb-142">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9f8cb-143">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="9f8cb-143">groupPolicyCategoryId</span></span>|<span data-ttu-id="9f8cb-144">Guid</span><span class="sxs-lookup"><span data-stu-id="9f8cb-144">Guid</span></span>|<span data-ttu-id="9f8cb-145">父类别的类别 id</span><span class="sxs-lookup"><span data-stu-id="9f8cb-145">The category id of the parent category</span></span>|
|<span data-ttu-id="9f8cb-146">id</span><span class="sxs-lookup"><span data-stu-id="9f8cb-146">id</span></span>|<span data-ttu-id="9f8cb-147">String</span><span class="sxs-lookup"><span data-stu-id="9f8cb-147">String</span></span>|<span data-ttu-id="9f8cb-148">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-148">Key of the entity.</span></span>|
|<span data-ttu-id="9f8cb-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f8cb-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9f8cb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f8cb-150">DateTimeOffset</span></span>|<span data-ttu-id="9f8cb-151">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f8cb-152">关系</span><span class="sxs-lookup"><span data-stu-id="9f8cb-152">Relationships</span></span>
|<span data-ttu-id="9f8cb-153">关系</span><span class="sxs-lookup"><span data-stu-id="9f8cb-153">Relationship</span></span>|<span data-ttu-id="9f8cb-154">类型</span><span class="sxs-lookup"><span data-stu-id="9f8cb-154">Type</span></span>|<span data-ttu-id="9f8cb-155">说明</span><span class="sxs-lookup"><span data-stu-id="9f8cb-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f8cb-156">definitionFile</span><span class="sxs-lookup"><span data-stu-id="9f8cb-156">definitionFile</span></span>|[<span data-ttu-id="9f8cb-157">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="9f8cb-157">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="9f8cb-158">与定义关联的组策略文件。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-158">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="9f8cb-159">“类别”</span><span class="sxs-lookup"><span data-stu-id="9f8cb-159">category</span></span>|[<span data-ttu-id="9f8cb-160">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="9f8cb-160">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="9f8cb-161">与定义关联的组策略类别。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-161">The group policy category associated with the definition.</span></span>|
|<span data-ttu-id="9f8cb-162">文稿</span><span class="sxs-lookup"><span data-stu-id="9f8cb-162">presentations</span></span>|<span data-ttu-id="9f8cb-163">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f8cb-163">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="9f8cb-164">与定义关联的组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-164">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f8cb-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f8cb-165">JSON Representation</span></span>
<span data-ttu-id="9f8cb-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f8cb-166">Here is a JSON representation of the resource.</span></span>
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






