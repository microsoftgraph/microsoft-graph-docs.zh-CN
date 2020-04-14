---
title: deviceManagementSettingCategory 资源类型
description: 表示设置类别的实体
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe3e2d1877548232df5da92bdee85408d462e281
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443280"
---
# <a name="devicemanagementsettingcategory-resource-type"></a><span data-ttu-id="ad345-103">deviceManagementSettingCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad345-103">deviceManagementSettingCategory resource type</span></span>

<span data-ttu-id="ad345-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad345-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad345-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ad345-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad345-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad345-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad345-107">表示设置类别的实体</span><span class="sxs-lookup"><span data-stu-id="ad345-107">Entity representing a setting category</span></span>

## <a name="methods"></a><span data-ttu-id="ad345-108">方法</span><span class="sxs-lookup"><span data-stu-id="ad345-108">Methods</span></span>
|<span data-ttu-id="ad345-109">方法</span><span class="sxs-lookup"><span data-stu-id="ad345-109">Method</span></span>|<span data-ttu-id="ad345-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ad345-110">Return Type</span></span>|<span data-ttu-id="ad345-111">说明</span><span class="sxs-lookup"><span data-stu-id="ad345-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ad345-112">列出 deviceManagementSettingCategories</span><span class="sxs-lookup"><span data-stu-id="ad345-112">List deviceManagementSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|<span data-ttu-id="ad345-113">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="ad345-113">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) collection</span></span>|<span data-ttu-id="ad345-114">列出[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad345-114">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="ad345-115">获取 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ad345-115">Get deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[<span data-ttu-id="ad345-116">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ad345-116">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="ad345-117">读取[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad345-117">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="ad345-118">创建 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ad345-118">Create deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[<span data-ttu-id="ad345-119">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ad345-119">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="ad345-120">创建新的[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ad345-120">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="ad345-121">删除 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ad345-121">Delete deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|<span data-ttu-id="ad345-122">无</span><span class="sxs-lookup"><span data-stu-id="ad345-122">None</span></span>|<span data-ttu-id="ad345-123">删除[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="ad345-123">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>|
|[<span data-ttu-id="ad345-124">更新 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ad345-124">Update deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[<span data-ttu-id="ad345-125">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="ad345-125">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="ad345-126">更新[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad345-126">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad345-127">属性</span><span class="sxs-lookup"><span data-stu-id="ad345-127">Properties</span></span>
|<span data-ttu-id="ad345-128">属性</span><span class="sxs-lookup"><span data-stu-id="ad345-128">Property</span></span>|<span data-ttu-id="ad345-129">类型</span><span class="sxs-lookup"><span data-stu-id="ad345-129">Type</span></span>|<span data-ttu-id="ad345-130">说明</span><span class="sxs-lookup"><span data-stu-id="ad345-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad345-131">id</span><span class="sxs-lookup"><span data-stu-id="ad345-131">id</span></span>|<span data-ttu-id="ad345-132">String</span><span class="sxs-lookup"><span data-stu-id="ad345-132">String</span></span>|<span data-ttu-id="ad345-133">类别 ID</span><span class="sxs-lookup"><span data-stu-id="ad345-133">The category ID</span></span>|
|<span data-ttu-id="ad345-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ad345-134">displayName</span></span>|<span data-ttu-id="ad345-135">String</span><span class="sxs-lookup"><span data-stu-id="ad345-135">String</span></span>|<span data-ttu-id="ad345-136">类别名称</span><span class="sxs-lookup"><span data-stu-id="ad345-136">The category name</span></span>|
|<span data-ttu-id="ad345-137">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="ad345-137">hasRequiredSetting</span></span>|<span data-ttu-id="ad345-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad345-138">Boolean</span></span>|<span data-ttu-id="ad345-139">类别包含 "必需顶级" 设置</span><span class="sxs-lookup"><span data-stu-id="ad345-139">The category contains top level required setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad345-140">关系</span><span class="sxs-lookup"><span data-stu-id="ad345-140">Relationships</span></span>
|<span data-ttu-id="ad345-141">关系</span><span class="sxs-lookup"><span data-stu-id="ad345-141">Relationship</span></span>|<span data-ttu-id="ad345-142">类型</span><span class="sxs-lookup"><span data-stu-id="ad345-142">Type</span></span>|<span data-ttu-id="ad345-143">说明</span><span class="sxs-lookup"><span data-stu-id="ad345-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad345-144">settingDefinitions</span><span class="sxs-lookup"><span data-stu-id="ad345-144">settingDefinitions</span></span>|<span data-ttu-id="ad345-145">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="ad345-145">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="ad345-146">此类别包含的设置定义</span><span class="sxs-lookup"><span data-stu-id="ad345-146">The setting definitions this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad345-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad345-147">JSON Representation</span></span>
<span data-ttu-id="ad345-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad345-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```



