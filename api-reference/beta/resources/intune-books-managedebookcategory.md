---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子书类别的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb7b15a76f055f9510ed62eab8ee41e0febc95be
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449761"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="13c09-103">managedEBookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="13c09-103">managedEBookCategory resource type</span></span>

<span data-ttu-id="13c09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13c09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13c09-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13c09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13c09-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13c09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c09-107">包含单个 Intune 电子书类别的属性。</span><span class="sxs-lookup"><span data-stu-id="13c09-107">Contains properties for a single Intune eBook category.</span></span>

## <a name="methods"></a><span data-ttu-id="13c09-108">方法</span><span class="sxs-lookup"><span data-stu-id="13c09-108">Methods</span></span>
|<span data-ttu-id="13c09-109">方法</span><span class="sxs-lookup"><span data-stu-id="13c09-109">Method</span></span>|<span data-ttu-id="13c09-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="13c09-110">Return Type</span></span>|<span data-ttu-id="13c09-111">说明</span><span class="sxs-lookup"><span data-stu-id="13c09-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13c09-112">列出 managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="13c09-112">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="13c09-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="13c09-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="13c09-114">列出[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13c09-114">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="13c09-115">获取 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="13c09-115">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="13c09-116">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="13c09-116">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="13c09-117">读取[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13c09-117">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="13c09-118">创建 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="13c09-118">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="13c09-119">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="13c09-119">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="13c09-120">创建新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="13c09-120">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="13c09-121">删除 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="13c09-121">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="13c09-122">无</span><span class="sxs-lookup"><span data-stu-id="13c09-122">None</span></span>|<span data-ttu-id="13c09-123">删除[managedEBookCategory](../resources/intune-books-managedebookcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="13c09-123">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="13c09-124">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="13c09-124">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="13c09-125">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="13c09-125">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="13c09-126">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13c09-126">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13c09-127">属性</span><span class="sxs-lookup"><span data-stu-id="13c09-127">Properties</span></span>
|<span data-ttu-id="13c09-128">属性</span><span class="sxs-lookup"><span data-stu-id="13c09-128">Property</span></span>|<span data-ttu-id="13c09-129">类型</span><span class="sxs-lookup"><span data-stu-id="13c09-129">Type</span></span>|<span data-ttu-id="13c09-130">说明</span><span class="sxs-lookup"><span data-stu-id="13c09-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c09-131">id</span><span class="sxs-lookup"><span data-stu-id="13c09-131">id</span></span>|<span data-ttu-id="13c09-132">String</span><span class="sxs-lookup"><span data-stu-id="13c09-132">String</span></span>|<span data-ttu-id="13c09-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="13c09-133">The key of the entity.</span></span>|
|<span data-ttu-id="13c09-134">displayName</span><span class="sxs-lookup"><span data-stu-id="13c09-134">displayName</span></span>|<span data-ttu-id="13c09-135">String</span><span class="sxs-lookup"><span data-stu-id="13c09-135">String</span></span>|<span data-ttu-id="13c09-136">电子书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="13c09-136">The name of the eBook category.</span></span>|
|<span data-ttu-id="13c09-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13c09-137">lastModifiedDateTime</span></span>|<span data-ttu-id="13c09-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13c09-138">DateTimeOffset</span></span>|<span data-ttu-id="13c09-139">上次修改 ManagedEBookCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="13c09-139">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13c09-140">关系</span><span class="sxs-lookup"><span data-stu-id="13c09-140">Relationships</span></span>
<span data-ttu-id="13c09-141">无</span><span class="sxs-lookup"><span data-stu-id="13c09-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13c09-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13c09-142">JSON Representation</span></span>
<span data-ttu-id="13c09-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13c09-143">Here is a JSON representation of the resource.</span></span>
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



