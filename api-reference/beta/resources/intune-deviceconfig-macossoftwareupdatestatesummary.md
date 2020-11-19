---
title: macOSSoftwareUpdateStateSummary 资源类型
description: MacOS 设备和用户的软件更新状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb7cebab56f9866753794259b70a0bdd8cc1e414
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279813"
---
# <a name="macossoftwareupdatestatesummary-resource-type"></a><span data-ttu-id="d9e40-103">macOSSoftwareUpdateStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9e40-103">macOSSoftwareUpdateStateSummary resource type</span></span>

<span data-ttu-id="d9e40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9e40-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9e40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e40-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9e40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e40-107">MacOS 设备和用户的软件更新状态摘要</span><span class="sxs-lookup"><span data-stu-id="d9e40-107">MacOS software update state summary for a device and user</span></span>

## <a name="methods"></a><span data-ttu-id="d9e40-108">方法</span><span class="sxs-lookup"><span data-stu-id="d9e40-108">Methods</span></span>
|<span data-ttu-id="d9e40-109">方法</span><span class="sxs-lookup"><span data-stu-id="d9e40-109">Method</span></span>|<span data-ttu-id="d9e40-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9e40-110">Return Type</span></span>|<span data-ttu-id="d9e40-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9e40-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9e40-112">列出 macOSSoftwareUpdateStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d9e40-112">List macOSSoftwareUpdateStateSummaries</span></span>](../api/intune-deviceconfig-macossoftwareupdatestatesummary-list.md)|<span data-ttu-id="d9e40-113">[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9e40-113">[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) collection</span></span>|<span data-ttu-id="d9e40-114">列出 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9e40-114">List properties and relationships of the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) objects.</span></span>|
|[<span data-ttu-id="d9e40-115">获取 macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9e40-115">Get macOSSoftwareUpdateStateSummary</span></span>](../api/intune-deviceconfig-macossoftwareupdatestatesummary-get.md)|[<span data-ttu-id="d9e40-116">macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9e40-116">macOSSoftwareUpdateStateSummary</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|<span data-ttu-id="d9e40-117">读取 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9e40-117">Read properties and relationships of the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>|
|[<span data-ttu-id="d9e40-118">创建 macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9e40-118">Create macOSSoftwareUpdateStateSummary</span></span>](../api/intune-deviceconfig-macossoftwareupdatestatesummary-create.md)|[<span data-ttu-id="d9e40-119">macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9e40-119">macOSSoftwareUpdateStateSummary</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|<span data-ttu-id="d9e40-120">创建新的 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9e40-120">Create a new [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>|
|[<span data-ttu-id="d9e40-121">删除 macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9e40-121">Delete macOSSoftwareUpdateStateSummary</span></span>](../api/intune-deviceconfig-macossoftwareupdatestatesummary-delete.md)|<span data-ttu-id="d9e40-122">无</span><span class="sxs-lookup"><span data-stu-id="d9e40-122">None</span></span>|<span data-ttu-id="d9e40-123">删除 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="d9e40-123">Deletes a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span></span>|
|[<span data-ttu-id="d9e40-124">更新 macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9e40-124">Update macOSSoftwareUpdateStateSummary</span></span>](../api/intune-deviceconfig-macossoftwareupdatestatesummary-update.md)|[<span data-ttu-id="d9e40-125">macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9e40-125">macOSSoftwareUpdateStateSummary</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|<span data-ttu-id="d9e40-126">更新 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9e40-126">Update the properties of a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9e40-127">属性</span><span class="sxs-lookup"><span data-stu-id="d9e40-127">Properties</span></span>
|<span data-ttu-id="d9e40-128">属性</span><span class="sxs-lookup"><span data-stu-id="d9e40-128">Property</span></span>|<span data-ttu-id="d9e40-129">类型</span><span class="sxs-lookup"><span data-stu-id="d9e40-129">Type</span></span>|<span data-ttu-id="d9e40-130">说明</span><span class="sxs-lookup"><span data-stu-id="d9e40-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e40-131">id</span><span class="sxs-lookup"><span data-stu-id="d9e40-131">id</span></span>|<span data-ttu-id="d9e40-132">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e40-132">String</span></span>|<span data-ttu-id="d9e40-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9e40-133">Key of the entity.</span></span>|
|<span data-ttu-id="d9e40-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d9e40-134">displayName</span></span>|<span data-ttu-id="d9e40-135">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e40-135">String</span></span>|<span data-ttu-id="d9e40-136">人工可读名称的软件更新</span><span class="sxs-lookup"><span data-stu-id="d9e40-136">Human readable name of the software update</span></span>|
|<span data-ttu-id="d9e40-137">productKey</span><span class="sxs-lookup"><span data-stu-id="d9e40-137">productKey</span></span>|<span data-ttu-id="d9e40-138">String</span><span class="sxs-lookup"><span data-stu-id="d9e40-138">String</span></span>|<span data-ttu-id="d9e40-139">软件更新的产品密钥。</span><span class="sxs-lookup"><span data-stu-id="d9e40-139">Product key of the software update.</span></span>|
|<span data-ttu-id="d9e40-140">updateCategory</span><span class="sxs-lookup"><span data-stu-id="d9e40-140">updateCategory</span></span>|[<span data-ttu-id="d9e40-141">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="d9e40-141">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="d9e40-142">软件更新类别。</span><span class="sxs-lookup"><span data-stu-id="d9e40-142">Software update category.</span></span> <span data-ttu-id="d9e40-143">可取值为：`critical`、`configurationDataFile`、`firmware`、`other`。</span><span class="sxs-lookup"><span data-stu-id="d9e40-143">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="d9e40-144">updateVersion</span><span class="sxs-lookup"><span data-stu-id="d9e40-144">updateVersion</span></span>|<span data-ttu-id="d9e40-145">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e40-145">String</span></span>|<span data-ttu-id="d9e40-146">软件更新的版本</span><span class="sxs-lookup"><span data-stu-id="d9e40-146">Version of the software update</span></span>|
|<span data-ttu-id="d9e40-147">state</span><span class="sxs-lookup"><span data-stu-id="d9e40-147">state</span></span>|[<span data-ttu-id="d9e40-148">macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="d9e40-148">macOSSoftwareUpdateState</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|<span data-ttu-id="d9e40-149">软件更新的状态。</span><span class="sxs-lookup"><span data-stu-id="d9e40-149">State of the software update.</span></span> <span data-ttu-id="d9e40-150">可能的值为：、、、、、、、、、、、、、、 `success` `downloading` `downloaded` `installing` `idle` `available` `scheduled` `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` 。</span><span class="sxs-lookup"><span data-stu-id="d9e40-150">Possible values are: `success`, `downloading`, `downloaded`, `installing`, `idle`, `available`, `scheduled`, `downloadFailed`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installInsufficientSpace`, `installInsufficientPower`, `installFailed`, `commandFailed`.</span></span>|
|<span data-ttu-id="d9e40-151">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e40-151">lastUpdatedDateTime</span></span>|<span data-ttu-id="d9e40-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e40-152">DateTimeOffset</span></span>|<span data-ttu-id="d9e40-153">最后一次更新此设备和产品密钥的报告的日期。</span><span class="sxs-lookup"><span data-stu-id="d9e40-153">Last date time the report for this device and product key was updated.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9e40-154">关系</span><span class="sxs-lookup"><span data-stu-id="d9e40-154">Relationships</span></span>
<span data-ttu-id="d9e40-155">无</span><span class="sxs-lookup"><span data-stu-id="d9e40-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9e40-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9e40-156">JSON Representation</span></span>
<span data-ttu-id="d9e40-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9e40-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "productKey": "String",
  "updateCategory": "String",
  "updateVersion": "String",
  "state": "String",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




