---
title: outlookTaskFolder 资源类型
description: '包含 Outlook 任务的文件夹 (outlookTask 对象的集合)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568574"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="a6b08-103">outlookTaskFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6b08-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6b08-104">包含 Outlook 任务的文件夹 ( [outlookTask](outlooktask.md)对象的集合)。</span><span class="sxs-lookup"><span data-stu-id="a6b08-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="a6b08-105">在 Outlook 中, 默认任务组`My Tasks`, 包含用户邮箱的默认任务文件夹`Tasks`。</span><span class="sxs-lookup"><span data-stu-id="a6b08-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="a6b08-106">您不能重命名或删除这些默认任务组和文件夹, 但可以创建其他任务组和任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="a6b08-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="a6b08-107">方法</span><span class="sxs-lookup"><span data-stu-id="a6b08-107">Methods</span></span>

| <span data-ttu-id="a6b08-108">方法</span><span class="sxs-lookup"><span data-stu-id="a6b08-108">Method</span></span>           | <span data-ttu-id="a6b08-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6b08-109">Return Type</span></span>    |<span data-ttu-id="a6b08-110">说明</span><span class="sxs-lookup"><span data-stu-id="a6b08-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6b08-111">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="a6b08-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="a6b08-113">获取指定的 Outlook 任务文件夹的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6b08-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="a6b08-114">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="a6b08-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="a6b08-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="a6b08-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="a6b08-116">在指定的任务文件夹中创建一个 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="a6b08-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="a6b08-117">列出任务</span><span class="sxs-lookup"><span data-stu-id="a6b08-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="a6b08-118">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6b08-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="a6b08-119">获取指定文件夹中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="a6b08-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="a6b08-120">更新</span><span class="sxs-lookup"><span data-stu-id="a6b08-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="a6b08-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="a6b08-122">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="a6b08-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="a6b08-123">删除</span><span class="sxs-lookup"><span data-stu-id="a6b08-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="a6b08-124">无</span><span class="sxs-lookup"><span data-stu-id="a6b08-124">None</span></span> |<span data-ttu-id="a6b08-125">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="a6b08-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="a6b08-126">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="a6b08-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="a6b08-127">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="a6b08-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="a6b08-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="a6b08-129">在新的或现有的 Outlook 任务文件夹中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="a6b08-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="a6b08-130">获取具有单值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="a6b08-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a6b08-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="a6b08-132">通过使用`$expand`或`$filter`获取包含单值扩展属性的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="a6b08-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="a6b08-133">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="a6b08-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="a6b08-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="a6b08-135">在新的或现有的 Outlook 任务文件夹中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="a6b08-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="a6b08-136">获取具有多值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="a6b08-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a6b08-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="a6b08-138">使用`$expand`获取包含多值扩展属性的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="a6b08-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="a6b08-139">属性</span><span class="sxs-lookup"><span data-stu-id="a6b08-139">Properties</span></span>
| <span data-ttu-id="a6b08-140">属性</span><span class="sxs-lookup"><span data-stu-id="a6b08-140">Property</span></span>     | <span data-ttu-id="a6b08-141">类型</span><span class="sxs-lookup"><span data-stu-id="a6b08-141">Type</span></span>   |<span data-ttu-id="a6b08-142">说明</span><span class="sxs-lookup"><span data-stu-id="a6b08-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6b08-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="a6b08-143">changeKey</span></span>|<span data-ttu-id="a6b08-144">String</span><span class="sxs-lookup"><span data-stu-id="a6b08-144">String</span></span>|<span data-ttu-id="a6b08-145">任务文件夹的版本。</span><span class="sxs-lookup"><span data-stu-id="a6b08-145">The version of the task folder.</span></span>|
|<span data-ttu-id="a6b08-146">id</span><span class="sxs-lookup"><span data-stu-id="a6b08-146">id</span></span>|<span data-ttu-id="a6b08-147">字符串</span><span class="sxs-lookup"><span data-stu-id="a6b08-147">String</span></span>|<span data-ttu-id="a6b08-148">任务文件夹的标识符, 在用户的邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="a6b08-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="a6b08-149">只读。</span><span class="sxs-lookup"><span data-stu-id="a6b08-149">Read-only.</span></span>|
|<span data-ttu-id="a6b08-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="a6b08-150">isDefaultFolder</span></span>|<span data-ttu-id="a6b08-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6b08-151">Boolean</span></span>|<span data-ttu-id="a6b08-152">如此如果该文件夹是默认的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="a6b08-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="a6b08-153">name</span><span class="sxs-lookup"><span data-stu-id="a6b08-153">name</span></span>|<span data-ttu-id="a6b08-154">String</span><span class="sxs-lookup"><span data-stu-id="a6b08-154">String</span></span>|<span data-ttu-id="a6b08-155">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="a6b08-155">The name of the task folder.</span></span>|
|<span data-ttu-id="a6b08-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="a6b08-156">parentGroupKey</span></span>|<span data-ttu-id="a6b08-157">Guid</span><span class="sxs-lookup"><span data-stu-id="a6b08-157">Guid</span></span>|<span data-ttu-id="a6b08-158">任务文件夹的父组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b08-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6b08-159">关系</span><span class="sxs-lookup"><span data-stu-id="a6b08-159">Relationships</span></span>
| <span data-ttu-id="a6b08-160">关系</span><span class="sxs-lookup"><span data-stu-id="a6b08-160">Relationship</span></span> | <span data-ttu-id="a6b08-161">类型</span><span class="sxs-lookup"><span data-stu-id="a6b08-161">Type</span></span>   |<span data-ttu-id="a6b08-162">说明</span><span class="sxs-lookup"><span data-stu-id="a6b08-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6b08-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a6b08-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="a6b08-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6b08-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="a6b08-165">为任务文件夹定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="a6b08-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="a6b08-166">只读。</span><span class="sxs-lookup"><span data-stu-id="a6b08-166">Read-only.</span></span> <span data-ttu-id="a6b08-167">可为空。</span><span class="sxs-lookup"><span data-stu-id="a6b08-167">Nullable.</span></span>|
|<span data-ttu-id="a6b08-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a6b08-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="a6b08-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="a6b08-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="a6b08-170">为任务文件夹定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="a6b08-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="a6b08-171">只读。</span><span class="sxs-lookup"><span data-stu-id="a6b08-171">Read-only.</span></span> <span data-ttu-id="a6b08-172">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a6b08-172">Nullable.</span></span>|
|<span data-ttu-id="a6b08-173">任务</span><span class="sxs-lookup"><span data-stu-id="a6b08-173">tasks</span></span>|<span data-ttu-id="a6b08-174">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6b08-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="a6b08-175">此任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="a6b08-175">The tasks in this task folder.</span></span> <span data-ttu-id="a6b08-176">只读。</span><span class="sxs-lookup"><span data-stu-id="a6b08-176">Read-only.</span></span> <span data-ttu-id="a6b08-177">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a6b08-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6b08-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6b08-178">JSON representation</span></span>
<span data-ttu-id="a6b08-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6b08-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
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
