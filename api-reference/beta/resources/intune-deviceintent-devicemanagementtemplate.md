---
title: deviceManagementTemplate 资源类型
description: 表示已定义的设备设置集合的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 438fbf37cb419145d63b8d25f9e8145005eac6cc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984413"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="d3cff-103">deviceManagementTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3cff-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="d3cff-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3cff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3cff-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3cff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3cff-106">表示已定义的设备设置集合的实体</span><span class="sxs-lookup"><span data-stu-id="d3cff-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="d3cff-107">方法</span><span class="sxs-lookup"><span data-stu-id="d3cff-107">Methods</span></span>
|<span data-ttu-id="d3cff-108">方法</span><span class="sxs-lookup"><span data-stu-id="d3cff-108">Method</span></span>|<span data-ttu-id="d3cff-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3cff-109">Return Type</span></span>|<span data-ttu-id="d3cff-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3cff-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3cff-111">列出 deviceManagementTemplates</span><span class="sxs-lookup"><span data-stu-id="d3cff-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="d3cff-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="d3cff-113">列出[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3cff-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="d3cff-114">获取 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3cff-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="d3cff-115">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3cff-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="d3cff-116">读取[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3cff-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="d3cff-117">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3cff-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="d3cff-118">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3cff-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="d3cff-119">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d3cff-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="d3cff-120">删除 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3cff-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="d3cff-121">无</span><span class="sxs-lookup"><span data-stu-id="d3cff-121">None</span></span>|<span data-ttu-id="d3cff-122">删除[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="d3cff-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="d3cff-123">更新 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3cff-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="d3cff-124">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="d3cff-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="d3cff-125">更新[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3cff-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="d3cff-126">createInstance 操作</span><span class="sxs-lookup"><span data-stu-id="d3cff-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="d3cff-127">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="d3cff-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="d3cff-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d3cff-128">Not yet documented</span></span>|
|[<span data-ttu-id="d3cff-129">compare 函数</span><span class="sxs-lookup"><span data-stu-id="d3cff-129">compare function</span></span>](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|<span data-ttu-id="d3cff-130">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-130">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection</span></span>|<span data-ttu-id="d3cff-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d3cff-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d3cff-132">属性</span><span class="sxs-lookup"><span data-stu-id="d3cff-132">Properties</span></span>
|<span data-ttu-id="d3cff-133">属性</span><span class="sxs-lookup"><span data-stu-id="d3cff-133">Property</span></span>|<span data-ttu-id="d3cff-134">类型</span><span class="sxs-lookup"><span data-stu-id="d3cff-134">Type</span></span>|<span data-ttu-id="d3cff-135">说明</span><span class="sxs-lookup"><span data-stu-id="d3cff-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3cff-136">id</span><span class="sxs-lookup"><span data-stu-id="d3cff-136">id</span></span>|<span data-ttu-id="d3cff-137">字符串</span><span class="sxs-lookup"><span data-stu-id="d3cff-137">String</span></span>|<span data-ttu-id="d3cff-138">模板 ID</span><span class="sxs-lookup"><span data-stu-id="d3cff-138">The template ID</span></span>|
|<span data-ttu-id="d3cff-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d3cff-139">displayName</span></span>|<span data-ttu-id="d3cff-140">String</span><span class="sxs-lookup"><span data-stu-id="d3cff-140">String</span></span>|<span data-ttu-id="d3cff-141">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="d3cff-141">The template's display name</span></span>|
|<span data-ttu-id="d3cff-142">说明</span><span class="sxs-lookup"><span data-stu-id="d3cff-142">description</span></span>|<span data-ttu-id="d3cff-143">String</span><span class="sxs-lookup"><span data-stu-id="d3cff-143">String</span></span>|<span data-ttu-id="d3cff-144">模板的说明</span><span class="sxs-lookup"><span data-stu-id="d3cff-144">The template's description</span></span>|
|<span data-ttu-id="d3cff-145">versionInfo</span><span class="sxs-lookup"><span data-stu-id="d3cff-145">versionInfo</span></span>|<span data-ttu-id="d3cff-146">String</span><span class="sxs-lookup"><span data-stu-id="d3cff-146">String</span></span>|<span data-ttu-id="d3cff-147">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="d3cff-147">The template's version information</span></span>|
|<span data-ttu-id="d3cff-148">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="d3cff-148">isDeprecated</span></span>|<span data-ttu-id="d3cff-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3cff-149">Boolean</span></span>|<span data-ttu-id="d3cff-150">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="d3cff-150">The template is deprecated or not.</span></span> <span data-ttu-id="d3cff-151">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="d3cff-151">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="d3cff-152">intentCount</span><span class="sxs-lookup"><span data-stu-id="d3cff-152">intentCount</span></span>|<span data-ttu-id="d3cff-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d3cff-153">Int32</span></span>|<span data-ttu-id="d3cff-154">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="d3cff-154">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="d3cff-155">templateType</span><span class="sxs-lookup"><span data-stu-id="d3cff-155">templateType</span></span>|[<span data-ttu-id="d3cff-156">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="d3cff-156">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="d3cff-157">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="d3cff-157">The template's type.</span></span> <span data-ttu-id="d3cff-158">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="d3cff-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.</span></span>|
|<span data-ttu-id="d3cff-159">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3cff-159">publishedDateTime</span></span>|<span data-ttu-id="d3cff-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3cff-160">DateTimeOffset</span></span>|<span data-ttu-id="d3cff-161">发布模板时</span><span class="sxs-lookup"><span data-stu-id="d3cff-161">When the template was published</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3cff-162">关系</span><span class="sxs-lookup"><span data-stu-id="d3cff-162">Relationships</span></span>
|<span data-ttu-id="d3cff-163">关系</span><span class="sxs-lookup"><span data-stu-id="d3cff-163">Relationship</span></span>|<span data-ttu-id="d3cff-164">类型</span><span class="sxs-lookup"><span data-stu-id="d3cff-164">Type</span></span>|<span data-ttu-id="d3cff-165">说明</span><span class="sxs-lookup"><span data-stu-id="d3cff-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3cff-166">settings</span><span class="sxs-lookup"><span data-stu-id="d3cff-166">settings</span></span>|<span data-ttu-id="d3cff-167">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-167">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="d3cff-168">此模板包含的所有设置的集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-168">Collection of all settings this template has</span></span>|
|<span data-ttu-id="d3cff-169">categories</span><span class="sxs-lookup"><span data-stu-id="d3cff-169">categories</span></span>|<span data-ttu-id="d3cff-170">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-170">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="d3cff-171">模板中设置类别的集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-171">Collection of setting categories within the template</span></span>|
|<span data-ttu-id="d3cff-172">migratableTo</span><span class="sxs-lookup"><span data-stu-id="d3cff-172">migratableTo</span></span>|<span data-ttu-id="d3cff-173">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-173">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="d3cff-174">此模板可以迁移到的模板集合</span><span class="sxs-lookup"><span data-stu-id="d3cff-174">Collection of templates this template can migrate to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3cff-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3cff-175">JSON Representation</span></span>
<span data-ttu-id="d3cff-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3cff-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "publishedDateTime": "String (timestamp)"
}
```





