---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子图书类别的属性。
ms.openlocfilehash: 0e459a9c2fe1e644f98e3cdfa314d87c6f65fd67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047328"
---
# <a name="managedebookcategory-resource-type"></a><span data-ttu-id="7d4db-103">managedEBookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d4db-103">managedEBookCategory resource type</span></span>

> <span data-ttu-id="7d4db-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7d4db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d4db-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7d4db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d4db-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d4db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d4db-107">包含单个 Intune 电子图书类别的属性。</span><span class="sxs-lookup"><span data-stu-id="7d4db-107">Contains properties for a single Intune eBook category.</span></span>
## <a name="methods"></a><span data-ttu-id="7d4db-108">方法</span><span class="sxs-lookup"><span data-stu-id="7d4db-108">Methods</span></span>
|<span data-ttu-id="7d4db-109">方法</span><span class="sxs-lookup"><span data-stu-id="7d4db-109">Method</span></span>|<span data-ttu-id="7d4db-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d4db-110">Return Type</span></span>|<span data-ttu-id="7d4db-111">说明</span><span class="sxs-lookup"><span data-stu-id="7d4db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7d4db-112">列表 managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="7d4db-112">List managedEBookCategories</span></span>](../api/intune-books-managedebookcategory-list.md)|<span data-ttu-id="7d4db-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="7d4db-113">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="7d4db-114">列出属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="7d4db-114">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>|
|[<span data-ttu-id="7d4db-115">获取 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="7d4db-115">Get managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-get.md)|[<span data-ttu-id="7d4db-116">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="7d4db-116">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="7d4db-117">读取属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="7d4db-117">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="7d4db-118">创建 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="7d4db-118">Create managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-create.md)|[<span data-ttu-id="7d4db-119">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="7d4db-119">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="7d4db-120">创建新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7d4db-120">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|
|[<span data-ttu-id="7d4db-121">删除 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="7d4db-121">Delete managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-delete.md)|<span data-ttu-id="7d4db-122">无</span><span class="sxs-lookup"><span data-stu-id="7d4db-122">None</span></span>|<span data-ttu-id="7d4db-123">删除[managedEBookCategory](../resources/intune-books-managedebookcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="7d4db-123">Deletes a [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>|
|[<span data-ttu-id="7d4db-124">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="7d4db-124">Update managedEBookCategory</span></span>](../api/intune-books-managedebookcategory-update.md)|[<span data-ttu-id="7d4db-125">managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="7d4db-125">managedEBookCategory</span></span>](../resources/intune-books-managedebookcategory.md)|<span data-ttu-id="7d4db-126">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7d4db-126">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d4db-127">属性</span><span class="sxs-lookup"><span data-stu-id="7d4db-127">Properties</span></span>
|<span data-ttu-id="7d4db-128">属性</span><span class="sxs-lookup"><span data-stu-id="7d4db-128">Property</span></span>|<span data-ttu-id="7d4db-129">类型</span><span class="sxs-lookup"><span data-stu-id="7d4db-129">Type</span></span>|<span data-ttu-id="7d4db-130">说明</span><span class="sxs-lookup"><span data-stu-id="7d4db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d4db-131">id</span><span class="sxs-lookup"><span data-stu-id="7d4db-131">id</span></span>|<span data-ttu-id="7d4db-132">String</span><span class="sxs-lookup"><span data-stu-id="7d4db-132">String</span></span>|<span data-ttu-id="7d4db-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7d4db-133">The key of the entity.</span></span>|
|<span data-ttu-id="7d4db-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7d4db-134">displayName</span></span>|<span data-ttu-id="7d4db-135">字符串</span><span class="sxs-lookup"><span data-stu-id="7d4db-135">String</span></span>|<span data-ttu-id="7d4db-136">电子图书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="7d4db-136">The name of the eBook category.</span></span>|
|<span data-ttu-id="7d4db-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d4db-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7d4db-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d4db-138">DateTimeOffset</span></span>|<span data-ttu-id="7d4db-139">日期和 ManagedEBookCategory 上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="7d4db-139">The date and time the ManagedEBookCategory was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d4db-140">Relationships</span><span class="sxs-lookup"><span data-stu-id="7d4db-140">Relationships</span></span>
<span data-ttu-id="7d4db-141">无</span><span class="sxs-lookup"><span data-stu-id="7d4db-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d4db-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d4db-142">JSON Representation</span></span>
<span data-ttu-id="7d4db-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d4db-143">Here is a JSON representation of the resource.</span></span>
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





