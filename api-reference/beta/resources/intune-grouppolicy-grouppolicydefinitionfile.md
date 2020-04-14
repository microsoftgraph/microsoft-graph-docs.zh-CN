---
title: groupPolicyDefinitionFile 资源类型
description: 实体表示 ADMX （管理模板） XML 文件。 ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。 组策略定义文件还包含由语言相关 ADML （管理模板）语言文件所确定的受支持的语言。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 821acf4f14602ea622b03b310b12a1e5f8269395
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448081"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="03d48-105">groupPolicyDefinitionFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="03d48-105">groupPolicyDefinitionFile resource type</span></span>

<span data-ttu-id="03d48-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03d48-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03d48-107">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03d48-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03d48-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03d48-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03d48-109">实体表示 ADMX （管理模板） XML 文件。</span><span class="sxs-lookup"><span data-stu-id="03d48-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="03d48-110">ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。</span><span class="sxs-lookup"><span data-stu-id="03d48-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="03d48-111">组策略定义文件还包含由语言相关 ADML （管理模板）语言文件所确定的受支持的语言。</span><span class="sxs-lookup"><span data-stu-id="03d48-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="03d48-112">方法</span><span class="sxs-lookup"><span data-stu-id="03d48-112">Methods</span></span>
|<span data-ttu-id="03d48-113">方法</span><span class="sxs-lookup"><span data-stu-id="03d48-113">Method</span></span>|<span data-ttu-id="03d48-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="03d48-114">Return Type</span></span>|<span data-ttu-id="03d48-115">说明</span><span class="sxs-lookup"><span data-stu-id="03d48-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03d48-116">获取 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="03d48-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="03d48-117">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="03d48-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="03d48-118">读取[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03d48-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="03d48-119">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="03d48-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="03d48-120">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="03d48-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="03d48-121">更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03d48-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="03d48-122">属性</span><span class="sxs-lookup"><span data-stu-id="03d48-122">Properties</span></span>
|<span data-ttu-id="03d48-123">属性</span><span class="sxs-lookup"><span data-stu-id="03d48-123">Property</span></span>|<span data-ttu-id="03d48-124">类型</span><span class="sxs-lookup"><span data-stu-id="03d48-124">Type</span></span>|<span data-ttu-id="03d48-125">说明</span><span class="sxs-lookup"><span data-stu-id="03d48-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03d48-126">displayName</span><span class="sxs-lookup"><span data-stu-id="03d48-126">displayName</span></span>|<span data-ttu-id="03d48-127">String</span><span class="sxs-lookup"><span data-stu-id="03d48-127">String</span></span>|<span data-ttu-id="03d48-128">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="03d48-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="03d48-129">description</span><span class="sxs-lookup"><span data-stu-id="03d48-129">description</span></span>|<span data-ttu-id="03d48-130">String</span><span class="sxs-lookup"><span data-stu-id="03d48-130">String</span></span>|<span data-ttu-id="03d48-131">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="03d48-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="03d48-132">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="03d48-132">The default value is empty.</span></span>|
|<span data-ttu-id="03d48-133">languageCodes</span><span class="sxs-lookup"><span data-stu-id="03d48-133">languageCodes</span></span>|<span data-ttu-id="03d48-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="03d48-134">String collection</span></span>|<span data-ttu-id="03d48-135">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="03d48-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="03d48-136">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="03d48-136">targetPrefix</span></span>|<span data-ttu-id="03d48-137">String</span><span class="sxs-lookup"><span data-stu-id="03d48-137">String</span></span>|<span data-ttu-id="03d48-138">指定在 ADMX 文件中引用命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="03d48-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="03d48-139">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="03d48-139">targetNamespace</span></span>|<span data-ttu-id="03d48-140">String</span><span class="sxs-lookup"><span data-stu-id="03d48-140">String</span></span>|<span data-ttu-id="03d48-141">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="03d48-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="03d48-142">policyType</span><span class="sxs-lookup"><span data-stu-id="03d48-142">policyType</span></span>|[<span data-ttu-id="03d48-143">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="03d48-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="03d48-144">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="03d48-144">Specifies the type of group policy.</span></span> <span data-ttu-id="03d48-145">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="03d48-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="03d48-146">a01</span><span class="sxs-lookup"><span data-stu-id="03d48-146">revision</span></span>|<span data-ttu-id="03d48-147">String</span><span class="sxs-lookup"><span data-stu-id="03d48-147">String</span></span>|<span data-ttu-id="03d48-148">与文件关联的修订版本。</span><span class="sxs-lookup"><span data-stu-id="03d48-148">The revision version associated with the file.</span></span>|
|<span data-ttu-id="03d48-149">id</span><span class="sxs-lookup"><span data-stu-id="03d48-149">id</span></span>|<span data-ttu-id="03d48-150">字符串</span><span class="sxs-lookup"><span data-stu-id="03d48-150">String</span></span>|<span data-ttu-id="03d48-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="03d48-151">Key of the entity.</span></span>|
|<span data-ttu-id="03d48-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03d48-152">lastModifiedDateTime</span></span>|<span data-ttu-id="03d48-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03d48-153">DateTimeOffset</span></span>|<span data-ttu-id="03d48-154">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="03d48-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03d48-155">关系</span><span class="sxs-lookup"><span data-stu-id="03d48-155">Relationships</span></span>
|<span data-ttu-id="03d48-156">关系</span><span class="sxs-lookup"><span data-stu-id="03d48-156">Relationship</span></span>|<span data-ttu-id="03d48-157">类型</span><span class="sxs-lookup"><span data-stu-id="03d48-157">Type</span></span>|<span data-ttu-id="03d48-158">说明</span><span class="sxs-lookup"><span data-stu-id="03d48-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03d48-159">限定</span><span class="sxs-lookup"><span data-stu-id="03d48-159">definitions</span></span>|<span data-ttu-id="03d48-160">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="03d48-160">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="03d48-161">与文件相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="03d48-161">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03d48-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03d48-162">JSON Representation</span></span>
<span data-ttu-id="03d48-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03d48-163">Here is a JSON representation of the resource.</span></span>
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
  "revision": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



