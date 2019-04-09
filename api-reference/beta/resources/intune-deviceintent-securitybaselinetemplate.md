---
title: securityBaselineTemplate 资源类型
description: 帐户的安全基准模板
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b572d3cc25943438f190a46fd23704a2eb6b7be3
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522340"
---
# <a name="securitybaselinetemplate-resource-type"></a><span data-ttu-id="84a2c-103">securityBaselineTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="84a2c-103">securityBaselineTemplate resource type</span></span>

> <span data-ttu-id="84a2c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84a2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84a2c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84a2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84a2c-106">帐户的安全基准模板</span><span class="sxs-lookup"><span data-stu-id="84a2c-106">The security baseline template of the account</span></span>


<span data-ttu-id="84a2c-107">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="84a2c-107">Inherits from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>

## <a name="methods"></a><span data-ttu-id="84a2c-108">方法</span><span class="sxs-lookup"><span data-stu-id="84a2c-108">Methods</span></span>
|<span data-ttu-id="84a2c-109">方法</span><span class="sxs-lookup"><span data-stu-id="84a2c-109">Method</span></span>|<span data-ttu-id="84a2c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="84a2c-110">Return Type</span></span>|<span data-ttu-id="84a2c-111">说明</span><span class="sxs-lookup"><span data-stu-id="84a2c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84a2c-112">列出 securityBaselineTemplates</span><span class="sxs-lookup"><span data-stu-id="84a2c-112">List securityBaselineTemplates</span></span>](../api/intune-deviceintent-securitybaselinetemplate-list.md)|<span data-ttu-id="84a2c-113">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="84a2c-113">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) collection</span></span>|<span data-ttu-id="84a2c-114">列出[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84a2c-114">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>|
|[<span data-ttu-id="84a2c-115">获取 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="84a2c-115">Get securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[<span data-ttu-id="84a2c-116">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="84a2c-116">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="84a2c-117">读取[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84a2c-117">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|
|[<span data-ttu-id="84a2c-118">创建 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="84a2c-118">Create securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[<span data-ttu-id="84a2c-119">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="84a2c-119">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="84a2c-120">创建新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84a2c-120">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|
|[<span data-ttu-id="84a2c-121">删除 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="84a2c-121">Delete securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|<span data-ttu-id="84a2c-122">无</span><span class="sxs-lookup"><span data-stu-id="84a2c-122">None</span></span>|<span data-ttu-id="84a2c-123">删除[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="84a2c-123">Deletes a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>|
|[<span data-ttu-id="84a2c-124">更新 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="84a2c-124">Update securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[<span data-ttu-id="84a2c-125">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="84a2c-125">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="84a2c-126">更新[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84a2c-126">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84a2c-127">属性</span><span class="sxs-lookup"><span data-stu-id="84a2c-127">Properties</span></span>
|<span data-ttu-id="84a2c-128">属性</span><span class="sxs-lookup"><span data-stu-id="84a2c-128">Property</span></span>|<span data-ttu-id="84a2c-129">类型</span><span class="sxs-lookup"><span data-stu-id="84a2c-129">Type</span></span>|<span data-ttu-id="84a2c-130">说明</span><span class="sxs-lookup"><span data-stu-id="84a2c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a2c-131">id</span><span class="sxs-lookup"><span data-stu-id="84a2c-131">id</span></span>|<span data-ttu-id="84a2c-132">String</span><span class="sxs-lookup"><span data-stu-id="84a2c-132">String</span></span>|<span data-ttu-id="84a2c-133">从[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID</span><span class="sxs-lookup"><span data-stu-id="84a2c-133">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="84a2c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="84a2c-134">displayName</span></span>|<span data-ttu-id="84a2c-135">String</span><span class="sxs-lookup"><span data-stu-id="84a2c-135">String</span></span>|<span data-ttu-id="84a2c-136">从[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="84a2c-136">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="84a2c-137">description</span><span class="sxs-lookup"><span data-stu-id="84a2c-137">description</span></span>|<span data-ttu-id="84a2c-138">String</span><span class="sxs-lookup"><span data-stu-id="84a2c-138">String</span></span>|<span data-ttu-id="84a2c-139">模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="84a2c-139">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="84a2c-140">关系</span><span class="sxs-lookup"><span data-stu-id="84a2c-140">Relationships</span></span>
|<span data-ttu-id="84a2c-141">关系</span><span class="sxs-lookup"><span data-stu-id="84a2c-141">Relationship</span></span>|<span data-ttu-id="84a2c-142">类型</span><span class="sxs-lookup"><span data-stu-id="84a2c-142">Type</span></span>|<span data-ttu-id="84a2c-143">说明</span><span class="sxs-lookup"><span data-stu-id="84a2c-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a2c-144">settings</span><span class="sxs-lookup"><span data-stu-id="84a2c-144">settings</span></span>|<span data-ttu-id="84a2c-145">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="84a2c-145">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="84a2c-146">此模板继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)的所有设置的集合</span><span class="sxs-lookup"><span data-stu-id="84a2c-146">Collection of all settings this template has Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="84a2c-147">类别</span><span class="sxs-lookup"><span data-stu-id="84a2c-147">categories</span></span>|<span data-ttu-id="84a2c-148">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="84a2c-148">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="84a2c-149">从[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板中的设置类别的集合</span><span class="sxs-lookup"><span data-stu-id="84a2c-149">Collection of setting categories within the template Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="84a2c-150">deviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="84a2c-150">deviceStateSummary</span></span>|[<span data-ttu-id="84a2c-151">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="84a2c-151">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="84a2c-152">安全基准设备状态摘要</span><span class="sxs-lookup"><span data-stu-id="84a2c-152">The security baseline device state summary</span></span>|
|<span data-ttu-id="84a2c-153">deviceStates</span><span class="sxs-lookup"><span data-stu-id="84a2c-153">deviceStates</span></span>|<span data-ttu-id="84a2c-154">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="84a2c-154">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="84a2c-155">安全基准设备状态</span><span class="sxs-lookup"><span data-stu-id="84a2c-155">The security baseline device states</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84a2c-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84a2c-156">JSON Representation</span></span>
<span data-ttu-id="84a2c-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84a2c-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```







