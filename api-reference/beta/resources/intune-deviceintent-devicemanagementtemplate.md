---
title: deviceManagementTemplate 资源类型
description: 表示已定义的设备设置集合的实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cf144ed30a017dc1f3ae84fc481568adc0d0d09
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522515"
---
# <a name="devicemanagementtemplate-resource-type"></a><span data-ttu-id="8d564-103">deviceManagementTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d564-103">deviceManagementTemplate resource type</span></span>

> <span data-ttu-id="8d564-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d564-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d564-106">表示已定义的设备设置集合的实体</span><span class="sxs-lookup"><span data-stu-id="8d564-106">Entity that represents a defined collection of device settings</span></span>

## <a name="methods"></a><span data-ttu-id="8d564-107">方法</span><span class="sxs-lookup"><span data-stu-id="8d564-107">Methods</span></span>
|<span data-ttu-id="8d564-108">方法</span><span class="sxs-lookup"><span data-stu-id="8d564-108">Method</span></span>|<span data-ttu-id="8d564-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d564-109">Return Type</span></span>|<span data-ttu-id="8d564-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d564-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8d564-111">列出 deviceManagementTemplates</span><span class="sxs-lookup"><span data-stu-id="8d564-111">List deviceManagementTemplates</span></span>](../api/intune-deviceintent-devicemanagementtemplate-list.md)|<span data-ttu-id="8d564-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d564-112">[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) collection</span></span>|<span data-ttu-id="8d564-113">列出[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d564-113">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>|
|[<span data-ttu-id="8d564-114">获取 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8d564-114">Get deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[<span data-ttu-id="8d564-115">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8d564-115">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="8d564-116">读取[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d564-116">Read properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="8d564-117">创建 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8d564-117">Create deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[<span data-ttu-id="8d564-118">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8d564-118">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="8d564-119">创建新的[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8d564-119">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="8d564-120">删除 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8d564-120">Delete deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|<span data-ttu-id="8d564-121">无</span><span class="sxs-lookup"><span data-stu-id="8d564-121">None</span></span>|<span data-ttu-id="8d564-122">删除[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="8d564-122">Deletes a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>|
|[<span data-ttu-id="8d564-123">更新 deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8d564-123">Update deviceManagementTemplate</span></span>](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[<span data-ttu-id="8d564-124">deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="8d564-124">deviceManagementTemplate</span></span>](../resources/intune-deviceintent-devicemanagementtemplate.md)|<span data-ttu-id="8d564-125">更新[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8d564-125">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>|
|[<span data-ttu-id="8d564-126">createInstance 操作</span><span class="sxs-lookup"><span data-stu-id="8d564-126">createInstance action</span></span>](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[<span data-ttu-id="8d564-127">deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="8d564-127">deviceManagementIntent</span></span>](../resources/intune-deviceintent-devicemanagementintent.md)|<span data-ttu-id="8d564-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d564-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8d564-129">属性</span><span class="sxs-lookup"><span data-stu-id="8d564-129">Properties</span></span>
|<span data-ttu-id="8d564-130">属性</span><span class="sxs-lookup"><span data-stu-id="8d564-130">Property</span></span>|<span data-ttu-id="8d564-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d564-131">Type</span></span>|<span data-ttu-id="8d564-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d564-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d564-133">id</span><span class="sxs-lookup"><span data-stu-id="8d564-133">id</span></span>|<span data-ttu-id="8d564-134">String</span><span class="sxs-lookup"><span data-stu-id="8d564-134">String</span></span>|<span data-ttu-id="8d564-135">模板 ID</span><span class="sxs-lookup"><span data-stu-id="8d564-135">The template ID</span></span>|
|<span data-ttu-id="8d564-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8d564-136">displayName</span></span>|<span data-ttu-id="8d564-137">String</span><span class="sxs-lookup"><span data-stu-id="8d564-137">String</span></span>|<span data-ttu-id="8d564-138">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="8d564-138">The template's display name</span></span>|
|<span data-ttu-id="8d564-139">description</span><span class="sxs-lookup"><span data-stu-id="8d564-139">description</span></span>|<span data-ttu-id="8d564-140">String</span><span class="sxs-lookup"><span data-stu-id="8d564-140">String</span></span>|<span data-ttu-id="8d564-141">模板的说明</span><span class="sxs-lookup"><span data-stu-id="8d564-141">The template's description</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d564-142">关系</span><span class="sxs-lookup"><span data-stu-id="8d564-142">Relationships</span></span>
|<span data-ttu-id="8d564-143">关系</span><span class="sxs-lookup"><span data-stu-id="8d564-143">Relationship</span></span>|<span data-ttu-id="8d564-144">类型</span><span class="sxs-lookup"><span data-stu-id="8d564-144">Type</span></span>|<span data-ttu-id="8d564-145">说明</span><span class="sxs-lookup"><span data-stu-id="8d564-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d564-146">settings</span><span class="sxs-lookup"><span data-stu-id="8d564-146">settings</span></span>|<span data-ttu-id="8d564-147">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d564-147">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="8d564-148">此模板包含的所有设置的集合</span><span class="sxs-lookup"><span data-stu-id="8d564-148">Collection of all settings this template has</span></span>|
|<span data-ttu-id="8d564-149">类别</span><span class="sxs-lookup"><span data-stu-id="8d564-149">categories</span></span>|<span data-ttu-id="8d564-150">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d564-150">[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) collection</span></span>|<span data-ttu-id="8d564-151">模板中设置类别的集合</span><span class="sxs-lookup"><span data-stu-id="8d564-151">Collection of setting categories within the template</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d564-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d564-152">JSON Representation</span></span>
<span data-ttu-id="8d564-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d564-153">Here is a JSON representation of the resource.</span></span>
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
  "description": "String"
}
```







