---
title: deviceManagementConfigurationCategory 资源类型
description: 设备管理配置策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14610b5bc87a1da11492decb122ee85b065b0c10
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665082"
---
# <a name="devicemanagementconfigurationcategory-resource-type"></a><span data-ttu-id="da5f9-103">deviceManagementConfigurationCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="da5f9-103">deviceManagementConfigurationCategory resource type</span></span>

<span data-ttu-id="da5f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da5f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da5f9-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da5f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da5f9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da5f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da5f9-107">设备管理配置策略</span><span class="sxs-lookup"><span data-stu-id="da5f9-107">Device Management Configuration Policy</span></span>

## <a name="methods"></a><span data-ttu-id="da5f9-108">方法</span><span class="sxs-lookup"><span data-stu-id="da5f9-108">Methods</span></span>
|<span data-ttu-id="da5f9-109">方法</span><span class="sxs-lookup"><span data-stu-id="da5f9-109">Method</span></span>|<span data-ttu-id="da5f9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="da5f9-110">Return Type</span></span>|<span data-ttu-id="da5f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="da5f9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da5f9-112">列出 deviceManagementConfigurationCategories</span><span class="sxs-lookup"><span data-stu-id="da5f9-112">List deviceManagementConfigurationCategories</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-list.md)|<span data-ttu-id="da5f9-113">[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="da5f9-113">[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) collection</span></span>|<span data-ttu-id="da5f9-114">列出 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da5f9-114">List properties and relationships of the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) objects.</span></span>|
|[<span data-ttu-id="da5f9-115">获取 deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="da5f9-115">Get deviceManagementConfigurationCategory</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-get.md)|[<span data-ttu-id="da5f9-116">deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="da5f9-116">deviceManagementConfigurationCategory</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|<span data-ttu-id="da5f9-117">读取 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da5f9-117">Read properties and relationships of the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>|
|[<span data-ttu-id="da5f9-118">创建 deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="da5f9-118">Create deviceManagementConfigurationCategory</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-create.md)|[<span data-ttu-id="da5f9-119">deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="da5f9-119">deviceManagementConfigurationCategory</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|<span data-ttu-id="da5f9-120">创建新的 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da5f9-120">Create a new [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>|
|[<span data-ttu-id="da5f9-121">删除 deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="da5f9-121">Delete deviceManagementConfigurationCategory</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-delete.md)|<span data-ttu-id="da5f9-122">无</span><span class="sxs-lookup"><span data-stu-id="da5f9-122">None</span></span>|<span data-ttu-id="da5f9-123">删除 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="da5f9-123">Deletes a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span></span>|
|[<span data-ttu-id="da5f9-124">更新 deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="da5f9-124">Update deviceManagementConfigurationCategory</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-update.md)|[<span data-ttu-id="da5f9-125">deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="da5f9-125">deviceManagementConfigurationCategory</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|<span data-ttu-id="da5f9-126">更新 [deviceManagementConfigurationCategory 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="da5f9-126">Update the properties of a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da5f9-127">属性</span><span class="sxs-lookup"><span data-stu-id="da5f9-127">Properties</span></span>
|<span data-ttu-id="da5f9-128">属性</span><span class="sxs-lookup"><span data-stu-id="da5f9-128">Property</span></span>|<span data-ttu-id="da5f9-129">类型</span><span class="sxs-lookup"><span data-stu-id="da5f9-129">Type</span></span>|<span data-ttu-id="da5f9-130">说明</span><span class="sxs-lookup"><span data-stu-id="da5f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da5f9-131">id</span><span class="sxs-lookup"><span data-stu-id="da5f9-131">id</span></span>|<span data-ttu-id="da5f9-132">String</span><span class="sxs-lookup"><span data-stu-id="da5f9-132">String</span></span>|<span data-ttu-id="da5f9-133">项的标识符</span><span class="sxs-lookup"><span data-stu-id="da5f9-133">Identifier for item</span></span>|
|<span data-ttu-id="da5f9-134">说明</span><span class="sxs-lookup"><span data-stu-id="da5f9-134">description</span></span>|<span data-ttu-id="da5f9-135">String</span><span class="sxs-lookup"><span data-stu-id="da5f9-135">String</span></span>|<span data-ttu-id="da5f9-136">项目说明</span><span class="sxs-lookup"><span data-stu-id="da5f9-136">Description of the item</span></span>|
|<span data-ttu-id="da5f9-137">helpText</span><span class="sxs-lookup"><span data-stu-id="da5f9-137">helpText</span></span>|<span data-ttu-id="da5f9-138">String</span><span class="sxs-lookup"><span data-stu-id="da5f9-138">String</span></span>|<span data-ttu-id="da5f9-139">项目的帮助文本</span><span class="sxs-lookup"><span data-stu-id="da5f9-139">Help text of the item</span></span>|
|<span data-ttu-id="da5f9-140">name</span><span class="sxs-lookup"><span data-stu-id="da5f9-140">name</span></span>|<span data-ttu-id="da5f9-141">String</span><span class="sxs-lookup"><span data-stu-id="da5f9-141">String</span></span>|<span data-ttu-id="da5f9-142">项目名称</span><span class="sxs-lookup"><span data-stu-id="da5f9-142">Name of the item</span></span>|
|<span data-ttu-id="da5f9-143">displayName</span><span class="sxs-lookup"><span data-stu-id="da5f9-143">displayName</span></span>|<span data-ttu-id="da5f9-144">String</span><span class="sxs-lookup"><span data-stu-id="da5f9-144">String</span></span>|<span data-ttu-id="da5f9-145">项目的显示名称</span><span class="sxs-lookup"><span data-stu-id="da5f9-145">Display name of the item</span></span>|
|<span data-ttu-id="da5f9-146">平台</span><span class="sxs-lookup"><span data-stu-id="da5f9-146">platforms</span></span>|[<span data-ttu-id="da5f9-147">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="da5f9-147">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="da5f9-148">平台类型，类别中的设置具有。</span><span class="sxs-lookup"><span data-stu-id="da5f9-148">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="da5f9-149">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="da5f9-149">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="da5f9-150">technologies</span><span class="sxs-lookup"><span data-stu-id="da5f9-150">technologies</span></span>|[<span data-ttu-id="da5f9-151">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="da5f9-151">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="da5f9-152">技术类型，类别中的设置具有。</span><span class="sxs-lookup"><span data-stu-id="da5f9-152">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="da5f9-153">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`。</span><span class="sxs-lookup"><span data-stu-id="da5f9-153">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="da5f9-154">settingUsage</span><span class="sxs-lookup"><span data-stu-id="da5f9-154">settingUsage</span></span>|[<span data-ttu-id="da5f9-155">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="da5f9-155">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="da5f9-156">指示类别包含用于合规性或配置的设置。</span><span class="sxs-lookup"><span data-stu-id="da5f9-156">Indicates that the category contains settings that are used for Compliance or Configuration.</span></span> <span data-ttu-id="da5f9-157">可取值为：`none`、`configuration`。</span><span class="sxs-lookup"><span data-stu-id="da5f9-157">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="da5f9-158">parentCategoryId</span><span class="sxs-lookup"><span data-stu-id="da5f9-158">parentCategoryId</span></span>|<span data-ttu-id="da5f9-159">String</span><span class="sxs-lookup"><span data-stu-id="da5f9-159">String</span></span>|<span data-ttu-id="da5f9-160">类别的父 ID。</span><span class="sxs-lookup"><span data-stu-id="da5f9-160">Parent id of the category.</span></span>|
|<span data-ttu-id="da5f9-161">rootCategoryId</span><span class="sxs-lookup"><span data-stu-id="da5f9-161">rootCategoryId</span></span>|<span data-ttu-id="da5f9-162">String</span><span class="sxs-lookup"><span data-stu-id="da5f9-162">String</span></span>|<span data-ttu-id="da5f9-163">类别的根 ID。</span><span class="sxs-lookup"><span data-stu-id="da5f9-163">Root id of the category.</span></span>|
|<span data-ttu-id="da5f9-164">childCategoryIds</span><span class="sxs-lookup"><span data-stu-id="da5f9-164">childCategoryIds</span></span>|<span data-ttu-id="da5f9-165">String collection</span><span class="sxs-lookup"><span data-stu-id="da5f9-165">String collection</span></span>|<span data-ttu-id="da5f9-166">类别的子 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="da5f9-166">List of child ids of the category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da5f9-167">关系</span><span class="sxs-lookup"><span data-stu-id="da5f9-167">Relationships</span></span>
<span data-ttu-id="da5f9-168">无</span><span class="sxs-lookup"><span data-stu-id="da5f9-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da5f9-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da5f9-169">JSON Representation</span></span>
<span data-ttu-id="da5f9-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da5f9-170">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "platforms": "String",
  "technologies": "String",
  "settingUsage": "String",
  "parentCategoryId": "String",
  "rootCategoryId": "String",
  "childCategoryIds": [
    "String"
  ]
}
```




