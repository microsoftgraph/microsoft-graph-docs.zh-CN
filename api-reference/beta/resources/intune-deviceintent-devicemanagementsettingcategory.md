---
title: deviceManagementSettingCategory 资源类型
description: 表示设置类别的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c87774cf0aa8a5e3a4cb65b10566323b2c7749
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943386"
---
# <a name="devicemanagementsettingcategory-resource-type"></a><span data-ttu-id="27e2b-103">deviceManagementSettingCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="27e2b-103">deviceManagementSettingCategory resource type</span></span>

> <span data-ttu-id="27e2b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27e2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27e2b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27e2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27e2b-106">表示设置类别的实体</span><span class="sxs-lookup"><span data-stu-id="27e2b-106">Entity representing a setting category</span></span>

## <a name="methods"></a><span data-ttu-id="27e2b-107">方法</span><span class="sxs-lookup"><span data-stu-id="27e2b-107">Methods</span></span>
|<span data-ttu-id="27e2b-108">方法</span><span class="sxs-lookup"><span data-stu-id="27e2b-108">Method</span></span>|<span data-ttu-id="27e2b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="27e2b-109">Return Type</span></span>|<span data-ttu-id="27e2b-110">说明</span><span class="sxs-lookup"><span data-stu-id="27e2b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27e2b-111">列出 deviceManagementSettingCategories</span><span class="sxs-lookup"><span data-stu-id="27e2b-111">List deviceManagementSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|<span data-ttu-id="27e2b-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="27e2b-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) collection</span></span>|<span data-ttu-id="27e2b-113">列出[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27e2b-113">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="27e2b-114">获取 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="27e2b-114">Get deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[<span data-ttu-id="27e2b-115">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="27e2b-115">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="27e2b-116">读取[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27e2b-116">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="27e2b-117">创建 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="27e2b-117">Create deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[<span data-ttu-id="27e2b-118">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="27e2b-118">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="27e2b-119">创建新的[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27e2b-119">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="27e2b-120">删除 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="27e2b-120">Delete deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|<span data-ttu-id="27e2b-121">无</span><span class="sxs-lookup"><span data-stu-id="27e2b-121">None</span></span>|<span data-ttu-id="27e2b-122">删除[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="27e2b-122">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>|
|[<span data-ttu-id="27e2b-123">更新 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="27e2b-123">Update deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[<span data-ttu-id="27e2b-124">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="27e2b-124">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="27e2b-125">更新[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27e2b-125">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27e2b-126">属性</span><span class="sxs-lookup"><span data-stu-id="27e2b-126">Properties</span></span>
|<span data-ttu-id="27e2b-127">属性</span><span class="sxs-lookup"><span data-stu-id="27e2b-127">Property</span></span>|<span data-ttu-id="27e2b-128">类型</span><span class="sxs-lookup"><span data-stu-id="27e2b-128">Type</span></span>|<span data-ttu-id="27e2b-129">说明</span><span class="sxs-lookup"><span data-stu-id="27e2b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27e2b-130">id</span><span class="sxs-lookup"><span data-stu-id="27e2b-130">id</span></span>|<span data-ttu-id="27e2b-131">String</span><span class="sxs-lookup"><span data-stu-id="27e2b-131">String</span></span>|<span data-ttu-id="27e2b-132">类别 ID</span><span class="sxs-lookup"><span data-stu-id="27e2b-132">The category ID</span></span>|
|<span data-ttu-id="27e2b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="27e2b-133">displayName</span></span>|<span data-ttu-id="27e2b-134">String</span><span class="sxs-lookup"><span data-stu-id="27e2b-134">String</span></span>|<span data-ttu-id="27e2b-135">类别名称</span><span class="sxs-lookup"><span data-stu-id="27e2b-135">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="27e2b-136">关系</span><span class="sxs-lookup"><span data-stu-id="27e2b-136">Relationships</span></span>
|<span data-ttu-id="27e2b-137">关系</span><span class="sxs-lookup"><span data-stu-id="27e2b-137">Relationship</span></span>|<span data-ttu-id="27e2b-138">类型</span><span class="sxs-lookup"><span data-stu-id="27e2b-138">Type</span></span>|<span data-ttu-id="27e2b-139">说明</span><span class="sxs-lookup"><span data-stu-id="27e2b-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27e2b-140">settingDefinitions</span><span class="sxs-lookup"><span data-stu-id="27e2b-140">settingDefinitions</span></span>|<span data-ttu-id="27e2b-141">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="27e2b-141">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="27e2b-142">此类别包含的设置定义</span><span class="sxs-lookup"><span data-stu-id="27e2b-142">The setting definitions this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27e2b-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27e2b-143">JSON Representation</span></span>
<span data-ttu-id="27e2b-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27e2b-144">Here is a JSON representation of the resource.</span></span>
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
  "displayName": "String"
}
```




