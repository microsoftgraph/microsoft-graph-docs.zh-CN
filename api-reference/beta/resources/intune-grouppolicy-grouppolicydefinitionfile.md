---
title: groupPolicyDefinitionFile 资源类型
description: 实体表示 ADMX (管理模板) XML 文件。 ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。 组策略定义文件还包含由语言相关 ADML (管理模板) 语言文件所确定的受支持的语言。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 494a2f8ff80b3a7f8ee9db9fea4d795494c19a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161332"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="8fba6-105">groupPolicyDefinitionFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fba6-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="8fba6-106">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8fba6-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fba6-107">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fba6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fba6-108">实体表示 ADMX (管理模板) XML 文件。</span><span class="sxs-lookup"><span data-stu-id="8fba6-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="8fba6-109">ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。</span><span class="sxs-lookup"><span data-stu-id="8fba6-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="8fba6-110">组策略定义文件还包含由语言相关 ADML (管理模板) 语言文件所确定的受支持的语言。</span><span class="sxs-lookup"><span data-stu-id="8fba6-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="8fba6-111">方法</span><span class="sxs-lookup"><span data-stu-id="8fba6-111">Methods</span></span>
|<span data-ttu-id="8fba6-112">方法</span><span class="sxs-lookup"><span data-stu-id="8fba6-112">Method</span></span>|<span data-ttu-id="8fba6-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="8fba6-113">Return Type</span></span>|<span data-ttu-id="8fba6-114">说明</span><span class="sxs-lookup"><span data-stu-id="8fba6-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8fba6-115">获取 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="8fba6-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="8fba6-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="8fba6-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="8fba6-117">读取[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8fba6-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="8fba6-118">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="8fba6-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="8fba6-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="8fba6-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="8fba6-120">更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8fba6-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fba6-121">属性</span><span class="sxs-lookup"><span data-stu-id="8fba6-121">Properties</span></span>
|<span data-ttu-id="8fba6-122">属性</span><span class="sxs-lookup"><span data-stu-id="8fba6-122">Property</span></span>|<span data-ttu-id="8fba6-123">类型</span><span class="sxs-lookup"><span data-stu-id="8fba6-123">Type</span></span>|<span data-ttu-id="8fba6-124">说明</span><span class="sxs-lookup"><span data-stu-id="8fba6-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fba6-125">displayName</span><span class="sxs-lookup"><span data-stu-id="8fba6-125">displayName</span></span>|<span data-ttu-id="8fba6-126">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-126">String</span></span>|<span data-ttu-id="8fba6-127">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="8fba6-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="8fba6-128">description</span><span class="sxs-lookup"><span data-stu-id="8fba6-128">description</span></span>|<span data-ttu-id="8fba6-129">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-129">String</span></span>|<span data-ttu-id="8fba6-130">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="8fba6-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="8fba6-131">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="8fba6-131">The default value is empty.</span></span>|
|<span data-ttu-id="8fba6-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="8fba6-132">languageCodes</span></span>|<span data-ttu-id="8fba6-133">String collection</span><span class="sxs-lookup"><span data-stu-id="8fba6-133">String collection</span></span>|<span data-ttu-id="8fba6-134">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="8fba6-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="8fba6-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="8fba6-135">targetPrefix</span></span>|<span data-ttu-id="8fba6-136">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-136">String</span></span>|<span data-ttu-id="8fba6-137">指定在 ADMX 文件中引用命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="8fba6-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="8fba6-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="8fba6-138">targetNamespace</span></span>|<span data-ttu-id="8fba6-139">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-139">String</span></span>|<span data-ttu-id="8fba6-140">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="8fba6-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="8fba6-141">policyType</span><span class="sxs-lookup"><span data-stu-id="8fba6-141">policyType</span></span>|[<span data-ttu-id="8fba6-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="8fba6-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="8fba6-143">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="8fba6-143">Specifies the type of group policy.</span></span> <span data-ttu-id="8fba6-144">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="8fba6-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="8fba6-145">id</span><span class="sxs-lookup"><span data-stu-id="8fba6-145">id</span></span>|<span data-ttu-id="8fba6-146">String</span><span class="sxs-lookup"><span data-stu-id="8fba6-146">String</span></span>|<span data-ttu-id="8fba6-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8fba6-147">Key of the entity.</span></span>|
|<span data-ttu-id="8fba6-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fba6-148">lastModifiedDateTime</span></span>|<span data-ttu-id="8fba6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fba6-149">DateTimeOffset</span></span>|<span data-ttu-id="8fba6-150">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8fba6-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fba6-151">关系</span><span class="sxs-lookup"><span data-stu-id="8fba6-151">Relationships</span></span>
|<span data-ttu-id="8fba6-152">关系</span><span class="sxs-lookup"><span data-stu-id="8fba6-152">Relationship</span></span>|<span data-ttu-id="8fba6-153">类型</span><span class="sxs-lookup"><span data-stu-id="8fba6-153">Type</span></span>|<span data-ttu-id="8fba6-154">说明</span><span class="sxs-lookup"><span data-stu-id="8fba6-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fba6-155">定义</span><span class="sxs-lookup"><span data-stu-id="8fba6-155">definitions</span></span>|<span data-ttu-id="8fba6-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="8fba6-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="8fba6-157">与文件相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="8fba6-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fba6-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fba6-158">JSON Representation</span></span>
<span data-ttu-id="8fba6-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fba6-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




