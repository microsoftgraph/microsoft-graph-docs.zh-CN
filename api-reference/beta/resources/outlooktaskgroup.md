---
title: outlookTaskGroup 资源类型
description: '一组文件夹（outlookTaskFolder），其中包含 Outlook 任务（outlookTask 对象的集合）。 '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8018863ed7fd142b99e0008f860495a4d13d4e01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463208"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="c1c00-103">outlookTaskGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1c00-103">outlookTaskGroup resource type</span></span>

<span data-ttu-id="c1c00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1c00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1c00-105">一组文件夹（[outlookTaskFolder](outlooktaskfolder.md)），其中包含 Outlook 任务（ [outlookTask](outlooktask.md)对象的集合）。</span><span class="sxs-lookup"><span data-stu-id="c1c00-105">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="c1c00-106">在 Outlook 中，有一个不能重`My Tasks`命名或删除的默认任务组。</span><span class="sxs-lookup"><span data-stu-id="c1c00-106">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="c1c00-107">不过，您可以创建其他任务组。</span><span class="sxs-lookup"><span data-stu-id="c1c00-107">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="c1c00-108">方法</span><span class="sxs-lookup"><span data-stu-id="c1c00-108">Methods</span></span>

| <span data-ttu-id="c1c00-109">方法</span><span class="sxs-lookup"><span data-stu-id="c1c00-109">Method</span></span>           | <span data-ttu-id="c1c00-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c1c00-110">Return Type</span></span>    |<span data-ttu-id="c1c00-111">说明</span><span class="sxs-lookup"><span data-stu-id="c1c00-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1c00-112">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c1c00-112">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="c1c00-113">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c1c00-113">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="c1c00-114">获取指定的 Outlook 任务组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1c00-114">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="c1c00-115">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c1c00-115">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="c1c00-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c1c00-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="c1c00-117">创建一个 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="c1c00-117">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="c1c00-118">列出 taskFolders</span><span class="sxs-lookup"><span data-stu-id="c1c00-118">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="c1c00-119">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="c1c00-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c1c00-120">获取 Outlook 任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="c1c00-120">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="c1c00-121">更新</span><span class="sxs-lookup"><span data-stu-id="c1c00-121">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="c1c00-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c1c00-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="c1c00-123">更新 Outlook 任务组的可写属性。</span><span class="sxs-lookup"><span data-stu-id="c1c00-123">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="c1c00-124">删除</span><span class="sxs-lookup"><span data-stu-id="c1c00-124">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="c1c00-125">无</span><span class="sxs-lookup"><span data-stu-id="c1c00-125">None</span></span> |<span data-ttu-id="c1c00-126">删除指定的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="c1c00-126">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="c1c00-127">属性</span><span class="sxs-lookup"><span data-stu-id="c1c00-127">Properties</span></span>
| <span data-ttu-id="c1c00-128">属性</span><span class="sxs-lookup"><span data-stu-id="c1c00-128">Property</span></span>     | <span data-ttu-id="c1c00-129">类型</span><span class="sxs-lookup"><span data-stu-id="c1c00-129">Type</span></span>   |<span data-ttu-id="c1c00-130">说明</span><span class="sxs-lookup"><span data-stu-id="c1c00-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1c00-131">changeKey</span><span class="sxs-lookup"><span data-stu-id="c1c00-131">changeKey</span></span>|<span data-ttu-id="c1c00-132">String</span><span class="sxs-lookup"><span data-stu-id="c1c00-132">String</span></span>|<span data-ttu-id="c1c00-133">任务组的版本。</span><span class="sxs-lookup"><span data-stu-id="c1c00-133">The version of the task group.</span></span>|
|<span data-ttu-id="c1c00-134">groupKey</span><span class="sxs-lookup"><span data-stu-id="c1c00-134">groupKey</span></span>|<span data-ttu-id="c1c00-135">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="c1c00-135">Edm.Guid</span></span>|<span data-ttu-id="c1c00-136">任务组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="c1c00-136">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="c1c00-137">id</span><span class="sxs-lookup"><span data-stu-id="c1c00-137">id</span></span>|<span data-ttu-id="c1c00-138">String</span><span class="sxs-lookup"><span data-stu-id="c1c00-138">String</span></span>|<span data-ttu-id="c1c00-139">任务组的唯一字符串标识符。</span><span class="sxs-lookup"><span data-stu-id="c1c00-139">The unique string identifier of the task group.</span></span> <span data-ttu-id="c1c00-140">只读。</span><span class="sxs-lookup"><span data-stu-id="c1c00-140">Read-only.</span></span>|
|<span data-ttu-id="c1c00-141">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="c1c00-141">isDefaultGroup</span></span>|<span data-ttu-id="c1c00-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="c1c00-142">Boolean</span></span>|<span data-ttu-id="c1c00-143">如此如果任务组是默认任务组。</span><span class="sxs-lookup"><span data-stu-id="c1c00-143">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="c1c00-144">name</span><span class="sxs-lookup"><span data-stu-id="c1c00-144">name</span></span>|<span data-ttu-id="c1c00-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c1c00-145">String</span></span>|<span data-ttu-id="c1c00-146">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="c1c00-146">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1c00-147">关系</span><span class="sxs-lookup"><span data-stu-id="c1c00-147">Relationships</span></span>
| <span data-ttu-id="c1c00-148">关系</span><span class="sxs-lookup"><span data-stu-id="c1c00-148">Relationship</span></span> | <span data-ttu-id="c1c00-149">类型</span><span class="sxs-lookup"><span data-stu-id="c1c00-149">Type</span></span>   |<span data-ttu-id="c1c00-150">说明</span><span class="sxs-lookup"><span data-stu-id="c1c00-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1c00-151">taskFolders</span><span class="sxs-lookup"><span data-stu-id="c1c00-151">taskFolders</span></span>|<span data-ttu-id="c1c00-152">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="c1c00-152">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="c1c00-153">任务组中的任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="c1c00-153">The collection of task folders in the task group.</span></span> <span data-ttu-id="c1c00-154">只读。</span><span class="sxs-lookup"><span data-stu-id="c1c00-154">Read-only.</span></span> <span data-ttu-id="c1c00-155">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c1c00-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1c00-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1c00-156">JSON representation</span></span>
<span data-ttu-id="c1c00-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1c00-157">Here is a JSON representation of the resource.</span></span>

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
