---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子图书类别的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f4136fbfb93db6e7e9dee4a81dcc44a613a7226
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915954"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="55474-103">managedEBookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="55474-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="55474-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55474-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55474-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55474-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55474-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55474-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55474-107">包含单个 Intune 电子图书类别的属性。</span><span class="sxs-lookup"><span data-stu-id="55474-107">Contains properties for a single Intune eBook category.</span></span>
## <a name="methods"></a><span data-ttu-id="55474-108">方法</span><span class="sxs-lookup"><span data-stu-id="55474-108">Methods</span></span>
|<span data-ttu-id="55474-109">方法</span><span class="sxs-lookup"><span data-stu-id="55474-109">Method</span></span>|<span data-ttu-id="55474-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="55474-110">Return Type</span></span>|<span data-ttu-id="55474-111">说明</span><span class="sxs-lookup"><span data-stu-id="55474-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55474-112">列表 managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="55474-112">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="55474-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="55474-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="55474-114">列出属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="55474-114">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="55474-115">获取 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="55474-115">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="55474-116">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="55474-116">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="55474-117">读取属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="55474-117">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="55474-118">创建 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="55474-118">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="55474-119">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="55474-119">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="55474-120">创建新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="55474-120">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="55474-121">删除 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="55474-121">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="55474-122">无</span><span class="sxs-lookup"><span data-stu-id="55474-122">None</span></span>|<span data-ttu-id="55474-123">删除[managedEBookCategory](../resources/intune-books-managedebookcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="55474-123">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="55474-124">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="55474-124">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="55474-125">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="55474-125">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="55474-126">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="55474-126">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55474-127">属性</span><span class="sxs-lookup"><span data-stu-id="55474-127">Properties</span></span>
|<span data-ttu-id="55474-128">属性</span><span class="sxs-lookup"><span data-stu-id="55474-128">Property</span></span>|<span data-ttu-id="55474-129">类型</span><span class="sxs-lookup"><span data-stu-id="55474-129">Type</span></span>|<span data-ttu-id="55474-130">说明</span><span class="sxs-lookup"><span data-stu-id="55474-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55474-131">id</span><span class="sxs-lookup"><span data-stu-id="55474-131">id</span></span>|<span data-ttu-id="55474-132">String</span><span class="sxs-lookup"><span data-stu-id="55474-132">String</span></span>|<span data-ttu-id="55474-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="55474-133">The key of the entity.</span></span>|
|<span data-ttu-id="55474-134">displayName</span><span class="sxs-lookup"><span data-stu-id="55474-134">displayName</span></span>|<span data-ttu-id="55474-135">字符串</span><span class="sxs-lookup"><span data-stu-id="55474-135">String</span></span>|<span data-ttu-id="55474-136">电子图书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="55474-136">The name of the eBook category.</span></span>|
|<span data-ttu-id="55474-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55474-137">lastModifiedDateTime</span></span>|<span data-ttu-id="55474-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55474-138">DateTimeOffset</span></span>|<span data-ttu-id="55474-139">日期和 ManagedEBookCategory 上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="55474-139">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55474-140">Relationships</span><span class="sxs-lookup"><span data-stu-id="55474-140">Relationships</span></span>
<span data-ttu-id="55474-141">无</span><span class="sxs-lookup"><span data-stu-id="55474-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55474-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55474-142">JSON Representation</span></span>
<span data-ttu-id="55474-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55474-143">Here is a JSON representation of the resource.</span></span>
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





