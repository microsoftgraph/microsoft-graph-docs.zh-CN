---
title: outlookTaskGroup 资源类型
description: '包含 Outlook 任务 （outlookTask 对象的集合） 的文件夹 (outlookTaskFolder) 组。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524616"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="9007f-103">outlookTaskGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="9007f-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9007f-104">包含 Outlook 任务 （ [outlookTask](outlooktask.md)对象的集合） 的文件夹 ([outlookTaskFolder](outlooktaskfolder.md)) 组。</span><span class="sxs-lookup"><span data-stu-id="9007f-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="9007f-105">在 Outlook 中，没有默认任务组`My Tasks`无法重命名或删除。</span><span class="sxs-lookup"><span data-stu-id="9007f-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="9007f-106">但是，您可以创建其他任务组。</span><span class="sxs-lookup"><span data-stu-id="9007f-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="9007f-107">方法</span><span class="sxs-lookup"><span data-stu-id="9007f-107">Methods</span></span>

| <span data-ttu-id="9007f-108">方法</span><span class="sxs-lookup"><span data-stu-id="9007f-108">Method</span></span>           | <span data-ttu-id="9007f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9007f-109">Return Type</span></span>    |<span data-ttu-id="9007f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9007f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9007f-111">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9007f-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="9007f-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9007f-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="9007f-113">要获取的属性和指定 Outlook 任务组的关系。</span><span class="sxs-lookup"><span data-stu-id="9007f-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="9007f-114">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9007f-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="9007f-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9007f-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="9007f-116">创建 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="9007f-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="9007f-117">列表 taskFolders</span><span class="sxs-lookup"><span data-stu-id="9007f-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="9007f-118">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="9007f-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="9007f-119">获取 Outlook 任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="9007f-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="9007f-120">Update</span><span class="sxs-lookup"><span data-stu-id="9007f-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="9007f-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9007f-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="9007f-122">更新 Outlook 任务组的可写属性。</span><span class="sxs-lookup"><span data-stu-id="9007f-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="9007f-123">删除</span><span class="sxs-lookup"><span data-stu-id="9007f-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="9007f-124">无</span><span class="sxs-lookup"><span data-stu-id="9007f-124">None</span></span> |<span data-ttu-id="9007f-125">删除指定的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="9007f-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="9007f-126">属性</span><span class="sxs-lookup"><span data-stu-id="9007f-126">Properties</span></span>
| <span data-ttu-id="9007f-127">属性</span><span class="sxs-lookup"><span data-stu-id="9007f-127">Property</span></span>     | <span data-ttu-id="9007f-128">类型</span><span class="sxs-lookup"><span data-stu-id="9007f-128">Type</span></span>   |<span data-ttu-id="9007f-129">说明</span><span class="sxs-lookup"><span data-stu-id="9007f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9007f-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="9007f-130">changeKey</span></span>|<span data-ttu-id="9007f-131">String</span><span class="sxs-lookup"><span data-stu-id="9007f-131">String</span></span>|<span data-ttu-id="9007f-132">任务组的版本。</span><span class="sxs-lookup"><span data-stu-id="9007f-132">The version of the task group.</span></span>|
|<span data-ttu-id="9007f-133">groupKey</span><span class="sxs-lookup"><span data-stu-id="9007f-133">groupKey</span></span>|<span data-ttu-id="9007f-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="9007f-134">Edm.Guid</span></span>|<span data-ttu-id="9007f-135">任务组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="9007f-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="9007f-136">id</span><span class="sxs-lookup"><span data-stu-id="9007f-136">id</span></span>|<span data-ttu-id="9007f-137">字串符号</span><span class="sxs-lookup"><span data-stu-id="9007f-137">String</span></span>|<span data-ttu-id="9007f-138">任务组的唯一字符串标识符。</span><span class="sxs-lookup"><span data-stu-id="9007f-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="9007f-139">只读。</span><span class="sxs-lookup"><span data-stu-id="9007f-139">Read-only.</span></span>|
|<span data-ttu-id="9007f-140">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="9007f-140">isDefaultGroup</span></span>|<span data-ttu-id="9007f-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="9007f-141">Boolean</span></span>|<span data-ttu-id="9007f-142">如果任务组的默认任务组，则为 true。</span><span class="sxs-lookup"><span data-stu-id="9007f-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="9007f-143">name</span><span class="sxs-lookup"><span data-stu-id="9007f-143">name</span></span>|<span data-ttu-id="9007f-144">String</span><span class="sxs-lookup"><span data-stu-id="9007f-144">String</span></span>|<span data-ttu-id="9007f-145">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="9007f-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9007f-146">关系</span><span class="sxs-lookup"><span data-stu-id="9007f-146">Relationships</span></span>
| <span data-ttu-id="9007f-147">关系</span><span class="sxs-lookup"><span data-stu-id="9007f-147">Relationship</span></span> | <span data-ttu-id="9007f-148">类型</span><span class="sxs-lookup"><span data-stu-id="9007f-148">Type</span></span>   |<span data-ttu-id="9007f-149">说明</span><span class="sxs-lookup"><span data-stu-id="9007f-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9007f-150">taskFolders</span><span class="sxs-lookup"><span data-stu-id="9007f-150">taskFolders</span></span>|<span data-ttu-id="9007f-151">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="9007f-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="9007f-152">在任务组中的任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="9007f-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="9007f-153">只读。</span><span class="sxs-lookup"><span data-stu-id="9007f-153">Read-only.</span></span> <span data-ttu-id="9007f-154">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9007f-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9007f-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9007f-155">JSON representation</span></span>
<span data-ttu-id="9007f-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9007f-156">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
