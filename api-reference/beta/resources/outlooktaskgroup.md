---
title: outlookTaskGroup 资源类型
description: '一组文件夹 (outlookTaskFolder), 其中包含 Outlook 任务 (outlookTask 对象的集合)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 486261d80b8faad7a5969f8f1ce198479e39583c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568571"
---
# <a name="outlooktaskgroup-resource-type"></a><span data-ttu-id="afbf9-103">outlookTaskGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="afbf9-103">outlookTaskGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afbf9-104">一组文件夹 ([outlookTaskFolder](outlooktaskfolder.md)), 其中包含 Outlook 任务 ( [outlookTask](outlooktask.md)对象的集合)。</span><span class="sxs-lookup"><span data-stu-id="afbf9-104">A group of folders ([outlookTaskFolder](outlooktaskfolder.md)) that contain Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="afbf9-105">在 Outlook 中, 有一个不能重`My Tasks`命名或删除的默认任务组。</span><span class="sxs-lookup"><span data-stu-id="afbf9-105">In Outlook, there is a default task group `My Tasks` which you cannot rename or delete.</span></span> <span data-ttu-id="afbf9-106">不过, 您可以创建其他任务组。</span><span class="sxs-lookup"><span data-stu-id="afbf9-106">You can, however, create additional task groups.</span></span> 


## <a name="methods"></a><span data-ttu-id="afbf9-107">方法</span><span class="sxs-lookup"><span data-stu-id="afbf9-107">Methods</span></span>

