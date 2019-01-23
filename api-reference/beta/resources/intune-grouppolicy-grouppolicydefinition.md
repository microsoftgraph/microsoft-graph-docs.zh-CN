---
title: groupPolicyDefinition 资源类型
description: 实体描述所有单个组策略的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429519"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="0f089-103">groupPolicyDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f089-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="0f089-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0f089-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f089-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f089-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f089-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f089-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f089-107">实体描述所有单个组策略的信息。</span><span class="sxs-lookup"><span data-stu-id="0f089-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="0f089-108">方法</span><span class="sxs-lookup"><span data-stu-id="0f089-108">Methods</span></span>
|<span data-ttu-id="0f089-109">方法</span><span class="sxs-lookup"><span data-stu-id="0f089-109">Method</span></span>|<span data-ttu-id="0f089-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0f089-110">Return Type</span></span>|<span data-ttu-id="0f089-111">说明</span><span class="sxs-lookup"><span data-stu-id="0f089-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f089-112">获取 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0f089-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="0f089-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0f089-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="0f089-114">读取属性和[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0f089-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="0f089-115">更新 groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0f089-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="0f089-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0f089-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="0f089-117">更新[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0f089-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f089-118">属性</span><span class="sxs-lookup"><span data-stu-id="0f089-118">Properties</span></span>
|<span data-ttu-id="0f089-119">属性</span><span class="sxs-lookup"><span data-stu-id="0f089-119">Property</span></span>|<span data-ttu-id="0f089-120">类型</span><span class="sxs-lookup"><span data-stu-id="0f089-120">Type</span></span>|<span data-ttu-id="0f089-121">说明</span><span class="sxs-lookup"><span data-stu-id="0f089-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f089-122">classType</span><span class="sxs-lookup"><span data-stu-id="0f089-122">classType</span></span>|[<span data-ttu-id="0f089-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="0f089-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="0f089-124">标识的组策略可应用于的类型。</span><span class="sxs-lookup"><span data-stu-id="0f089-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="0f089-125">可取值为：`user`、`machine`、`both`。</span><span class="sxs-lookup"><span data-stu-id="0f089-125">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="0f089-126">displayName</span><span class="sxs-lookup"><span data-stu-id="0f089-126">displayName</span></span>|<span data-ttu-id="0f089-127">String</span><span class="sxs-lookup"><span data-stu-id="0f089-127">String</span></span>|<span data-ttu-id="0f089-128">本地化的策略名称。</span><span class="sxs-lookup"><span data-stu-id="0f089-128">The localized policy name.</span></span>|
|<span data-ttu-id="0f089-129">explainText</span><span class="sxs-lookup"><span data-stu-id="0f089-129">explainText</span></span>|<span data-ttu-id="0f089-130">String</span><span class="sxs-lookup"><span data-stu-id="0f089-130">String</span></span>|<span data-ttu-id="0f089-131">本地化的说明或帮助文本与策略相关联。</span><span class="sxs-lookup"><span data-stu-id="0f089-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="0f089-132">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="0f089-132">The default value is empty.</span></span>|
|<span data-ttu-id="0f089-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="0f089-133">categoryPath</span></span>|<span data-ttu-id="0f089-134">String</span><span class="sxs-lookup"><span data-stu-id="0f089-134">String</span></span>|<span data-ttu-id="0f089-135">本地化的完整类别策略路径。</span><span class="sxs-lookup"><span data-stu-id="0f089-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="0f089-136">supportedOn</span><span class="sxs-lookup"><span data-stu-id="0f089-136">supportedOn</span></span>|<span data-ttu-id="0f089-137">String</span><span class="sxs-lookup"><span data-stu-id="0f089-137">String</span></span>|<span data-ttu-id="0f089-138">用于指定哪些操作系统或应用程序版本的本地化的字符串受策略。</span><span class="sxs-lookup"><span data-stu-id="0f089-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="0f089-139">policyType</span><span class="sxs-lookup"><span data-stu-id="0f089-139">policyType</span></span>|[<span data-ttu-id="0f089-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="0f089-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="0f089-141">指定的组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="0f089-141">Specifies the type of group policy.</span></span> <span data-ttu-id="0f089-142">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="0f089-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="0f089-143">id</span><span class="sxs-lookup"><span data-stu-id="0f089-143">id</span></span>|<span data-ttu-id="0f089-144">String</span><span class="sxs-lookup"><span data-stu-id="0f089-144">String</span></span>|<span data-ttu-id="0f089-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f089-145">Key of the entity.</span></span>|
|<span data-ttu-id="0f089-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f089-146">lastModifiedDateTime</span></span>|<span data-ttu-id="0f089-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f089-147">DateTimeOffset</span></span>|<span data-ttu-id="0f089-148">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="0f089-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f089-149">关系</span><span class="sxs-lookup"><span data-stu-id="0f089-149">Relationships</span></span>
|<span data-ttu-id="0f089-150">关系</span><span class="sxs-lookup"><span data-stu-id="0f089-150">Relationship</span></span>|<span data-ttu-id="0f089-151">类型</span><span class="sxs-lookup"><span data-stu-id="0f089-151">Type</span></span>|<span data-ttu-id="0f089-152">说明</span><span class="sxs-lookup"><span data-stu-id="0f089-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f089-153">definitionFile</span><span class="sxs-lookup"><span data-stu-id="0f089-153">definitionFile</span></span>|[<span data-ttu-id="0f089-154">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="0f089-154">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="0f089-155">组策略文件与定义关联。</span><span class="sxs-lookup"><span data-stu-id="0f089-155">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="0f089-156">演示文稿</span><span class="sxs-lookup"><span data-stu-id="0f089-156">presentations</span></span>|<span data-ttu-id="0f089-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f089-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="0f089-158">与定义关联组策略演示文稿。</span><span class="sxs-lookup"><span data-stu-id="0f089-158">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f089-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f089-159">JSON Representation</span></span>
<span data-ttu-id="0f089-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f089-160">Here is a JSON representation of the resource.</span></span>
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




