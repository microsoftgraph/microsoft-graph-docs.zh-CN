---
title: securityBaselineTemplate 资源类型
description: 帐户的安全基准模板
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4287b83281299110fefad3ee2e2c6bd0e861e4da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778164"
---
# <a name="securitybaselinetemplate-resource-type"></a><span data-ttu-id="6f710-103">securityBaselineTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f710-103">securityBaselineTemplate resource type</span></span>

> <span data-ttu-id="6f710-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f710-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f710-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f710-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f710-106">帐户的安全基准模板</span><span class="sxs-lookup"><span data-stu-id="6f710-106">The security baseline template of the account</span></span>


<span data-ttu-id="6f710-107">继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="6f710-107">Inherits from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6f710-108">方法</span><span class="sxs-lookup"><span data-stu-id="6f710-108">Methods</span></span>
|<span data-ttu-id="6f710-109">方法</span><span class="sxs-lookup"><span data-stu-id="6f710-109">Method</span></span>|<span data-ttu-id="6f710-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6f710-110">Return Type</span></span>|<span data-ttu-id="6f710-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f710-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6f710-112">列出 securityBaselineTemplates</span><span class="sxs-lookup"><span data-stu-id="6f710-112">List securityBaselineTemplates</span></span>](../api/intune-deviceintent-securitybaselinetemplate-list.md)|<span data-ttu-id="6f710-113">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="6f710-113">[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) collection</span></span>|<span data-ttu-id="6f710-114">列出[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f710-114">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>|
|[<span data-ttu-id="6f710-115">获取 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="6f710-115">Get securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[<span data-ttu-id="6f710-116">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="6f710-116">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="6f710-117">读取[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f710-117">Read properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|
|[<span data-ttu-id="6f710-118">创建 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="6f710-118">Create securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[<span data-ttu-id="6f710-119">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="6f710-119">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="6f710-120">创建新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6f710-120">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|
|[<span data-ttu-id="6f710-121">删除 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="6f710-121">Delete securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|<span data-ttu-id="6f710-122">无</span><span class="sxs-lookup"><span data-stu-id="6f710-122">None</span></span>|<span data-ttu-id="6f710-123">删除[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="6f710-123">Deletes a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>|
|[<span data-ttu-id="6f710-124">更新 securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="6f710-124">Update securityBaselineTemplate</span></span>](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[<span data-ttu-id="6f710-125">securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="6f710-125">securityBaselineTemplate</span></span>](../resources/intune-deviceintent-securitybaselinetemplate.md)|<span data-ttu-id="6f710-126">更新[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6f710-126">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6f710-127">属性</span><span class="sxs-lookup"><span data-stu-id="6f710-127">Properties</span></span>
|<span data-ttu-id="6f710-128">属性</span><span class="sxs-lookup"><span data-stu-id="6f710-128">Property</span></span>|<span data-ttu-id="6f710-129">类型</span><span class="sxs-lookup"><span data-stu-id="6f710-129">Type</span></span>|<span data-ttu-id="6f710-130">说明</span><span class="sxs-lookup"><span data-stu-id="6f710-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f710-131">id</span><span class="sxs-lookup"><span data-stu-id="6f710-131">id</span></span>|<span data-ttu-id="6f710-132">String</span><span class="sxs-lookup"><span data-stu-id="6f710-132">String</span></span>|<span data-ttu-id="6f710-133">从[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID</span><span class="sxs-lookup"><span data-stu-id="6f710-133">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="6f710-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6f710-134">displayName</span></span>|<span data-ttu-id="6f710-135">String</span><span class="sxs-lookup"><span data-stu-id="6f710-135">String</span></span>|<span data-ttu-id="6f710-136">从[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="6f710-136">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="6f710-137">description</span><span class="sxs-lookup"><span data-stu-id="6f710-137">description</span></span>|<span data-ttu-id="6f710-138">String</span><span class="sxs-lookup"><span data-stu-id="6f710-138">String</span></span>|<span data-ttu-id="6f710-139">模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="6f710-139">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f710-140">关系</span><span class="sxs-lookup"><span data-stu-id="6f710-140">Relationships</span></span>
|<span data-ttu-id="6f710-141">关系</span><span class="sxs-lookup"><span data-stu-id="6f710-141">Relationship</span></span>|<span data-ttu-id="6f710-142">类型</span><span class="sxs-lookup"><span data-stu-id="6f710-142">Type</span></span>|<span data-ttu-id="6f710-143">说明</span><span class="sxs-lookup"><span data-stu-id="6f710-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f710-144">settings</span><span class="sxs-lookup"><span data-stu-id="6f710-144">settings</span></span>|<span data-ttu-id="6f710-145">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="6f710-145">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="6f710-146">此模板继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)的所有设置的集合</span><span class="sxs-lookup"><span data-stu-id="6f710-146">Collection of all settings this template has Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="6f710-147">类别</span><span class="sxs-lookup"><span data-stu-id="6f710-147">categories</span></span>|<span data-ttu-id="6f710-148">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="6f710-148">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="6f710-149">从[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板中的设置类别的集合</span><span class="sxs-lookup"><span data-stu-id="6f710-149">Collection of setting categories within the template Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="6f710-150">deviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="6f710-150">deviceStateSummary</span></span>|[<span data-ttu-id="6f710-151">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="6f710-151">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="6f710-152">安全基准设备状态摘要</span><span class="sxs-lookup"><span data-stu-id="6f710-152">The security baseline device state summary</span></span>|
|<span data-ttu-id="6f710-153">deviceStates</span><span class="sxs-lookup"><span data-stu-id="6f710-153">deviceStates</span></span>|<span data-ttu-id="6f710-154">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="6f710-154">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="6f710-155">安全基准设备状态</span><span class="sxs-lookup"><span data-stu-id="6f710-155">The security baseline device states</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f710-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f710-156">JSON Representation</span></span>
<span data-ttu-id="6f710-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f710-157">Here is a JSON representation of the resource.</span></span>
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