| <span data-ttu-id="afbf9-108">方法</span><span class="sxs-lookup"><span data-stu-id="afbf9-108">Method</span></span>           | <span data-ttu-id="afbf9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="afbf9-109">Return Type</span></span>    |<span data-ttu-id="afbf9-110">说明</span><span class="sxs-lookup"><span data-stu-id="afbf9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="afbf9-111">获取 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="afbf9-111">Get outlookTaskGroup</span></span>](../api/outlooktaskgroup-get.md) | [<span data-ttu-id="afbf9-112">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="afbf9-112">outlookTaskGroup</span></span>](outlooktaskgroup.md) |<span data-ttu-id="afbf9-113">获取指定的 Outlook 任务组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="afbf9-113">Get the properties and relationships of the specified Outlook task group.</span></span>|
|[<span data-ttu-id="afbf9-114">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="afbf9-114">Create outlookTaskFolder</span></span>](../api/outlooktaskgroup-post-taskfolders.md) |[<span data-ttu-id="afbf9-115">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="afbf9-115">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="afbf9-116">创建一个 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="afbf9-116">Create an Outlook task folder.</span></span>|
|[<span data-ttu-id="afbf9-117">列出 taskFolders</span><span class="sxs-lookup"><span data-stu-id="afbf9-117">List taskFolders</span></span>](../api/outlooktaskgroup-list-taskfolders.md) |<span data-ttu-id="afbf9-118">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="afbf9-118">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="afbf9-119">获取 Outlook 任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="afbf9-119">Get a collection of Outlook task folders.</span></span>|
|[<span data-ttu-id="afbf9-120">更新</span><span class="sxs-lookup"><span data-stu-id="afbf9-120">Update</span></span>](../api/outlooktaskgroup-update.md) | [<span data-ttu-id="afbf9-121">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="afbf9-121">outlookTaskGroup</span></span>](outlooktaskgroup.md)  |<span data-ttu-id="afbf9-122">更新 Outlook 任务组的可写属性。</span><span class="sxs-lookup"><span data-stu-id="afbf9-122">Update the writable properties of an Outlook task group.</span></span> |
|[<span data-ttu-id="afbf9-123">删除</span><span class="sxs-lookup"><span data-stu-id="afbf9-123">Delete</span></span>](../api/outlooktaskgroup-delete.md) | <span data-ttu-id="afbf9-124">无</span><span class="sxs-lookup"><span data-stu-id="afbf9-124">None</span></span> |<span data-ttu-id="afbf9-125">删除指定的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="afbf9-125">Delete the specified Outlook task group.</span></span> |

## <a name="properties"></a><span data-ttu-id="afbf9-126">属性</span><span class="sxs-lookup"><span data-stu-id="afbf9-126">Properties</span></span>
| <span data-ttu-id="afbf9-127">属性</span><span class="sxs-lookup"><span data-stu-id="afbf9-127">Property</span></span>     | <span data-ttu-id="afbf9-128">类型</span><span class="sxs-lookup"><span data-stu-id="afbf9-128">Type</span></span>   |<span data-ttu-id="afbf9-129">说明</span><span class="sxs-lookup"><span data-stu-id="afbf9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afbf9-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="afbf9-130">changeKey</span></span>|<span data-ttu-id="afbf9-131">String</span><span class="sxs-lookup"><span data-stu-id="afbf9-131">String</span></span>|<span data-ttu-id="afbf9-132">任务组的版本。</span><span class="sxs-lookup"><span data-stu-id="afbf9-132">The version of the task group.</span></span>|
|<span data-ttu-id="afbf9-133">groupKey</span><span class="sxs-lookup"><span data-stu-id="afbf9-133">groupKey</span></span>|<span data-ttu-id="afbf9-134">Edm.Guid</span><span class="sxs-lookup"><span data-stu-id="afbf9-134">Edm.Guid</span></span>|<span data-ttu-id="afbf9-135">任务组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="afbf9-135">The unique GUID identifier for the task group.</span></span>|
|<span data-ttu-id="afbf9-136">id</span><span class="sxs-lookup"><span data-stu-id="afbf9-136">id</span></span>|<span data-ttu-id="afbf9-137">字符串</span><span class="sxs-lookup"><span data-stu-id="afbf9-137">String</span></span>|<span data-ttu-id="afbf9-138">任务组的唯一字符串标识符。</span><span class="sxs-lookup"><span data-stu-id="afbf9-138">The unique string identifier of the task group.</span></span> <span data-ttu-id="afbf9-139">只读。</span><span class="sxs-lookup"><span data-stu-id="afbf9-139">Read-only.</span></span>|
|<span data-ttu-id="afbf9-140">isDefaultGroup</span><span class="sxs-lookup"><span data-stu-id="afbf9-140">isDefaultGroup</span></span>|<span data-ttu-id="afbf9-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="afbf9-141">Boolean</span></span>|<span data-ttu-id="afbf9-142">如此如果任务组是默认任务组。</span><span class="sxs-lookup"><span data-stu-id="afbf9-142">True if the task group is the default task group.</span></span>|
|<span data-ttu-id="afbf9-143">name</span><span class="sxs-lookup"><span data-stu-id="afbf9-143">name</span></span>|<span data-ttu-id="afbf9-144">String</span><span class="sxs-lookup"><span data-stu-id="afbf9-144">String</span></span>|<span data-ttu-id="afbf9-145">任务组的名称。</span><span class="sxs-lookup"><span data-stu-id="afbf9-145">The name of the task group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afbf9-146">关系</span><span class="sxs-lookup"><span data-stu-id="afbf9-146">Relationships</span></span>
| <span data-ttu-id="afbf9-147">关系</span><span class="sxs-lookup"><span data-stu-id="afbf9-147">Relationship</span></span> | <span data-ttu-id="afbf9-148">类型</span><span class="sxs-lookup"><span data-stu-id="afbf9-148">Type</span></span>   |<span data-ttu-id="afbf9-149">说明</span><span class="sxs-lookup"><span data-stu-id="afbf9-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afbf9-150">taskFolders</span><span class="sxs-lookup"><span data-stu-id="afbf9-150">taskFolders</span></span>|<span data-ttu-id="afbf9-151">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="afbf9-151">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="afbf9-152">任务组中的任务文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="afbf9-152">The collection of task folders in the task group.</span></span> <span data-ttu-id="afbf9-153">只读。</span><span class="sxs-lookup"><span data-stu-id="afbf9-153">Read-only.</span></span> <span data-ttu-id="afbf9-154">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="afbf9-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="afbf9-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afbf9-155">JSON representation</span></span>
<span data-ttu-id="afbf9-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afbf9-156">Here is a JSON representation of the resource.</span></span>

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
