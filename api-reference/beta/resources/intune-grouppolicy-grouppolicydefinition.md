---
title: groupPolicyDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17fef49d7d08f94f5ebafd02636d9536a05b87f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941168"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="f9926-103">groupPolicyDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9926-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="f9926-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9926-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9926-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9926-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9926-106">实体描述有关单个组策略的所有信息。</span><span class="sxs-lookup"><span data-stu-id="f9926-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="f9926-107">方法</span><span class="sxs-lookup"><span data-stu-id="f9926-107">Methods</span></span>
|<span data-ttu-id="f9926-108">方法</span><span class="sxs-lookup"><span data-stu-id="f9926-108">Method</span></span>|<span data-ttu-id="f9926-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f9926-109">Return Type</span></span>|<span data-ttu-id="f9926-110">说明</span><span class="sxs-lookup"><span data-stu-id="f9926-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f9926-111">获取 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f9926-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="f9926-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f9926-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="f9926-113">读取[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9926-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="f9926-114">更新 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f9926-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="f9926-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="f9926-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="f9926-116">更新[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9926-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9926-117">属性</span><span class="sxs-lookup"><span data-stu-id="f9926-117">Properties</span></span>
|<span data-ttu-id="f9926-118">属性</span><span class="sxs-lookup"><span data-stu-id="f9926-118">Property</span></span>|<span data-ttu-id="f9926-119">类型</span><span class="sxs-lookup"><span data-stu-id="f9926-119">Type</span></span>|<span data-ttu-id="f9926-120">说明</span><span class="sxs-lookup"><span data-stu-id="f9926-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9926-121">classType</span><span class="sxs-lookup"><span data-stu-id="f9926-121">classType</span></span>|[<span data-ttu-id="f9926-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="f9926-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="f9926-123">标识策略可应用于的组的类型。</span><span class="sxs-lookup"><span data-stu-id="f9926-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="f9926-124">可取值为：`user`、`machine`。</span><span class="sxs-lookup"><span data-stu-id="f9926-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f9926-125">displayName</span><span class="sxs-lookup"><span data-stu-id="f9926-125">displayName</span></span>|<span data-ttu-id="f9926-126">String</span><span class="sxs-lookup"><span data-stu-id="f9926-126">String</span></span>|<span data-ttu-id="f9926-127">本地化策略名称。</span><span class="sxs-lookup"><span data-stu-id="f9926-127">The localized policy name.</span></span>|
|<span data-ttu-id="f9926-128">explainText</span><span class="sxs-lookup"><span data-stu-id="f9926-128">explainText</span></span>|<span data-ttu-id="f9926-129">String</span><span class="sxs-lookup"><span data-stu-id="f9926-129">String</span></span>|<span data-ttu-id="f9926-130">与策略关联的本地化说明或帮助文本。</span><span class="sxs-lookup"><span data-stu-id="f9926-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="f9926-131">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="f9926-131">The default value is empty.</span></span>|
|<span data-ttu-id="f9926-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="f9926-132">categoryPath</span></span>|<span data-ttu-id="f9926-133">String</span><span class="sxs-lookup"><span data-stu-id="f9926-133">String</span></span>|<span data-ttu-id="f9926-134">策略的本地化完整类别路径。</span><span class="sxs-lookup"><span data-stu-id="f9926-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="f9926-135">supportedOn</span><span class="sxs-lookup"><span data-stu-id="f9926-135">supportedOn</span></span>|<span data-ttu-id="f9926-136">String</span><span class="sxs-lookup"><span data-stu-id="f9926-136">String</span></span>|<span data-ttu-id="f9926-137">用于指定受策略影响的操作系统或应用程序版本的本地化字符串。</span><span class="sxs-lookup"><span data-stu-id="f9926-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="f9926-138">policyType</span><span class="sxs-lookup"><span data-stu-id="f9926-138">policyType</span></span>|[<span data-ttu-id="f9926-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="f9926-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="f9926-140">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="f9926-140">Specifies the type of group policy.</span></span> <span data-ttu-id="f9926-141">可能的值是：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="f9926-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="f9926-142">id</span><span class="sxs-lookup"><span data-stu-id="f9926-142">id</span></span>|<span data-ttu-id="f9926-143">String</span><span class="sxs-lookup"><span data-stu-id="f9926-143">String</span></span>|<span data-ttu-id="f9926-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9926-144">Key of the entity.</span></span>|
|<span data-ttu-id="f9926-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9926-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f9926-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9926-146">DateTimeOffset</span></span>|<span data-ttu-id="f9926-147">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f9926-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9926-148">关系</span><span class="sxs-lookup"><span data-stu-id="f9926-148">Relationships</span></span>
|<span data-ttu-id="f9926-149">关系</span><span class="sxs-lookup"><span data-stu-id="f9926-149">Relationship</span></span>|<span data-ttu-id="f9926-150">类型</span><span class="sxs-lookup"><span data-stu-id="f9926-150">Type</span></span>|<span data-ttu-id="f9926-151">说明</span><span class="sxs-lookup"><span data-stu-id="f9926-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9926-152">definitionFile</span><span class="sxs-lookup"><span data-stu-id="f9926-152">definitionFile</span></span>|[<span data-ttu-id="f9926-153">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="f9926-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="f9926-154">与定义关联的组策略文件。</span><span class="sxs-lookup"><span data-stu-id="f9926-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="f9926-155">文稿</span><span class="sxs-lookup"><span data-stu-id="f9926-155">presentations</span></span>|<span data-ttu-id="f9926-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9926-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="f9926-157">与定义关联的组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="f9926-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9926-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9926-158">JSON Representation</span></span>
<span data-ttu-id="f9926-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9926-159">Here is a JSON representation of the resource.</span></span>
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




