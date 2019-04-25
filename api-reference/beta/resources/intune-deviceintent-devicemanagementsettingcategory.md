---
title: deviceManagementSettingCategory 资源类型
description: 表示设置类别的实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6af038e31135a99e473f6b14638655af073e1602
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550567"
---
# <a name="devicemanagementsettingcategory-resource-type"></a><span data-ttu-id="34682-103">deviceManagementSettingCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="34682-103">deviceManagementSettingCategory resource type</span></span>

> <span data-ttu-id="34682-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34682-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34682-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34682-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34682-106">表示设置类别的实体</span><span class="sxs-lookup"><span data-stu-id="34682-106">Entity representing a setting category</span></span>

## <a name="methods"></a><span data-ttu-id="34682-107">方法</span><span class="sxs-lookup"><span data-stu-id="34682-107">Methods</span></span>
|<span data-ttu-id="34682-108">方法</span><span class="sxs-lookup"><span data-stu-id="34682-108">Method</span></span>|<span data-ttu-id="34682-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="34682-109">Return Type</span></span>|<span data-ttu-id="34682-110">说明</span><span class="sxs-lookup"><span data-stu-id="34682-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34682-111">列出 deviceManagementSettingCategories</span><span class="sxs-lookup"><span data-stu-id="34682-111">List deviceManagementSettingCategories</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|<span data-ttu-id="34682-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="34682-112">[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) collection</span></span>|<span data-ttu-id="34682-113">列出[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34682-113">List properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) objects.</span></span>|
|[<span data-ttu-id="34682-114">获取 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="34682-114">Get deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[<span data-ttu-id="34682-115">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="34682-115">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="34682-116">读取[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34682-116">Read properties and relationships of the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="34682-117">创建 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="34682-117">Create deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[<span data-ttu-id="34682-118">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="34682-118">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="34682-119">创建新的[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34682-119">Create a new [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|
|[<span data-ttu-id="34682-120">删除 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="34682-120">Delete deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|<span data-ttu-id="34682-121">无</span><span class="sxs-lookup"><span data-stu-id="34682-121">None</span></span>|<span data-ttu-id="34682-122">删除[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="34682-122">Deletes a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>|
|[<span data-ttu-id="34682-123">更新 deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="34682-123">Update deviceManagementSettingCategory</span></span>](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[<span data-ttu-id="34682-124">deviceManagementSettingCategory</span><span class="sxs-lookup"><span data-stu-id="34682-124">deviceManagementSettingCategory</span></span>](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|<span data-ttu-id="34682-125">更新[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="34682-125">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34682-126">属性</span><span class="sxs-lookup"><span data-stu-id="34682-126">Properties</span></span>
|<span data-ttu-id="34682-127">属性</span><span class="sxs-lookup"><span data-stu-id="34682-127">Property</span></span>|<span data-ttu-id="34682-128">类型</span><span class="sxs-lookup"><span data-stu-id="34682-128">Type</span></span>|<span data-ttu-id="34682-129">说明</span><span class="sxs-lookup"><span data-stu-id="34682-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34682-130">id</span><span class="sxs-lookup"><span data-stu-id="34682-130">id</span></span>|<span data-ttu-id="34682-131">String</span><span class="sxs-lookup"><span data-stu-id="34682-131">String</span></span>|<span data-ttu-id="34682-132">类别 ID</span><span class="sxs-lookup"><span data-stu-id="34682-132">The category ID</span></span>|
|<span data-ttu-id="34682-133">displayName</span><span class="sxs-lookup"><span data-stu-id="34682-133">displayName</span></span>|<span data-ttu-id="34682-134">String</span><span class="sxs-lookup"><span data-stu-id="34682-134">String</span></span>|<span data-ttu-id="34682-135">类别名称</span><span class="sxs-lookup"><span data-stu-id="34682-135">The category name</span></span>|

## <a name="relationships"></a><span data-ttu-id="34682-136">关系</span><span class="sxs-lookup"><span data-stu-id="34682-136">Relationships</span></span>
|<span data-ttu-id="34682-137">关系</span><span class="sxs-lookup"><span data-stu-id="34682-137">Relationship</span></span>|<span data-ttu-id="34682-138">类型</span><span class="sxs-lookup"><span data-stu-id="34682-138">Type</span></span>|<span data-ttu-id="34682-139">说明</span><span class="sxs-lookup"><span data-stu-id="34682-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34682-140">settingDefinitions</span><span class="sxs-lookup"><span data-stu-id="34682-140">settingDefinitions</span></span>|<span data-ttu-id="34682-141">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="34682-141">[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) collection</span></span>|<span data-ttu-id="34682-142">此类别包含的设置定义</span><span class="sxs-lookup"><span data-stu-id="34682-142">The setting definitions this category contains</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34682-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34682-143">JSON Representation</span></span>
<span data-ttu-id="34682-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34682-144">Here is a JSON representation of the resource.</span></span>
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





