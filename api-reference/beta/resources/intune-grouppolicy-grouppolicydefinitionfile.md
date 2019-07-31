---
title: groupPolicyDefinitionFile 资源类型
description: 实体表示 ADMX (管理模板) XML 文件。 ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。 组策略定义文件还包含由语言相关 ADML (管理模板) 语言文件所确定的受支持的语言。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60001517f635352ea2717033279ebebc8df7895b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998623"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="fce47-105">groupPolicyDefinitionFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="fce47-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="fce47-106">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fce47-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fce47-107">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fce47-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fce47-108">实体表示 ADMX (管理模板) XML 文件。</span><span class="sxs-lookup"><span data-stu-id="fce47-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="fce47-109">ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。</span><span class="sxs-lookup"><span data-stu-id="fce47-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="fce47-110">组策略定义文件还包含由语言相关 ADML (管理模板) 语言文件所确定的受支持的语言。</span><span class="sxs-lookup"><span data-stu-id="fce47-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="fce47-111">方法</span><span class="sxs-lookup"><span data-stu-id="fce47-111">Methods</span></span>
|<span data-ttu-id="fce47-112">方法</span><span class="sxs-lookup"><span data-stu-id="fce47-112">Method</span></span>|<span data-ttu-id="fce47-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="fce47-113">Return Type</span></span>|<span data-ttu-id="fce47-114">说明</span><span class="sxs-lookup"><span data-stu-id="fce47-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fce47-115">获取 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="fce47-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="fce47-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="fce47-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="fce47-117">读取[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fce47-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="fce47-118">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="fce47-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="fce47-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="fce47-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="fce47-120">更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fce47-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fce47-121">属性</span><span class="sxs-lookup"><span data-stu-id="fce47-121">Properties</span></span>
|<span data-ttu-id="fce47-122">属性</span><span class="sxs-lookup"><span data-stu-id="fce47-122">Property</span></span>|<span data-ttu-id="fce47-123">类型</span><span class="sxs-lookup"><span data-stu-id="fce47-123">Type</span></span>|<span data-ttu-id="fce47-124">说明</span><span class="sxs-lookup"><span data-stu-id="fce47-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce47-125">displayName</span><span class="sxs-lookup"><span data-stu-id="fce47-125">displayName</span></span>|<span data-ttu-id="fce47-126">String</span><span class="sxs-lookup"><span data-stu-id="fce47-126">String</span></span>|<span data-ttu-id="fce47-127">ADMX 文件的本地化友好名称。</span><span class="sxs-lookup"><span data-stu-id="fce47-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="fce47-128">说明</span><span class="sxs-lookup"><span data-stu-id="fce47-128">description</span></span>|<span data-ttu-id="fce47-129">String</span><span class="sxs-lookup"><span data-stu-id="fce47-129">String</span></span>|<span data-ttu-id="fce47-130">ADMX 文件中策略设置的本地化说明。</span><span class="sxs-lookup"><span data-stu-id="fce47-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="fce47-131">默认值为空白。</span><span class="sxs-lookup"><span data-stu-id="fce47-131">The default value is empty.</span></span>|
|<span data-ttu-id="fce47-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="fce47-132">languageCodes</span></span>|<span data-ttu-id="fce47-133">String collection</span><span class="sxs-lookup"><span data-stu-id="fce47-133">String collection</span></span>|<span data-ttu-id="fce47-134">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="fce47-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="fce47-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="fce47-135">targetPrefix</span></span>|<span data-ttu-id="fce47-136">String</span><span class="sxs-lookup"><span data-stu-id="fce47-136">String</span></span>|<span data-ttu-id="fce47-137">指定在 ADMX 文件中引用命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="fce47-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="fce47-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="fce47-138">targetNamespace</span></span>|<span data-ttu-id="fce47-139">String</span><span class="sxs-lookup"><span data-stu-id="fce47-139">String</span></span>|<span data-ttu-id="fce47-140">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="fce47-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="fce47-141">policyType</span><span class="sxs-lookup"><span data-stu-id="fce47-141">policyType</span></span>|[<span data-ttu-id="fce47-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="fce47-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="fce47-143">指定组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="fce47-143">Specifies the type of group policy.</span></span> <span data-ttu-id="fce47-144">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="fce47-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="fce47-145">a01</span><span class="sxs-lookup"><span data-stu-id="fce47-145">revision</span></span>|<span data-ttu-id="fce47-146">String</span><span class="sxs-lookup"><span data-stu-id="fce47-146">String</span></span>|<span data-ttu-id="fce47-147">与文件关联的修订版本。</span><span class="sxs-lookup"><span data-stu-id="fce47-147">The revision version associated with the file.</span></span>|
|<span data-ttu-id="fce47-148">id</span><span class="sxs-lookup"><span data-stu-id="fce47-148">id</span></span>|<span data-ttu-id="fce47-149">字符串</span><span class="sxs-lookup"><span data-stu-id="fce47-149">String</span></span>|<span data-ttu-id="fce47-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fce47-150">Key of the entity.</span></span>|
|<span data-ttu-id="fce47-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fce47-151">lastModifiedDateTime</span></span>|<span data-ttu-id="fce47-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fce47-152">DateTimeOffset</span></span>|<span data-ttu-id="fce47-153">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fce47-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fce47-154">关系</span><span class="sxs-lookup"><span data-stu-id="fce47-154">Relationships</span></span>
|<span data-ttu-id="fce47-155">关系</span><span class="sxs-lookup"><span data-stu-id="fce47-155">Relationship</span></span>|<span data-ttu-id="fce47-156">类型</span><span class="sxs-lookup"><span data-stu-id="fce47-156">Type</span></span>|<span data-ttu-id="fce47-157">说明</span><span class="sxs-lookup"><span data-stu-id="fce47-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce47-158">限定</span><span class="sxs-lookup"><span data-stu-id="fce47-158">definitions</span></span>|<span data-ttu-id="fce47-159">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="fce47-159">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="fce47-160">与文件相关联的组策略定义。</span><span class="sxs-lookup"><span data-stu-id="fce47-160">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fce47-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fce47-161">JSON Representation</span></span>
<span data-ttu-id="fce47-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fce47-162">Here is a JSON representation of the resource.</span></span>
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





