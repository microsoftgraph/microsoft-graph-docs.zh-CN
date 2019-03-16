---
title: groupPolicyDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5062fda984dbe1dda518e77ff271750d30adb8
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644284"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="968a3-103">groupPolicyDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="968a3-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="968a3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="968a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="968a3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="968a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="968a3-106">实体描述有关单个组策略的所有信息。</span><span class="sxs-lookup"><span data-stu-id="968a3-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="968a3-107">方法</span><span class="sxs-lookup"><span data-stu-id="968a3-107">Methods</span></span>
|<span data-ttu-id="968a3-108">方法</span><span class="sxs-lookup"><span data-stu-id="968a3-108">Method</span></span>|<span data-ttu-id="968a3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="968a3-109">Return Type</span></span>|<span data-ttu-id="968a3-110">说明</span><span class="sxs-lookup"><span data-stu-id="968a3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="968a3-111">获取 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="968a3-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="968a3-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="968a3-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="968a3-113">读取[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="968a3-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="968a3-114">更新 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="968a3-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="968a3-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="968a3-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="968a3-116">更新[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="968a3-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="968a3-117">属性</span><span class="sxs-lookup"><span data-stu-id="968a3-117">Properties</span></span>
|<span data-ttu-id="968a3-118">属性</span><span class="sxs-lookup"><span data-stu-id="968a3-118">Property</span></span>|<span data-ttu-id="968a3-119">类型</span><span class="sxs-lookup"><span data-stu-id="968a3-119">Type</span></span>|<span data-ttu-id="968a3-120">说明</span><span class="sxs-lookup"><span data-stu-id="968a3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="968a3-121">classType</span><span class="sxs-lookup"><span data-stu-id="968a3-121">classType</span></span>|[<span data-ttu-id="968a3-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="968a3-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="968a3-123">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="968a3-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="968a3-124">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="968a3-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="968a3-125">displayName</span><span class="sxs-lookup"><span data-stu-id="968a3-125">displayName</span></span>|<span data-ttu-id="968a3-126">String</span><span class="sxs-lookup"><span data-stu-id="968a3-126">String</span></span>|<span data-ttu-id="968a3-127">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="968a3-127">The localized policy name.</span></span>|
|<span data-ttu-id="968a3-128">explainText</span><span class="sxs-lookup"><span data-stu-id="968a3-128">explainText</span></span>|<span data-ttu-id="968a3-129">字符串</span><span class="sxs-lookup"><span data-stu-id="968a3-129">String</span></span>|<span data-ttu-id="968a3-130">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="968a3-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="968a3-131">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="968a3-131">The default value is empty.</span></span>|
|<span data-ttu-id="968a3-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="968a3-132">categoryPath</span></span>|<span data-ttu-id="968a3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="968a3-133">String</span></span>|<span data-ttu-id="968a3-134">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="968a3-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="968a3-135">supportedOn</span><span class="sxs-lookup"><span data-stu-id="968a3-135">supportedOn</span></span>|<span data-ttu-id="968a3-136">字符串</span><span class="sxs-lookup"><span data-stu-id="968a3-136">String</span></span>|<span data-ttu-id="968a3-137">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="968a3-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="968a3-138">policyType</span><span class="sxs-lookup"><span data-stu-id="968a3-138">policyType</span></span>|[<span data-ttu-id="968a3-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="968a3-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="968a3-140">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="968a3-140">Specifies the type of group policy.</span></span> <span data-ttu-id="968a3-141">可能的值是：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="968a3-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="968a3-142">id</span><span class="sxs-lookup"><span data-stu-id="968a3-142">id</span></span>|<span data-ttu-id="968a3-143">String</span><span class="sxs-lookup"><span data-stu-id="968a3-143">String</span></span>|<span data-ttu-id="968a3-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="968a3-144">Key of the entity.</span></span>|
|<span data-ttu-id="968a3-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="968a3-145">lastModifiedDateTime</span></span>|<span data-ttu-id="968a3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="968a3-146">DateTimeOffset</span></span>|<span data-ttu-id="968a3-147">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="968a3-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="968a3-148">关系</span><span class="sxs-lookup"><span data-stu-id="968a3-148">Relationships</span></span>
|<span data-ttu-id="968a3-149">关系</span><span class="sxs-lookup"><span data-stu-id="968a3-149">Relationship</span></span>|<span data-ttu-id="968a3-150">类型</span><span class="sxs-lookup"><span data-stu-id="968a3-150">Type</span></span>|<span data-ttu-id="968a3-151">说明</span><span class="sxs-lookup"><span data-stu-id="968a3-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="968a3-152">definitionFile</span><span class="sxs-lookup"><span data-stu-id="968a3-152">definitionFile</span></span>|[<span data-ttu-id="968a3-153">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="968a3-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="968a3-154">与定义关联的组策略文件。</span><span class="sxs-lookup"><span data-stu-id="968a3-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="968a3-155">文稿</span><span class="sxs-lookup"><span data-stu-id="968a3-155">presentations</span></span>|<span data-ttu-id="968a3-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)集合</span><span class="sxs-lookup"><span data-stu-id="968a3-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="968a3-157">与定义关联的组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="968a3-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="968a3-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="968a3-158">JSON Representation</span></span>
<span data-ttu-id="968a3-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="968a3-159">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




