---
title: outlookTaskFolder 资源类型
description: '包含 Outlook 任务 （outlookTask 对象的集合） 的文件夹。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a117e14ea1cfe4b69cbbf69720a22a0094fb0b72
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575665"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="1e122-103">outlookTaskFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e122-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e122-104">包含 Outlook 任务 （ [outlookTask](outlooktask.md)对象的集合） 的文件夹。</span><span class="sxs-lookup"><span data-stu-id="1e122-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="1e122-105">在 Outlook 中，默认任务组中， `My Tasks`，包含默认任务文件夹， `Tasks`，用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="1e122-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="1e122-106">无法重命名或删除这些默认任务组和文件夹，但您可以创建其他任务组和任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="1e122-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="1e122-107">方法</span><span class="sxs-lookup"><span data-stu-id="1e122-107">Methods</span></span>

| <span data-ttu-id="1e122-108">方法</span><span class="sxs-lookup"><span data-stu-id="1e122-108">Method</span></span>           | <span data-ttu-id="1e122-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1e122-109">Return Type</span></span>    |<span data-ttu-id="1e122-110">说明</span><span class="sxs-lookup"><span data-stu-id="1e122-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e122-111">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="1e122-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="1e122-113">要获取的属性和指定 Outlook 任务文件夹的关系。</span><span class="sxs-lookup"><span data-stu-id="1e122-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="1e122-114">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="1e122-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="1e122-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="1e122-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="1e122-116">在指定的任务文件夹中创建 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="1e122-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="1e122-117">List tasks</span><span class="sxs-lookup"><span data-stu-id="1e122-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="1e122-118">[outlookTask](outlooktask.md)集合</span><span class="sxs-lookup"><span data-stu-id="1e122-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="1e122-119">在指定文件夹中获取所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="1e122-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="1e122-120">Update</span><span class="sxs-lookup"><span data-stu-id="1e122-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="1e122-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="1e122-122">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="1e122-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="1e122-123">Delete</span><span class="sxs-lookup"><span data-stu-id="1e122-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="1e122-124">无</span><span class="sxs-lookup"><span data-stu-id="1e122-124">None</span></span> |<span data-ttu-id="1e122-125">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="1e122-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="1e122-126">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="1e122-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="1e122-127">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="1e122-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="1e122-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="1e122-129">在新的或现有的 Outlook 任务文件夹中创建一个或多个单值扩展的属性。</span><span class="sxs-lookup"><span data-stu-id="1e122-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="1e122-130">使用单值扩展属性获取任务文件夹</span><span class="sxs-lookup"><span data-stu-id="1e122-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="1e122-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="1e122-132">获取包含一个单值使用扩展属性的 Outlook 任务文件夹`$expand`或`$filter`。</span><span class="sxs-lookup"><span data-stu-id="1e122-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="1e122-133">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="1e122-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="1e122-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="1e122-135">在新的或现有的 Outlook 任务文件夹中创建一个或多个多值扩展的属性。</span><span class="sxs-lookup"><span data-stu-id="1e122-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="1e122-136">多值扩展属性获取任务文件夹</span><span class="sxs-lookup"><span data-stu-id="1e122-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="1e122-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="1e122-138">获取包含多值扩展的属性，通过使用 Outlook 任务文件夹`$expand`。</span><span class="sxs-lookup"><span data-stu-id="1e122-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e122-139">属性</span><span class="sxs-lookup"><span data-stu-id="1e122-139">Properties</span></span>
| <span data-ttu-id="1e122-140">属性</span><span class="sxs-lookup"><span data-stu-id="1e122-140">Property</span></span>     | <span data-ttu-id="1e122-141">类型</span><span class="sxs-lookup"><span data-stu-id="1e122-141">Type</span></span>   |<span data-ttu-id="1e122-142">说明</span><span class="sxs-lookup"><span data-stu-id="1e122-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e122-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="1e122-143">changeKey</span></span>|<span data-ttu-id="1e122-144">String</span><span class="sxs-lookup"><span data-stu-id="1e122-144">String</span></span>|<span data-ttu-id="1e122-145">任务文件夹的版本。</span><span class="sxs-lookup"><span data-stu-id="1e122-145">The version of the task folder.</span></span>|
|<span data-ttu-id="1e122-146">id</span><span class="sxs-lookup"><span data-stu-id="1e122-146">id</span></span>|<span data-ttu-id="1e122-147">String</span><span class="sxs-lookup"><span data-stu-id="1e122-147">String</span></span>|<span data-ttu-id="1e122-148">任务文件夹中，用户的邮箱中的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1e122-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="1e122-149">只读。</span><span class="sxs-lookup"><span data-stu-id="1e122-149">Read-only.</span></span>|
|<span data-ttu-id="1e122-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="1e122-150">isDefaultFolder</span></span>|<span data-ttu-id="1e122-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="1e122-151">Boolean</span></span>|<span data-ttu-id="1e122-152">如果文件夹为默认的任务文件夹，则为 true。</span><span class="sxs-lookup"><span data-stu-id="1e122-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="1e122-153">name</span><span class="sxs-lookup"><span data-stu-id="1e122-153">name</span></span>|<span data-ttu-id="1e122-154">String</span><span class="sxs-lookup"><span data-stu-id="1e122-154">String</span></span>|<span data-ttu-id="1e122-155">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="1e122-155">The name of the task folder.</span></span>|
|<span data-ttu-id="1e122-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="1e122-156">parentGroupKey</span></span>|<span data-ttu-id="1e122-157">Guid</span><span class="sxs-lookup"><span data-stu-id="1e122-157">Guid</span></span>|<span data-ttu-id="1e122-158">任务文件夹的父组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="1e122-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e122-159">关系</span><span class="sxs-lookup"><span data-stu-id="1e122-159">Relationships</span></span>
| <span data-ttu-id="1e122-160">关系</span><span class="sxs-lookup"><span data-stu-id="1e122-160">Relationship</span></span> | <span data-ttu-id="1e122-161">类型</span><span class="sxs-lookup"><span data-stu-id="1e122-161">Type</span></span>   |<span data-ttu-id="1e122-162">说明</span><span class="sxs-lookup"><span data-stu-id="1e122-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e122-163">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1e122-163">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="1e122-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1e122-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="1e122-165">多值定义的任务文件夹的扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="1e122-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="1e122-166">只读。</span><span class="sxs-lookup"><span data-stu-id="1e122-166">Read-only.</span></span> <span data-ttu-id="1e122-167">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1e122-167">Nullable.</span></span>|
|<span data-ttu-id="1e122-168">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1e122-168">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="1e122-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="1e122-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="1e122-170">定义的任务文件夹的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="1e122-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="1e122-171">只读。</span><span class="sxs-lookup"><span data-stu-id="1e122-171">Read-only.</span></span> <span data-ttu-id="1e122-172">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1e122-172">Nullable.</span></span>|
|<span data-ttu-id="1e122-173">tasks</span><span class="sxs-lookup"><span data-stu-id="1e122-173">tasks</span></span>|<span data-ttu-id="1e122-174">[outlookTask](outlooktask.md)集合</span><span class="sxs-lookup"><span data-stu-id="1e122-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="1e122-175">此任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="1e122-175">The tasks in this task folder.</span></span> <span data-ttu-id="1e122-176">只读。</span><span class="sxs-lookup"><span data-stu-id="1e122-176">Read-only.</span></span> <span data-ttu-id="1e122-177">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1e122-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e122-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e122-178">JSON representation</span></span>
<span data-ttu-id="1e122-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e122-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
