---
title: outlookTaskFolder 资源类型
description: '包含 Outlook 任务的文件夹 () 的 outlookTask 对象的集合。 '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c9f9958750cca1aaa40ba9394832e5974bed8cc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998360"
---
# <a name="outlooktaskfolder-resource-type-deprecated"></a><span data-ttu-id="901f1-103">outlookTaskFolder 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="901f1-103">outlookTaskFolder resource type (deprecated)</span></span>

<span data-ttu-id="901f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="901f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="901f1-105">包含 Outlook 任务的文件夹 () 的 [outlookTask](outlooktask.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="901f1-105">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="901f1-106">在 Outlook 中，默认任务组， `My Tasks` 包含用户邮箱的默认任务文件夹 `Tasks` 。</span><span class="sxs-lookup"><span data-stu-id="901f1-106">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="901f1-107">您不能重命名或删除这些默认任务组和文件夹，但可以创建其他任务组和任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="901f1-107">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="901f1-108">方法</span><span class="sxs-lookup"><span data-stu-id="901f1-108">Methods</span></span>

| <span data-ttu-id="901f1-109">方法</span><span class="sxs-lookup"><span data-stu-id="901f1-109">Method</span></span>           | <span data-ttu-id="901f1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="901f1-110">Return Type</span></span>    |<span data-ttu-id="901f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="901f1-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="901f1-112">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-112">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="901f1-113">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-113">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="901f1-114">获取指定的 Outlook 任务文件夹的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="901f1-114">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="901f1-115">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="901f1-115">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="901f1-116">outlookTask</span><span class="sxs-lookup"><span data-stu-id="901f1-116">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="901f1-117">在指定的任务文件夹中创建一个 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="901f1-117">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="901f1-118">列出任务</span><span class="sxs-lookup"><span data-stu-id="901f1-118">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="901f1-119">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="901f1-119">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="901f1-120">获取指定文件夹中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="901f1-120">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="901f1-121">更新</span><span class="sxs-lookup"><span data-stu-id="901f1-121">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="901f1-122">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-122">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="901f1-123">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="901f1-123">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="901f1-124">删除</span><span class="sxs-lookup"><span data-stu-id="901f1-124">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="901f1-125">无</span><span class="sxs-lookup"><span data-stu-id="901f1-125">None</span></span> |<span data-ttu-id="901f1-126">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="901f1-126">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="901f1-127">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="901f1-127">**Extended properties**</span></span>| | |
|[<span data-ttu-id="901f1-128">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="901f1-128">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="901f1-129">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-129">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="901f1-130">在新的或现有的 Outlook 任务文件夹中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="901f1-130">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="901f1-131">获取具有单值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="901f1-131">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="901f1-132">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-132">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="901f1-133">通过使用或获取包含单值扩展属性的 Outlook 任务文件夹 `$expand` `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="901f1-133">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="901f1-134">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="901f1-134">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="901f1-135">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-135">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="901f1-136">在新的或现有的 Outlook 任务文件夹中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="901f1-136">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="901f1-137">获取具有多值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="901f1-137">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="901f1-138">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-138">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="901f1-139">使用获取包含多值扩展属性的 Outlook 任务文件夹 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="901f1-139">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="901f1-140">属性</span><span class="sxs-lookup"><span data-stu-id="901f1-140">Properties</span></span>
| <span data-ttu-id="901f1-141">属性</span><span class="sxs-lookup"><span data-stu-id="901f1-141">Property</span></span>     | <span data-ttu-id="901f1-142">类型</span><span class="sxs-lookup"><span data-stu-id="901f1-142">Type</span></span>   |<span data-ttu-id="901f1-143">说明</span><span class="sxs-lookup"><span data-stu-id="901f1-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="901f1-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="901f1-144">changeKey</span></span>|<span data-ttu-id="901f1-145">String</span><span class="sxs-lookup"><span data-stu-id="901f1-145">String</span></span>|<span data-ttu-id="901f1-146">任务文件夹的版本。</span><span class="sxs-lookup"><span data-stu-id="901f1-146">The version of the task folder.</span></span>|
|<span data-ttu-id="901f1-147">id</span><span class="sxs-lookup"><span data-stu-id="901f1-147">id</span></span>|<span data-ttu-id="901f1-148">String</span><span class="sxs-lookup"><span data-stu-id="901f1-148">String</span></span>|<span data-ttu-id="901f1-149">任务文件夹的标识符，在用户的邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="901f1-149">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="901f1-150">只读。</span><span class="sxs-lookup"><span data-stu-id="901f1-150">Read-only.</span></span>|
|<span data-ttu-id="901f1-151">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="901f1-151">isDefaultFolder</span></span>|<span data-ttu-id="901f1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="901f1-152">Boolean</span></span>|<span data-ttu-id="901f1-153">如此如果该文件夹是默认的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="901f1-153">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="901f1-154">name</span><span class="sxs-lookup"><span data-stu-id="901f1-154">name</span></span>|<span data-ttu-id="901f1-155">String</span><span class="sxs-lookup"><span data-stu-id="901f1-155">String</span></span>|<span data-ttu-id="901f1-156">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="901f1-156">The name of the task folder.</span></span>|
|<span data-ttu-id="901f1-157">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="901f1-157">parentGroupKey</span></span>|<span data-ttu-id="901f1-158">Guid</span><span class="sxs-lookup"><span data-stu-id="901f1-158">Guid</span></span>|<span data-ttu-id="901f1-159">任务文件夹的父组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="901f1-159">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="901f1-160">关系</span><span class="sxs-lookup"><span data-stu-id="901f1-160">Relationships</span></span>
| <span data-ttu-id="901f1-161">关系</span><span class="sxs-lookup"><span data-stu-id="901f1-161">Relationship</span></span> | <span data-ttu-id="901f1-162">类型</span><span class="sxs-lookup"><span data-stu-id="901f1-162">Type</span></span>   |<span data-ttu-id="901f1-163">说明</span><span class="sxs-lookup"><span data-stu-id="901f1-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="901f1-164">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="901f1-164">multiValueExtendedProperties</span></span>|<span data-ttu-id="901f1-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="901f1-165">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="901f1-166">为任务文件夹定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="901f1-166">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="901f1-167">只读。</span><span class="sxs-lookup"><span data-stu-id="901f1-167">Read-only.</span></span> <span data-ttu-id="901f1-168">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="901f1-168">Nullable.</span></span>|
|<span data-ttu-id="901f1-169">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="901f1-169">singleValueExtendedProperties</span></span>|<span data-ttu-id="901f1-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="901f1-170">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="901f1-171">为任务文件夹定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="901f1-171">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="901f1-172">只读。</span><span class="sxs-lookup"><span data-stu-id="901f1-172">Read-only.</span></span> <span data-ttu-id="901f1-173">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="901f1-173">Nullable.</span></span>|
|<span data-ttu-id="901f1-174">任务</span><span class="sxs-lookup"><span data-stu-id="901f1-174">tasks</span></span>|<span data-ttu-id="901f1-175">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="901f1-175">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="901f1-176">此任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="901f1-176">The tasks in this task folder.</span></span> <span data-ttu-id="901f1-177">只读。</span><span class="sxs-lookup"><span data-stu-id="901f1-177">Read-only.</span></span> <span data-ttu-id="901f1-178">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="901f1-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="901f1-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="901f1-179">JSON representation</span></span>
<span data-ttu-id="901f1-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="901f1-180">Here is a JSON representation of the resource.</span></span>

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


