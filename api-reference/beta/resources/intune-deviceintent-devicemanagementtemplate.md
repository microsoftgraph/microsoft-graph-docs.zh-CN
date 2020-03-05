---
title: deviceManagementTemplate 资源类型
description: 表示已定义的设备设置集合的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a8721af64af42b93d8a60349443b68381ad89f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528761"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="a2464-103">deviceManagementTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2464-103">deviceManagementTemplate resource type</span></span>

<span data-ttu-id="a2464-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a2464-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2464-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2464-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2464-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2464-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2464-107">表示已定义的设备设置集合的实体</span><span class="sxs-lookup"><span data-stu-id="a2464-107">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="a2464-108">方法</span><span class="sxs-lookup"><span data-stu-id="a2464-108">Methods</span></span>
|<span data-ttu-id="a2464-109">方法</span><span class="sxs-lookup"><span data-stu-id="a2464-109">Method</span></span>|<span data-ttu-id="a2464-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2464-110">Return Type</span></span>|<span data-ttu-id="a2464-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2464-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2464-112">列出 deviceManagementTemplates</span><span class="sxs-lookup"><span data-stu-id="a2464-112">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="a2464-113">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2464-113">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="a2464-114">列出[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2464-114">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="a2464-115">获取 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2464-115">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="a2464-116">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2464-116">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="a2464-117">读取[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2464-117">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="a2464-118">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2464-118">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="a2464-119">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2464-119">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="a2464-120">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2464-120">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="a2464-121">删除 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2464-121">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="a2464-122">无</span><span class="sxs-lookup"><span data-stu-id="a2464-122">None</span></span>|<span data-ttu-id="a2464-123">删除[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="a2464-123">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="a2464-124">更新 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2464-124">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="a2464-125">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="a2464-125">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="a2464-126">更新[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2464-126">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="a2464-127">createInstance 操作</span><span class="sxs-lookup"><span data-stu-id="a2464-127">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="a2464-128">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="a2464-128">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="a2464-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a2464-129">Not yet documented</span></span>|
|[<span data-ttu-id="a2464-130">compare 函数</span><span class="sxs-lookup"><span data-stu-id="a2464-130">compare function</span></span>](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|<span data-ttu-id="a2464-131">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2464-131">[deviceManagementSettingComparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md) collection</span></span>|<span data-ttu-id="a2464-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a2464-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a2464-133">属性</span><span class="sxs-lookup"><span data-stu-id="a2464-133">Properties</span></span>
|<span data-ttu-id="a2464-134">属性</span><span class="sxs-lookup"><span data-stu-id="a2464-134">Property</span></span>|<span data-ttu-id="a2464-135">类型</span><span class="sxs-lookup"><span data-stu-id="a2464-135">Type</span></span>|<span data-ttu-id="a2464-136">说明</span><span class="sxs-lookup"><span data-stu-id="a2464-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2464-137">id</span><span class="sxs-lookup"><span data-stu-id="a2464-137">id</span></span>|<span data-ttu-id="a2464-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a2464-138">String</span></span>|<span data-ttu-id="a2464-139">模板 ID</span><span class="sxs-lookup"><span data-stu-id="a2464-139">The template ID</span></span>|
|<span data-ttu-id="a2464-140">displayName</span><span class="sxs-lookup"><span data-stu-id="a2464-140">displayName</span></span>|<span data-ttu-id="a2464-141">String</span><span class="sxs-lookup"><span data-stu-id="a2464-141">String</span></span>|<span data-ttu-id="a2464-142">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="a2464-142">The template's display name</span></span>|
|<span data-ttu-id="a2464-143">说明</span><span class="sxs-lookup"><span data-stu-id="a2464-143">description</span></span>|<span data-ttu-id="a2464-144">String</span><span class="sxs-lookup"><span data-stu-id="a2464-144">String</span></span>|<span data-ttu-id="a2464-145">模板的说明</span><span class="sxs-lookup"><span data-stu-id="a2464-145">The template's description</span></span>|
|<span data-ttu-id="a2464-146">versionInfo</span><span class="sxs-lookup"><span data-stu-id="a2464-146">versionInfo</span></span>|<span data-ttu-id="a2464-147">String</span><span class="sxs-lookup"><span data-stu-id="a2464-147">String</span></span>|<span data-ttu-id="a2464-148">模板的版本信息</span><span class="sxs-lookup"><span data-stu-id="a2464-148">The template's version information</span></span>|
|<span data-ttu-id="a2464-149">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="a2464-149">isDeprecated</span></span>|<span data-ttu-id="a2464-150">布尔</span><span class="sxs-lookup"><span data-stu-id="a2464-150">Boolean</span></span>|<span data-ttu-id="a2464-151">模板已弃用或不已弃用。</span><span class="sxs-lookup"><span data-stu-id="a2464-151">The template is deprecated or not.</span></span> <span data-ttu-id="a2464-152">无法从已弃用的模板创建意向。</span><span class="sxs-lookup"><span data-stu-id="a2464-152">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="a2464-153">intentCount</span><span class="sxs-lookup"><span data-stu-id="a2464-153">intentCount</span></span>|<span data-ttu-id="a2464-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a2464-154">Int32</span></span>|<span data-ttu-id="a2464-155">从此模板创建的意向数。</span><span class="sxs-lookup"><span data-stu-id="a2464-155">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="a2464-156">templateType</span><span class="sxs-lookup"><span data-stu-id="a2464-156">templateType</span></span>|[<span data-ttu-id="a2464-157">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="a2464-157">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="a2464-158">模板的类型。</span><span class="sxs-lookup"><span data-stu-id="a2464-158">The template's type.</span></span> <span data-ttu-id="a2464-159">可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`。</span><span class="sxs-lookup"><span data-stu-id="a2464-159">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="a2464-160">platformType</span><span class="sxs-lookup"><span data-stu-id="a2464-160">platformType</span></span>|[<span data-ttu-id="a2464-161">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a2464-161">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="a2464-162">模板的平台。</span><span class="sxs-lookup"><span data-stu-id="a2464-162">The template's platform.</span></span> <span data-ttu-id="a2464-163">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="a2464-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a2464-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2464-164">publishedDateTime</span></span>|<span data-ttu-id="a2464-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2464-165">DateTimeOffset</span></span>|<span data-ttu-id="a2464-166">发布模板时</span><span class="sxs-lookup"><span data-stu-id="a2464-166">When the template was published</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2464-167">关系</span><span class="sxs-lookup"><span data-stu-id="a2464-167">Relationships</span></span>
|<span data-ttu-id="a2464-168">关系</span><span class="sxs-lookup"><span data-stu-id="a2464-168">Relationship</span></span>|<span data-ttu-id="a2464-169">类型</span><span class="sxs-lookup"><span data-stu-id="a2464-169">Type</span></span>|<span data-ttu-id="a2464-170">说明</span><span class="sxs-lookup"><span data-stu-id="a2464-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2464-171">设置</span><span class="sxs-lookup"><span data-stu-id="a2464-171">settings</span></span>|<span data-ttu-id="a2464-172">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2464-172">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="a2464-173">此模板包含的所有设置的集合</span><span class="sxs-lookup"><span data-stu-id="a2464-173">Collection of all settings this template has</span></span>|
|<span data-ttu-id="a2464-174">categories</span><span class="sxs-lookup"><span data-stu-id="a2464-174">categories</span></span>|<span data-ttu-id="a2464-175">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2464-175">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="a2464-176">模板中设置类别的集合</span><span class="sxs-lookup"><span data-stu-id="a2464-176">Collection of setting categories within the template</span></span>|
|<span data-ttu-id="a2464-177">migratableTo</span><span class="sxs-lookup"><span data-stu-id="a2464-177">migratableTo</span></span>|<span data-ttu-id="a2464-178">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2464-178">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="a2464-179">此模板可以迁移到的模板集合</span><span class="sxs-lookup"><span data-stu-id="a2464-179">Collection of templates this template can migrate to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2464-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2464-180">JSON Representation</span></span>
<span data-ttu-id="a2464-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2464-181">Here is a JSON representation of the resource.</span></span>
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



