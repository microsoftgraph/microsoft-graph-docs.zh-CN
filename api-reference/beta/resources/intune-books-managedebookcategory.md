---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子图书类别的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df057c3aa05d181365397d150aeae93754b63dad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415332"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="ca4c4-103">managedEBookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca4c4-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="ca4c4-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca4c4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca4c4-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca4c4-107">包含单个 Intune 电子图书类别的属性。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-107">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="ca4c4-108">方法</span><span class="sxs-lookup"><span data-stu-id="ca4c4-108">Methods</span></span>
|<span data-ttu-id="ca4c4-109">方法</span><span class="sxs-lookup"><span data-stu-id="ca4c4-109">Method</span></span>|<span data-ttu-id="ca4c4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca4c4-110">Return Type</span></span>|<span data-ttu-id="ca4c4-111">说明</span><span class="sxs-lookup"><span data-stu-id="ca4c4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca4c4-112">列表 managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="ca4c4-112">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="ca4c4-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca4c4-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="ca4c4-114">列出属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-114">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="ca4c4-115">获取 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="ca4c4-115">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="ca4c4-116">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="ca4c4-116">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="ca4c4-117">读取属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-117">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="ca4c4-118">创建 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="ca4c4-118">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="ca4c4-119">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="ca4c4-119">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="ca4c4-120">创建新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-120">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="ca4c4-121">删除 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="ca4c4-121">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="ca4c4-122">无</span><span class="sxs-lookup"><span data-stu-id="ca4c4-122">None</span></span>|<span data-ttu-id="ca4c4-123">删除[managedEBookCategory](../resources/intune-books-managedebookcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-123">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="ca4c4-124">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="ca4c4-124">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="ca4c4-125">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="ca4c4-125">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="ca4c4-126">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-126">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca4c4-127">属性</span><span class="sxs-lookup"><span data-stu-id="ca4c4-127">Properties</span></span>
|<span data-ttu-id="ca4c4-128">属性</span><span class="sxs-lookup"><span data-stu-id="ca4c4-128">Property</span></span>|<span data-ttu-id="ca4c4-129">类型</span><span class="sxs-lookup"><span data-stu-id="ca4c4-129">Type</span></span>|<span data-ttu-id="ca4c4-130">说明</span><span class="sxs-lookup"><span data-stu-id="ca4c4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca4c4-131">id</span><span class="sxs-lookup"><span data-stu-id="ca4c4-131">id</span></span>|<span data-ttu-id="ca4c4-132">String</span><span class="sxs-lookup"><span data-stu-id="ca4c4-132">String</span></span>|<span data-ttu-id="ca4c4-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-133">The key of the entity.</span></span>|
|<span data-ttu-id="ca4c4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ca4c4-134">displayName</span></span>|<span data-ttu-id="ca4c4-135">String</span><span class="sxs-lookup"><span data-stu-id="ca4c4-135">String</span></span>|<span data-ttu-id="ca4c4-136">电子图书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-136">The name of the eBook category.</span></span>|
|<span data-ttu-id="ca4c4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca4c4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ca4c4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca4c4-138">DateTimeOffset</span></span>|<span data-ttu-id="ca4c4-139">日期和 ManagedEBookCategory 上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-139">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca4c4-140">关系</span><span class="sxs-lookup"><span data-stu-id="ca4c4-140">Relationships</span></span>
<span data-ttu-id="ca4c4-141">无</span><span class="sxs-lookup"><span data-stu-id="ca4c4-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca4c4-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca4c4-142">JSON Representation</span></span>
<span data-ttu-id="ca4c4-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca4c4-143">Here is a JSON representation of the resource.</span></span>
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




