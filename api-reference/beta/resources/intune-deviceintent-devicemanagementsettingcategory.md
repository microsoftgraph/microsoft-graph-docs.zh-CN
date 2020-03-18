---
title: deviceManagementSettingCategory 资源类型
description: 表示设置类别的实体
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d32812cd3ae60f9113fb3fba842024cd291a0eb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785363"
---
# <a name="devicemanagementsettingcategory-resource-type"></a><span data-ttu-id="c696c-103">deviceManagementSettingCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="c696c-103">deviceManagementSettingCategory resource type</span></span>

> <span data-ttu-id="c696c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c696c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c696c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c696c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c696c-106">表示设置类别的实体</span><span class="sxs-lookup"><span data-stu-id="c696c-106">Entity representing a setting category</span></span>

## <a name="methods"></a><span data-ttu-id="c696c-107">方法</span><span class="sxs-lookup"><span data-stu-id="c696c-107">Methods</span></span>
|<span data-ttu-id="c696c-108">方法</span><span class="sxs-lookup"><span data-stu-id="c696c-108">Method</span></span>|<span data-ttu-id="c696c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c696c-109">Return Type</span></span>|<span data-ttu-id="c696c-110">说明</span><span class="sxs-lookup"><span data-stu-id="c696c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c696c-111">列出 deviceManagementSettingCategories</span><span class="sxs-lookup"><span data-stu-id="c696c-111">List deviceManagementSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|<span data-ttu-id="c696c-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="c696c-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) collection</span></span>|<span data-ttu-id="c696c-113">列出[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c696c-113">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="c696c-114">获取 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c696c-114">Get deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[<span data-ttu-id="c696c-115">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c696c-115">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="c696c-116">读取[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c696c-116">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="c696c-117">创建 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c696c-117">Create deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[<span data-ttu-id="c696c-118">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c696c-118">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="c696c-119">创建新的[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c696c-119">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="c696c-120">删除 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c696c-120">Delete deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|<span data-ttu-id="c696c-121">None</span><span class="sxs-lookup"><span data-stu-id="c696c-121">None</span></span>|<span data-ttu-id="c696c-122">删除[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="c696c-122">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>|
|[<span data-ttu-id="c696c-123">更新 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c696c-123">Update deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[<span data-ttu-id="c696c-124">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="c696c-124">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="c696c-125">更新[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c696c-125">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c696c-126">属性</span><span class="sxs-lookup"><span data-stu-id="c696c-126">Properties</span></span>
|<span data-ttu-id="c696c-127">属性</span><span class="sxs-lookup"><span data-stu-id="c696c-127">Property</span></span>|<span data-ttu-id="c696c-128">类型</span><span class="sxs-lookup"><span data-stu-id="c696c-128">Type</span></span>|<span data-ttu-id="c696c-129">说明</span><span class="sxs-lookup"><span data-stu-id="c696c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c696c-130">id</span><span class="sxs-lookup"><span data-stu-id="c696c-130">id</span></span>|<span data-ttu-id="c696c-131">String</span><span class="sxs-lookup"><span data-stu-id="c696c-131">String</span></span>|<span data-ttu-id="c696c-132">类别 ID</span><span class="sxs-lookup"><span data-stu-id="c696c-132">The category ID</span></span>|
|<span data-ttu-id="c696c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c696c-133">displayName</span></span>|<span data-ttu-id="c696c-134">String</span><span class="sxs-lookup"><span data-stu-id="c696c-134">String</span></span>|<span data-ttu-id="c696c-135">类别名称</span><span class="sxs-lookup"><span data-stu-id="c696c-135">The category name</span></span>|
|<span data-ttu-id="c696c-136">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="c696c-136">hasRequiredSetting</span></span>|<span data-ttu-id="c696c-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="c696c-137">Boolean</span></span>|<span data-ttu-id="c696c-138">类别包含 "必需顶级" 设置</span><span class="sxs-lookup"><span data-stu-id="c696c-138">The category contains top level required setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="c696c-139">关系</span><span class="sxs-lookup"><span data-stu-id="c696c-139">Relationships</span></span>
|<span data-ttu-id="c696c-140">关系</span><span class="sxs-lookup"><span data-stu-id="c696c-140">Relationship</span></span>|<span data-ttu-id="c696c-141">类型</span><span class="sxs-lookup"><span data-stu-id="c696c-141">Type</span></span>|<span data-ttu-id="c696c-142">说明</span><span class="sxs-lookup"><span data-stu-id="c696c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c696c-143">settingDefinitions</span><span class="sxs-lookup"><span data-stu-id="c696c-143">settingDefinitions</span></span>|<span data-ttu-id="c696c-144">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="c696c-144">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="c696c-145">此类别包含的设置定义</span><span class="sxs-lookup"><span data-stu-id="c696c-145">The setting definitions this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c696c-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c696c-146">JSON Representation</span></span>
<span data-ttu-id="c696c-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c696c-147">Here is a JSON representation of the resource.</span></span>
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



