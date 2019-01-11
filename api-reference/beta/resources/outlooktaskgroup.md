---
title: outlookTaskGroup 资源类型
description: '包含 Outlook 任务 （outlookTask 对象的集合） 的文件夹 (outlookTaskFolder) 组。 '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5e885c4c8cc2abe4b3890635e010d495267dc877
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878769"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="d42ce-103">outlookTaskGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="d42ce-103">outlookTaskGroup resource type</span></span>

> <span data-ttu-id="d42ce-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d42ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d42ce-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d42ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d42ce-106">包含 Outlook 任务 （ [outlookTask](outlooktask.md)对象的集合） 的文件夹 ([outlookTaskFolder](outlooktaskfolder.md)) 组。</span><span class="sxs-lookup"><span data-stu-id="d42ce-106">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="d42ce-107">在 Outlook 中，没有默认任务组`My Tasks`无法重命名或删除。</span><span class="sxs-lookup"><span data-stu-id="d42ce-107">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="d42ce-108">但是，您可以创建其他任务组。</span><span class="sxs-lookup"><span data-stu-id="d42ce-108">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="d42ce-109">方法</span><span class="sxs-lookup"><span data-stu-id="d42ce-109">Methods</span></span>

| <span data-ttu-id="d42ce-110">方法</span><span class="sxs-lookup"><span data-stu-id="d42ce-110">Method</span></span>           | <span data-ttu-id="d42ce-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d42ce-111">Return Type</span></span>    |<span data-ttu-id="d42ce-112">说明</span><span class="sxs-lookup"><span data-stu-id="d42ce-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d42ce-113">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d42ce-113">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="d42ce-114">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d42ce-114">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="d42ce-115">要获取的属性和指定 Outlook 任务组的关系。</span><span class="sxs-lookup"><span data-stu-id="d42ce-115">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="d42ce-116">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="d42ce-116">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="d42ce-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="d42ce-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="d42ce-118">创建 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="d42ce-118">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="d42ce-119">列表 taskFolders</span><span class="sxs-lookup"><span data-stu-id="d42ce-119">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="d42ce-120">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="d42ce-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="d42ce-121">获取 Outlook 任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="d42ce-121">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="d42ce-122">Update</span><span class="sxs-lookup"><span data-stu-id="d42ce-122">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="d42ce-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="d42ce-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="d42ce-124">更新 Outlook 任务组的可写属性。</span><span class="sxs-lookup"><span data-stu-id="d42ce-124">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="d42ce-125">删除</span><span class="sxs-lookup"><span data-stu-id="d42ce-125">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="d42ce-126">无</span><span class="sxs-lookup"><span data-stu-id="d42ce-126">None</span></span> |<span data-ttu-id="d42ce-127">删除指定的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="d42ce-127">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="d42ce-128">属性</span><span class="sxs-lookup"><span data-stu-id="d42ce-128">Properties</span></span>
| <span data-ttu-id="d42ce-129">属性</span><span class="sxs-lookup"><span data-stu-id="d42ce-129">Property</span></span>     | <span data-ttu-id="d42ce-130">类型</span><span class="sxs-lookup"><span data-stu-id="d42ce-130">Type</span></span>   |<span data-ttu-id="d42ce-131">说明</span><span class="sxs-lookup"><span data-stu-id="d42ce-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d42ce-132">changeKey</span><span class="sxs-lookup"><span data-stu-id="d42ce-132">changeKey</span></span>|<span data-ttu-id="d42ce-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d42ce-133">String</span></span>|<span data-ttu-id="d42ce-134">任务组的版本。</span><span class="sxs-lookup"><span data-stu-id="d42ce-134">The version of the task group.</span></span>|
|<span data-ttu-id="d42ce-135">groupKey</span><span class="sxs-lookup"><span data-stu-id="d42ce-135">groupKey</span></span>|<span data-ttu-id="d42ce-136">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="d42ce-136">Edm.Guid</span></span>|<span data-ttu-id="d42ce-137">任务组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="d42ce-137">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="d42ce-138">id</span><span class="sxs-lookup"><span data-stu-id="d42ce-138">id</span></span>|<span data-ttu-id="d42ce-139">字符串</span><span class="sxs-lookup"><span data-stu-id="d42ce-139">String</span></span>|<span data-ttu-id="d42ce-140">任务组的唯一字符串标识符。</span><span class="sxs-lookup"><span data-stu-id="d42ce-140">The unique string identifier of the task group.</span></span> <span data-ttu-id="d42ce-141">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="d42ce-141">Read-only.</span></span>|
|<span data-ttu-id="d42ce-142">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="d42ce-142">isDefaultGroup</span></span>|<span data-ttu-id="d42ce-143">布尔</span><span class="sxs-lookup"><span data-stu-id="d42ce-143">Boolean</span></span>|<span data-ttu-id="d42ce-144">如果任务组的默认任务组，则为 true。</span><span class="sxs-lookup"><span data-stu-id="d42ce-144">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="d42ce-145">name</span><span class="sxs-lookup"><span data-stu-id="d42ce-145">name</span></span>|<span data-ttu-id="d42ce-146">字符串</span><span class="sxs-lookup"><span data-stu-id="d42ce-146">String</span></span>|<span data-ttu-id="d42ce-147">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="d42ce-147">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d42ce-148">Relationships</span><span class="sxs-lookup"><span data-stu-id="d42ce-148">Relationships</span></span>
| <span data-ttu-id="d42ce-149">关系</span><span class="sxs-lookup"><span data-stu-id="d42ce-149">Relationship</span></span> | <span data-ttu-id="d42ce-150">类型</span><span class="sxs-lookup"><span data-stu-id="d42ce-150">Type</span></span>   |<span data-ttu-id="d42ce-151">Description</span><span class="sxs-lookup"><span data-stu-id="d42ce-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d42ce-152">taskFolders</span><span class="sxs-lookup"><span data-stu-id="d42ce-152">taskFolders</span></span>|<span data-ttu-id="d42ce-153">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="d42ce-153">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="d42ce-154">在任务组中的任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="d42ce-154">The collection of task folders in the task group.</span></span> <span data-ttu-id="d42ce-155">只读。</span><span class="sxs-lookup"><span data-stu-id="d42ce-155">Read-only.</span></span> <span data-ttu-id="d42ce-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d42ce-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d42ce-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d42ce-157">JSON representation</span></span>
<span data-ttu-id="d42ce-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d42ce-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
