---
title: outlookTaskFolder 资源类型
description: '包含 outlookTask 对象和 (中的 Outlook 任务) 。 '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f950028bef8bcdcdcd8252ca16348c235ef31d3f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849785"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="9ec50-103">outlookTaskFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ec50-103">outlookTaskFolder resource type</span></span>

<span data-ttu-id="9ec50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ec50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="9ec50-105">包含 OutlookTask 对象集合的[ (Outlook 任务) 。](outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="9ec50-105">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="9ec50-106">在 Outlook 中，默认任务 `My Tasks` 组包含用户邮箱 `Tasks` 的默认任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="9ec50-106">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="9ec50-107">不能重命名或删除这些默认任务组和文件夹，但可以创建其他任务组和任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="9ec50-107">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="9ec50-108">方法</span><span class="sxs-lookup"><span data-stu-id="9ec50-108">Methods</span></span>

| <span data-ttu-id="9ec50-109">方法</span><span class="sxs-lookup"><span data-stu-id="9ec50-109">Method</span></span>           | <span data-ttu-id="9ec50-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ec50-110">Return Type</span></span>    |<span data-ttu-id="9ec50-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ec50-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ec50-112">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-112">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="9ec50-113">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-113">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="9ec50-114">获取指定的 Outlook 任务文件夹的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ec50-114">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="9ec50-115">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="9ec50-115">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="9ec50-116">outlookTask</span><span class="sxs-lookup"><span data-stu-id="9ec50-116">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="9ec50-117">在指定的任务文件夹中创建 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="9ec50-117">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="9ec50-118">列出任务</span><span class="sxs-lookup"><span data-stu-id="9ec50-118">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="9ec50-119">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ec50-119">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="9ec50-120">获取指定文件夹中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="9ec50-120">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="9ec50-121">更新</span><span class="sxs-lookup"><span data-stu-id="9ec50-121">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="9ec50-122">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-122">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="9ec50-123">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="9ec50-123">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="9ec50-124">删除</span><span class="sxs-lookup"><span data-stu-id="9ec50-124">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="9ec50-125">无</span><span class="sxs-lookup"><span data-stu-id="9ec50-125">None</span></span> |<span data-ttu-id="9ec50-126">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="9ec50-126">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="9ec50-127">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="9ec50-127">**Extended properties**</span></span>| | |
|[<span data-ttu-id="9ec50-128">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="9ec50-128">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="9ec50-129">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-129">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="9ec50-130">在新建或现有的 Outlook 任务文件夹中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="9ec50-130">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="9ec50-131">获取包含单值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="9ec50-131">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9ec50-132">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-132">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="9ec50-133">通过使用或获取包含单值扩展属性的 Outlook 任务 `$expand` 文件夹 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="9ec50-133">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="9ec50-134">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="9ec50-134">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="9ec50-135">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-135">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="9ec50-136">在新建或现有的 Outlook 任务文件夹中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="9ec50-136">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="9ec50-137">获取具有多值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="9ec50-137">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9ec50-138">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-138">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="9ec50-139">使用获取包含一个多值扩展属性的 Outlook 任务文件夹 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="9ec50-139">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ec50-140">属性</span><span class="sxs-lookup"><span data-stu-id="9ec50-140">Properties</span></span>
| <span data-ttu-id="9ec50-141">属性</span><span class="sxs-lookup"><span data-stu-id="9ec50-141">Property</span></span>     | <span data-ttu-id="9ec50-142">类型</span><span class="sxs-lookup"><span data-stu-id="9ec50-142">Type</span></span>   |<span data-ttu-id="9ec50-143">说明</span><span class="sxs-lookup"><span data-stu-id="9ec50-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ec50-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="9ec50-144">changeKey</span></span>|<span data-ttu-id="9ec50-145">String</span><span class="sxs-lookup"><span data-stu-id="9ec50-145">String</span></span>|<span data-ttu-id="9ec50-146">任务文件夹的版本。</span><span class="sxs-lookup"><span data-stu-id="9ec50-146">The version of the task folder.</span></span>|
|<span data-ttu-id="9ec50-147">id</span><span class="sxs-lookup"><span data-stu-id="9ec50-147">id</span></span>|<span data-ttu-id="9ec50-148">String</span><span class="sxs-lookup"><span data-stu-id="9ec50-148">String</span></span>|<span data-ttu-id="9ec50-149">任务文件夹的标识符，在用户邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="9ec50-149">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="9ec50-150">只读。</span><span class="sxs-lookup"><span data-stu-id="9ec50-150">Read-only.</span></span>|
|<span data-ttu-id="9ec50-151">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="9ec50-151">isDefaultFolder</span></span>|<span data-ttu-id="9ec50-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec50-152">Boolean</span></span>|<span data-ttu-id="9ec50-153">如此 如果该文件夹是默认任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="9ec50-153">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="9ec50-154">name</span><span class="sxs-lookup"><span data-stu-id="9ec50-154">name</span></span>|<span data-ttu-id="9ec50-155">String</span><span class="sxs-lookup"><span data-stu-id="9ec50-155">String</span></span>|<span data-ttu-id="9ec50-156">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="9ec50-156">The name of the task folder.</span></span>|
|<span data-ttu-id="9ec50-157">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="9ec50-157">parentGroupKey</span></span>|<span data-ttu-id="9ec50-158">Guid</span><span class="sxs-lookup"><span data-stu-id="9ec50-158">Guid</span></span>|<span data-ttu-id="9ec50-159">任务文件夹父级组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="9ec50-159">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ec50-160">关系</span><span class="sxs-lookup"><span data-stu-id="9ec50-160">Relationships</span></span>
| <span data-ttu-id="9ec50-161">关系</span><span class="sxs-lookup"><span data-stu-id="9ec50-161">Relationship</span></span> | <span data-ttu-id="9ec50-162">类型</span><span class="sxs-lookup"><span data-stu-id="9ec50-162">Type</span></span>   |<span data-ttu-id="9ec50-163">说明</span><span class="sxs-lookup"><span data-stu-id="9ec50-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ec50-164">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9ec50-164">multiValueExtendedProperties</span></span>|<span data-ttu-id="9ec50-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ec50-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="9ec50-166">为任务文件夹定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="9ec50-166">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="9ec50-167">只读。</span><span class="sxs-lookup"><span data-stu-id="9ec50-167">Read-only.</span></span> <span data-ttu-id="9ec50-168">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9ec50-168">Nullable.</span></span>|
|<span data-ttu-id="9ec50-169">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9ec50-169">singleValueExtendedProperties</span></span>|<span data-ttu-id="9ec50-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="9ec50-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="9ec50-171">为任务文件夹定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="9ec50-171">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="9ec50-172">只读。</span><span class="sxs-lookup"><span data-stu-id="9ec50-172">Read-only.</span></span> <span data-ttu-id="9ec50-173">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9ec50-173">Nullable.</span></span>|
|<span data-ttu-id="9ec50-174">任务</span><span class="sxs-lookup"><span data-stu-id="9ec50-174">tasks</span></span>|<span data-ttu-id="9ec50-175">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ec50-175">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="9ec50-176">此任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="9ec50-176">The tasks in this task folder.</span></span> <span data-ttu-id="9ec50-177">只读。</span><span class="sxs-lookup"><span data-stu-id="9ec50-177">Read-only.</span></span> <span data-ttu-id="9ec50-178">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9ec50-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ec50-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ec50-179">JSON representation</span></span>
<span data-ttu-id="9ec50-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ec50-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->
