---
title: mobileAppCategory 资源类型
description: 包含单个 Intune 应用类别的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 190fc435cbcfb1ad262e93f86bec84de989f9194
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140563"
---
# <a name="mobileappcategory-resource-type"></a><span data-ttu-id="145af-103">mobileAppCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="145af-103">mobileAppCategory resource type</span></span>

> <span data-ttu-id="145af-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="145af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="145af-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="145af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="145af-106">包含单个 Intune 应用类别的属性。</span><span class="sxs-lookup"><span data-stu-id="145af-106">Contains properties for a single Intune app category.</span></span>

## <a name="methods"></a><span data-ttu-id="145af-107">方法</span><span class="sxs-lookup"><span data-stu-id="145af-107">Methods</span></span>
|<span data-ttu-id="145af-108">方法</span><span class="sxs-lookup"><span data-stu-id="145af-108">Method</span></span>|<span data-ttu-id="145af-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="145af-109">Return Type</span></span>|<span data-ttu-id="145af-110">说明</span><span class="sxs-lookup"><span data-stu-id="145af-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="145af-111">列出 mobileAppCategories</span><span class="sxs-lookup"><span data-stu-id="145af-111">List mobileAppCategories</span></span>](../api/intune-apps-mobileappcategory-list.md)|<span data-ttu-id="145af-112">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="145af-112">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="145af-113">列出 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="145af-113">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>|
|[<span data-ttu-id="145af-114">获取 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="145af-114">Get mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-get.md)|[<span data-ttu-id="145af-115">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="145af-115">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="145af-116">读取 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="145af-116">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="145af-117">创建 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="145af-117">Create mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-create.md)|[<span data-ttu-id="145af-118">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="145af-118">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="145af-119">创建新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="145af-119">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|
|[<span data-ttu-id="145af-120">删除 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="145af-120">Delete mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-delete.md)|<span data-ttu-id="145af-121">无</span><span class="sxs-lookup"><span data-stu-id="145af-121">None</span></span>|<span data-ttu-id="145af-122">删除 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="145af-122">Deletes a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>|
|[<span data-ttu-id="145af-123">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="145af-123">Update mobileAppCategory</span></span>](../api/intune-apps-mobileappcategory-update.md)|[<span data-ttu-id="145af-124">mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="145af-124">mobileAppCategory</span></span>](../resources/intune-apps-mobileappcategory.md)|<span data-ttu-id="145af-125">更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="145af-125">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="145af-126">属性</span><span class="sxs-lookup"><span data-stu-id="145af-126">Properties</span></span>
|<span data-ttu-id="145af-127">属性</span><span class="sxs-lookup"><span data-stu-id="145af-127">Property</span></span>|<span data-ttu-id="145af-128">类型</span><span class="sxs-lookup"><span data-stu-id="145af-128">Type</span></span>|<span data-ttu-id="145af-129">说明</span><span class="sxs-lookup"><span data-stu-id="145af-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="145af-130">id</span><span class="sxs-lookup"><span data-stu-id="145af-130">id</span></span>|<span data-ttu-id="145af-131">String</span><span class="sxs-lookup"><span data-stu-id="145af-131">String</span></span>|<span data-ttu-id="145af-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="145af-132">The key of the entity.</span></span>|
|<span data-ttu-id="145af-133">displayName</span><span class="sxs-lookup"><span data-stu-id="145af-133">displayName</span></span>|<span data-ttu-id="145af-134">String</span><span class="sxs-lookup"><span data-stu-id="145af-134">String</span></span>|<span data-ttu-id="145af-135">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="145af-135">The name of the app category.</span></span>|
|<span data-ttu-id="145af-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="145af-136">lastModifiedDateTime</span></span>|<span data-ttu-id="145af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="145af-137">DateTimeOffset</span></span>|<span data-ttu-id="145af-138">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="145af-138">The date and time the mobileAppCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="145af-139">关系</span><span class="sxs-lookup"><span data-stu-id="145af-139">Relationships</span></span>
<span data-ttu-id="145af-140">无</span><span class="sxs-lookup"><span data-stu-id="145af-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="145af-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="145af-141">JSON Representation</span></span>
<span data-ttu-id="145af-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="145af-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




