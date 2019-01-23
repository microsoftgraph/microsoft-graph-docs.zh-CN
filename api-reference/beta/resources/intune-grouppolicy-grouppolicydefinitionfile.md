---
title: groupPolicyDefinitionFile 资源类型
description: 实体表示 ADMX （管理模板） XML 文件。 ADMX 文件包含类别路径其位置和组策略定义的集合。 组策略定义文件还包含由语言相关 ADML （管理模板） 语言文件支持的语言。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431351"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="d107b-105">groupPolicyDefinitionFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="d107b-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="d107b-106">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d107b-106">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d107b-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d107b-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d107b-108">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d107b-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d107b-109">实体表示 ADMX （管理模板） XML 文件。</span><span class="sxs-lookup"><span data-stu-id="d107b-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="d107b-110">ADMX 文件包含类别路径其位置和组策略定义的集合。</span><span class="sxs-lookup"><span data-stu-id="d107b-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="d107b-111">组策略定义文件还包含由语言相关 ADML （管理模板） 语言文件支持的语言。</span><span class="sxs-lookup"><span data-stu-id="d107b-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="d107b-112">方法</span><span class="sxs-lookup"><span data-stu-id="d107b-112">Methods</span></span>
|<span data-ttu-id="d107b-113">方法</span><span class="sxs-lookup"><span data-stu-id="d107b-113">Method</span></span>|<span data-ttu-id="d107b-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="d107b-114">Return Type</span></span>|<span data-ttu-id="d107b-115">说明</span><span class="sxs-lookup"><span data-stu-id="d107b-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d107b-116">获取 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="d107b-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="d107b-117">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="d107b-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="d107b-118">读取属性和[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d107b-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="d107b-119">更新 groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="d107b-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="d107b-120">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="d107b-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="d107b-121">更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d107b-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d107b-122">属性</span><span class="sxs-lookup"><span data-stu-id="d107b-122">Properties</span></span>
|<span data-ttu-id="d107b-123">属性</span><span class="sxs-lookup"><span data-stu-id="d107b-123">Property</span></span>|<span data-ttu-id="d107b-124">类型</span><span class="sxs-lookup"><span data-stu-id="d107b-124">Type</span></span>|<span data-ttu-id="d107b-125">说明</span><span class="sxs-lookup"><span data-stu-id="d107b-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d107b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d107b-126">displayName</span></span>|<span data-ttu-id="d107b-127">String</span><span class="sxs-lookup"><span data-stu-id="d107b-127">String</span></span>|<span data-ttu-id="d107b-128">ADMX 文件的本地化的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d107b-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="d107b-129">说明</span><span class="sxs-lookup"><span data-stu-id="d107b-129">description</span></span>|<span data-ttu-id="d107b-130">String</span><span class="sxs-lookup"><span data-stu-id="d107b-130">String</span></span>|<span data-ttu-id="d107b-131">ADMX 文件中的策略设置的本地化的描述。</span><span class="sxs-lookup"><span data-stu-id="d107b-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="d107b-132">默认值为空。</span><span class="sxs-lookup"><span data-stu-id="d107b-132">The default value is empty.</span></span>|
|<span data-ttu-id="d107b-133">languageCodes</span><span class="sxs-lookup"><span data-stu-id="d107b-133">languageCodes</span></span>|<span data-ttu-id="d107b-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="d107b-134">String collection</span></span>|<span data-ttu-id="d107b-135">ADMX 文件的受支持的语言代码。</span><span class="sxs-lookup"><span data-stu-id="d107b-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="d107b-136">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="d107b-136">targetPrefix</span></span>|<span data-ttu-id="d107b-137">String</span><span class="sxs-lookup"><span data-stu-id="d107b-137">String</span></span>|<span data-ttu-id="d107b-138">指定引用 ADMX 文件中的命名空间的逻辑名称。</span><span class="sxs-lookup"><span data-stu-id="d107b-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="d107b-139">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="d107b-139">targetNamespace</span></span>|<span data-ttu-id="d107b-140">String</span><span class="sxs-lookup"><span data-stu-id="d107b-140">String</span></span>|<span data-ttu-id="d107b-141">指定用于标识 ADMX 文件中的命名空间的 URI。</span><span class="sxs-lookup"><span data-stu-id="d107b-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="d107b-142">policyType</span><span class="sxs-lookup"><span data-stu-id="d107b-142">policyType</span></span>|[<span data-ttu-id="d107b-143">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="d107b-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="d107b-144">指定的组策略的类型。</span><span class="sxs-lookup"><span data-stu-id="d107b-144">Specifies the type of group policy.</span></span> <span data-ttu-id="d107b-145">可取值为：`admxBacked`、`admxIngested`。</span><span class="sxs-lookup"><span data-stu-id="d107b-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="d107b-146">id</span><span class="sxs-lookup"><span data-stu-id="d107b-146">id</span></span>|<span data-ttu-id="d107b-147">String</span><span class="sxs-lookup"><span data-stu-id="d107b-147">String</span></span>|<span data-ttu-id="d107b-148">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d107b-148">Key of the entity.</span></span>|
|<span data-ttu-id="d107b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d107b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d107b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d107b-150">DateTimeOffset</span></span>|<span data-ttu-id="d107b-151">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="d107b-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d107b-152">关系</span><span class="sxs-lookup"><span data-stu-id="d107b-152">Relationships</span></span>
|<span data-ttu-id="d107b-153">关系</span><span class="sxs-lookup"><span data-stu-id="d107b-153">Relationship</span></span>|<span data-ttu-id="d107b-154">类型</span><span class="sxs-lookup"><span data-stu-id="d107b-154">Type</span></span>|<span data-ttu-id="d107b-155">说明</span><span class="sxs-lookup"><span data-stu-id="d107b-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d107b-156">定义</span><span class="sxs-lookup"><span data-stu-id="d107b-156">definitions</span></span>|<span data-ttu-id="d107b-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="d107b-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="d107b-158">组策略定义与文件关联。</span><span class="sxs-lookup"><span data-stu-id="d107b-158">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d107b-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d107b-159">JSON Representation</span></span>
<span data-ttu-id="d107b-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d107b-160">Here is a JSON representation of the resource.</span></span>
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




