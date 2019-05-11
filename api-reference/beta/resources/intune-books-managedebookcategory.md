---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子书类别的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0baa3dbbecd90483eeb182edf486fcd6bfdd846b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949316"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="3f55c-103">managedEBookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f55c-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="3f55c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f55c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f55c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f55c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f55c-106">包含单个 Intune 电子书类别的属性。</span><span class="sxs-lookup"><span data-stu-id="3f55c-106">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="3f55c-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f55c-107">Methods</span></span>
|<span data-ttu-id="3f55c-108">方法</span><span class="sxs-lookup"><span data-stu-id="3f55c-108">Method</span></span>|<span data-ttu-id="3f55c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f55c-109">Return Type</span></span>|<span data-ttu-id="3f55c-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f55c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f55c-111">列出 managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="3f55c-111">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="3f55c-112">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f55c-112">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="3f55c-113">列出[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f55c-113">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="3f55c-114">获取 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3f55c-114">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="3f55c-115">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3f55c-115">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="3f55c-116">读取[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f55c-116">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="3f55c-117">创建 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3f55c-117">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="3f55c-118">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3f55c-118">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="3f55c-119">创建新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3f55c-119">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="3f55c-120">删除 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3f55c-120">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="3f55c-121">无</span><span class="sxs-lookup"><span data-stu-id="3f55c-121">None</span></span>|<span data-ttu-id="3f55c-122">删除[managedEBookCategory](../resources/intune-books-managedebookcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="3f55c-122">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="3f55c-123">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3f55c-123">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="3f55c-124">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3f55c-124">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="3f55c-125">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f55c-125">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f55c-126">属性</span><span class="sxs-lookup"><span data-stu-id="3f55c-126">Properties</span></span>
|<span data-ttu-id="3f55c-127">属性</span><span class="sxs-lookup"><span data-stu-id="3f55c-127">Property</span></span>|<span data-ttu-id="3f55c-128">类型</span><span class="sxs-lookup"><span data-stu-id="3f55c-128">Type</span></span>|<span data-ttu-id="3f55c-129">说明</span><span class="sxs-lookup"><span data-stu-id="3f55c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f55c-130">id</span><span class="sxs-lookup"><span data-stu-id="3f55c-130">id</span></span>|<span data-ttu-id="3f55c-131">String</span><span class="sxs-lookup"><span data-stu-id="3f55c-131">String</span></span>|<span data-ttu-id="3f55c-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3f55c-132">The key of the entity.</span></span>|
|<span data-ttu-id="3f55c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3f55c-133">displayName</span></span>|<span data-ttu-id="3f55c-134">String</span><span class="sxs-lookup"><span data-stu-id="3f55c-134">String</span></span>|<span data-ttu-id="3f55c-135">电子书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="3f55c-135">The name of the eBook category.</span></span>|
|<span data-ttu-id="3f55c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f55c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3f55c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f55c-137">DateTimeOffset</span></span>|<span data-ttu-id="3f55c-138">上次修改 ManagedEBookCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3f55c-138">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f55c-139">关系</span><span class="sxs-lookup"><span data-stu-id="3f55c-139">Relationships</span></span>
<span data-ttu-id="3f55c-140">无</span><span class="sxs-lookup"><span data-stu-id="3f55c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f55c-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f55c-141">JSON Representation</span></span>
<span data-ttu-id="3f55c-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f55c-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




