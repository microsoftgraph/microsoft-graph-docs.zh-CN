---
title: deviceManagementTemplate 资源类型
description: 表示已定义的设备设置集合的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ee94a6b74b3eae69f2c6bccbea9ccb13831cdb14
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539069"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="e5b99-103">deviceManagementTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5b99-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="e5b99-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5b99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5b99-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5b99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5b99-106">表示已定义的设备设置集合的实体</span><span class="sxs-lookup"><span data-stu-id="e5b99-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="e5b99-107">方法</span><span class="sxs-lookup"><span data-stu-id="e5b99-107">Methods</span></span>
|<span data-ttu-id="e5b99-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5b99-108">Method</span></span>|<span data-ttu-id="e5b99-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5b99-109">Return Type</span></span>|<span data-ttu-id="e5b99-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5b99-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5b99-111">列出 deviceManagementTemplates</span><span class="sxs-lookup"><span data-stu-id="e5b99-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="e5b99-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="e5b99-113">列出[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5b99-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="e5b99-114">获取 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e5b99-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="e5b99-115">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e5b99-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="e5b99-116">读取[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5b99-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="e5b99-117">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e5b99-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="e5b99-118">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e5b99-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="e5b99-119">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5b99-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="e5b99-120">删除 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e5b99-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="e5b99-121">无</span><span class="sxs-lookup"><span data-stu-id="e5b99-121">None</span></span>|<span data-ttu-id="e5b99-122">删除[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="e5b99-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="e5b99-123">更新 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e5b99-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="e5b99-124">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="e5b99-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="e5b99-125">更新[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5b99-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="e5b99-126">createInstance 操作</span><span class="sxs-lookup"><span data-stu-id="e5b99-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="e5b99-127">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="e5b99-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="e5b99-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e5b99-128">Not yet documented</span></span>|
|[<span data-ttu-id="e5b99-129">compare 函数</span><span class="sxs-lookup"><span data-stu-id="e5b99-129">compare function</span></span>](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|<span data-ttu-id="e5b99-130">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-130">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection</span></span>|<span data-ttu-id="e5b99-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e5b99-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e5b99-132">属性</span><span class="sxs-lookup"><span data-stu-id="e5b99-132">Properties</span></span>
|<span data-ttu-id="e5b99-133">属性</span><span class="sxs-lookup"><span data-stu-id="e5b99-133">Property</span></span>|<span data-ttu-id="e5b99-134">类型</span><span class="sxs-lookup"><span data-stu-id="e5b99-134">Type</span></span>|<span data-ttu-id="e5b99-135">说明</span><span class="sxs-lookup"><span data-stu-id="e5b99-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b99-136">id</span><span class="sxs-lookup"><span data-stu-id="e5b99-136">id</span></span>|<span data-ttu-id="e5b99-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b99-137">String</span></span>|<span data-ttu-id="e5b99-138">模板 ID</span><span class="sxs-lookup"><span data-stu-id="e5b99-138">The template ID</span></span>|
|<span data-ttu-id="e5b99-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e5b99-139">displayName</span></span>|<span data-ttu-id="e5b99-140">String</span><span class="sxs-lookup"><span data-stu-id="e5b99-140">String</span></span>|<span data-ttu-id="e5b99-141">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="e5b99-141">The template's display name</span></span>|
|<span data-ttu-id="e5b99-142">说明</span><span class="sxs-lookup"><span data-stu-id="e5b99-142">description</span></span>|<span data-ttu-id="e5b99-143">String</span><span class="sxs-lookup"><span data-stu-id="e5b99-143">String</span></span>|<span data-ttu-id="e5b99-144">模板的说明</span><span class="sxs-lookup"><span data-stu-id="e5b99-144">The template's description</span></span>|
|<span data-ttu-id="e5b99-145">versionInfo</span><span class="sxs-lookup"><span data-stu-id="e5b99-145">versionInfo</span></span>|<span data-ttu-id="e5b99-146">字符串</span><span class="sxs-lookup"><span data-stu-id="e5b99-146">String</span></span>|<span data-ttu-id="e5b99-147">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="e5b99-147">The template's version information</span></span>|
|<span data-ttu-id="e5b99-148">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="e5b99-148">isDeprecated</span></span>|<span data-ttu-id="e5b99-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b99-149">Boolean</span></span>|<span data-ttu-id="e5b99-150">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="e5b99-150">The template is deprecated or not.</span></span> <span data-ttu-id="e5b99-151">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="e5b99-151">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="e5b99-152">intentCount</span><span class="sxs-lookup"><span data-stu-id="e5b99-152">intentCount</span></span>|<span data-ttu-id="e5b99-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b99-153">Int32</span></span>|<span data-ttu-id="e5b99-154">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="e5b99-154">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="e5b99-155">templateType</span><span class="sxs-lookup"><span data-stu-id="e5b99-155">templateType</span></span>|[<span data-ttu-id="e5b99-156">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="e5b99-156">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="e5b99-157">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="e5b99-157">The template's type.</span></span> <span data-ttu-id="e5b99-158">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`。</span><span class="sxs-lookup"><span data-stu-id="e5b99-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span></span>|
|<span data-ttu-id="e5b99-159">platformType</span><span class="sxs-lookup"><span data-stu-id="e5b99-159">platformType</span></span>|[<span data-ttu-id="e5b99-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="e5b99-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="e5b99-161">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="e5b99-161">The template's platform.</span></span> <span data-ttu-id="e5b99-162">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="e5b99-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="e5b99-163">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b99-163">publishedDateTime</span></span>|<span data-ttu-id="e5b99-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b99-164">DateTimeOffset</span></span>|<span data-ttu-id="e5b99-165">发布模板时</span><span class="sxs-lookup"><span data-stu-id="e5b99-165">When the template was published</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5b99-166">关系</span><span class="sxs-lookup"><span data-stu-id="e5b99-166">Relationships</span></span>
|<span data-ttu-id="e5b99-167">关系</span><span class="sxs-lookup"><span data-stu-id="e5b99-167">Relationship</span></span>|<span data-ttu-id="e5b99-168">类型</span><span class="sxs-lookup"><span data-stu-id="e5b99-168">Type</span></span>|<span data-ttu-id="e5b99-169">说明</span><span class="sxs-lookup"><span data-stu-id="e5b99-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b99-170">settings</span><span class="sxs-lookup"><span data-stu-id="e5b99-170">settings</span></span>|<span data-ttu-id="e5b99-171">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-171">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="e5b99-172">此模板包含的所有设置的集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-172">Collection of all settings this template has</span></span>|
|<span data-ttu-id="e5b99-173">类别</span><span class="sxs-lookup"><span data-stu-id="e5b99-173">categories</span></span>|<span data-ttu-id="e5b99-174">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-174">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="e5b99-175">模板中设置类别的集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-175">Collection of setting categories within the template</span></span>|
|<span data-ttu-id="e5b99-176">migratableTo</span><span class="sxs-lookup"><span data-stu-id="e5b99-176">migratableTo</span></span>|<span data-ttu-id="e5b99-177">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-177">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="e5b99-178">此模板可以迁移到的模板集合</span><span class="sxs-lookup"><span data-stu-id="e5b99-178">Collection of templates this template can migrate to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5b99-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5b99-179">JSON Representation</span></span>
<span data-ttu-id="e5b99-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5b99-180">Here is a JSON representation of the resource.</span></span>
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
  "platformType": "String",
  "publishedDateTime": "String (timestamp)"
}
```



