---
title: outlookTaskGroup 资源类型
description: 'outlookTaskFolder (outlookTaskFolder) 包含 outlookTask 对象 (集合中的一组) 。 '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 112ffab7699a2c8812311ba0c21c2b0e47efff70
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849786"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="90ff4-103">outlookTaskGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="90ff4-103">outlookTaskGroup resource type</span></span>

<span data-ttu-id="90ff4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ff4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="90ff4-105">[outlookTaskFolder (一组](outlooktaskfolder.md)) [outlookTaskfolder](outlooktask.md)对象 (outlookTask 对象的集合) 。</span><span class="sxs-lookup"><span data-stu-id="90ff4-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="90ff4-106">在 Outlook 中，有一个您无法 `My Tasks` 重命名或删除的默认任务组。</span><span class="sxs-lookup"><span data-stu-id="90ff4-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="90ff4-107">但是，你可以创建其他任务组。</span><span class="sxs-lookup"><span data-stu-id="90ff4-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="90ff4-108">方法</span><span class="sxs-lookup"><span data-stu-id="90ff4-108">Methods</span></span>

| <span data-ttu-id="90ff4-109">方法</span><span class="sxs-lookup"><span data-stu-id="90ff4-109">Method</span></span>           | <span data-ttu-id="90ff4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="90ff4-110">Return Type</span></span>    |<span data-ttu-id="90ff4-111">说明</span><span class="sxs-lookup"><span data-stu-id="90ff4-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90ff4-112">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="90ff4-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="90ff4-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="90ff4-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="90ff4-114">获取指定的 Outlook 任务组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90ff4-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="90ff4-115">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="90ff4-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="90ff4-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="90ff4-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="90ff4-117">创建 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="90ff4-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="90ff4-118">列出 taskFolders</span><span class="sxs-lookup"><span data-stu-id="90ff4-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="90ff4-119">[outlookTaskFolder](outlooktaskfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90ff4-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="90ff4-120">获取 Outlook 任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="90ff4-120">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="90ff4-121">更新</span><span class="sxs-lookup"><span data-stu-id="90ff4-121">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="90ff4-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="90ff4-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="90ff4-123">更新 Outlook 任务组的可写属性。</span><span class="sxs-lookup"><span data-stu-id="90ff4-123">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="90ff4-124">删除</span><span class="sxs-lookup"><span data-stu-id="90ff4-124">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="90ff4-125">无</span><span class="sxs-lookup"><span data-stu-id="90ff4-125">None</span></span> |<span data-ttu-id="90ff4-126">删除指定的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="90ff4-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="90ff4-127">属性</span><span class="sxs-lookup"><span data-stu-id="90ff4-127">Properties</span></span>
| <span data-ttu-id="90ff4-128">属性</span><span class="sxs-lookup"><span data-stu-id="90ff4-128">Property</span></span>     | <span data-ttu-id="90ff4-129">类型</span><span class="sxs-lookup"><span data-stu-id="90ff4-129">Type</span></span>   |<span data-ttu-id="90ff4-130">说明</span><span class="sxs-lookup"><span data-stu-id="90ff4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90ff4-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="90ff4-131">changeKey</span></span>|<span data-ttu-id="90ff4-132">String</span><span class="sxs-lookup"><span data-stu-id="90ff4-132">String</span></span>|<span data-ttu-id="90ff4-133">任务组的版本。</span><span class="sxs-lookup"><span data-stu-id="90ff4-133">The version of the task group.</span></span>|
|<span data-ttu-id="90ff4-134">groupKey</span><span class="sxs-lookup"><span data-stu-id="90ff4-134">groupKey</span></span>|<span data-ttu-id="90ff4-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="90ff4-135">Edm.Guid</span></span>|<span data-ttu-id="90ff4-136">任务组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="90ff4-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="90ff4-137">id</span><span class="sxs-lookup"><span data-stu-id="90ff4-137">id</span></span>|<span data-ttu-id="90ff4-138">String</span><span class="sxs-lookup"><span data-stu-id="90ff4-138">String</span></span>|<span data-ttu-id="90ff4-139">任务组的唯一字符串标识符。</span><span class="sxs-lookup"><span data-stu-id="90ff4-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="90ff4-140">只读。</span><span class="sxs-lookup"><span data-stu-id="90ff4-140">Read-only.</span></span>|
|<span data-ttu-id="90ff4-141">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="90ff4-141">isDefaultGroup</span></span>|<span data-ttu-id="90ff4-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="90ff4-142">Boolean</span></span>|<span data-ttu-id="90ff4-143">如此 如果任务组是默认任务组。</span><span class="sxs-lookup"><span data-stu-id="90ff4-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="90ff4-144">name</span><span class="sxs-lookup"><span data-stu-id="90ff4-144">name</span></span>|<span data-ttu-id="90ff4-145">String</span><span class="sxs-lookup"><span data-stu-id="90ff4-145">String</span></span>|<span data-ttu-id="90ff4-146">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="90ff4-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ff4-147">关系</span><span class="sxs-lookup"><span data-stu-id="90ff4-147">Relationships</span></span>
| <span data-ttu-id="90ff4-148">关系</span><span class="sxs-lookup"><span data-stu-id="90ff4-148">Relationship</span></span> | <span data-ttu-id="90ff4-149">类型</span><span class="sxs-lookup"><span data-stu-id="90ff4-149">Type</span></span>   |<span data-ttu-id="90ff4-150">说明</span><span class="sxs-lookup"><span data-stu-id="90ff4-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90ff4-151">taskFolders</span><span class="sxs-lookup"><span data-stu-id="90ff4-151">taskFolders</span></span>|<span data-ttu-id="90ff4-152">[outlookTaskFolder](outlooktaskfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90ff4-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="90ff4-153">任务组中的任务文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="90ff4-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="90ff4-154">只读。</span><span class="sxs-lookup"><span data-stu-id="90ff4-154">Read-only.</span></span> <span data-ttu-id="90ff4-155">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90ff4-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90ff4-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90ff4-156">JSON representation</span></span>
<span data-ttu-id="90ff4-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90ff4-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
