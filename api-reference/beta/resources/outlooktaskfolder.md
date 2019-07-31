---
title: outlookTaskFolder 资源类型
description: '包含 Outlook 任务的文件夹 (outlookTask 对象的集合)。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 631da782e47325a2ff28eb6ae9eb1447e1b0a14d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009256"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="b792f-103">outlookTaskFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="b792f-103">outlookTaskFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b792f-104">包含 Outlook 任务的文件夹 ( [outlookTask](outlooktask.md)对象的集合)。</span><span class="sxs-lookup"><span data-stu-id="b792f-104">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="b792f-105">在 Outlook 中, 默认任务组`My Tasks`, 包含用户邮箱的默认任务文件夹`Tasks`。</span><span class="sxs-lookup"><span data-stu-id="b792f-105">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="b792f-106">您不能重命名或删除这些默认任务组和文件夹, 但可以创建其他任务组和任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="b792f-106">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="b792f-107">方法</span><span class="sxs-lookup"><span data-stu-id="b792f-107">Methods</span></span>

| <span data-ttu-id="b792f-108">方法</span><span class="sxs-lookup"><span data-stu-id="b792f-108">Method</span></span>           | <span data-ttu-id="b792f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b792f-109">Return Type</span></span>    |<span data-ttu-id="b792f-110">说明</span><span class="sxs-lookup"><span data-stu-id="b792f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b792f-111">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-111">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="b792f-112">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-112">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="b792f-113">获取指定的 Outlook 任务文件夹的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b792f-113">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="b792f-114">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="b792f-114">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="b792f-115">outlookTask</span><span class="sxs-lookup"><span data-stu-id="b792f-115">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="b792f-116">在指定的任务文件夹中创建一个 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="b792f-116">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="b792f-117">List tasks</span><span class="sxs-lookup"><span data-stu-id="b792f-117">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="b792f-118">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b792f-118">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="b792f-119">获取指定文件夹中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="b792f-119">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="b792f-120">更新</span><span class="sxs-lookup"><span data-stu-id="b792f-120">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="b792f-121">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-121">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="b792f-122">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="b792f-122">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="b792f-123">删除</span><span class="sxs-lookup"><span data-stu-id="b792f-123">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="b792f-124">无</span><span class="sxs-lookup"><span data-stu-id="b792f-124">None</span></span> |<span data-ttu-id="b792f-125">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="b792f-125">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="b792f-126">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="b792f-126">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b792f-127">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b792f-127">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="b792f-128">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-128">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="b792f-129">在新的或现有的 Outlook 任务文件夹中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b792f-129">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="b792f-130">获取具有单值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="b792f-130">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b792f-131">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-131">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b792f-132">通过使用`$expand`或`$filter`获取包含单值扩展属性的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="b792f-132">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b792f-133">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b792f-133">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="b792f-134">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-134">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b792f-135">在新的或现有的 Outlook 任务文件夹中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b792f-135">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="b792f-136">获取具有多值扩展属性的任务文件夹</span><span class="sxs-lookup"><span data-stu-id="b792f-136">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b792f-137">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-137">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="b792f-138">使用`$expand`获取包含多值扩展属性的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="b792f-138">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b792f-139">属性</span><span class="sxs-lookup"><span data-stu-id="b792f-139">Properties</span></span>
| <span data-ttu-id="b792f-140">属性</span><span class="sxs-lookup"><span data-stu-id="b792f-140">Property</span></span>     | <span data-ttu-id="b792f-141">类型</span><span class="sxs-lookup"><span data-stu-id="b792f-141">Type</span></span>   |<span data-ttu-id="b792f-142">说明</span><span class="sxs-lookup"><span data-stu-id="b792f-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b792f-143">changeKey</span><span class="sxs-lookup"><span data-stu-id="b792f-143">changeKey</span></span>|<span data-ttu-id="b792f-144">String</span><span class="sxs-lookup"><span data-stu-id="b792f-144">String</span></span>|<span data-ttu-id="b792f-145">任务文件夹的版本。</span><span class="sxs-lookup"><span data-stu-id="b792f-145">The version of the task folder.</span></span>|
|<span data-ttu-id="b792f-146">id</span><span class="sxs-lookup"><span data-stu-id="b792f-146">id</span></span>|<span data-ttu-id="b792f-147">String</span><span class="sxs-lookup"><span data-stu-id="b792f-147">String</span></span>|<span data-ttu-id="b792f-148">任务文件夹的标识符, 在用户的邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="b792f-148">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="b792f-149">只读。</span><span class="sxs-lookup"><span data-stu-id="b792f-149">Read-only.</span></span>|
|<span data-ttu-id="b792f-150">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="b792f-150">isDefaultFolder</span></span>|<span data-ttu-id="b792f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b792f-151">Boolean</span></span>|<span data-ttu-id="b792f-152">如此如果该文件夹是默认的任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="b792f-152">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="b792f-153">name</span><span class="sxs-lookup"><span data-stu-id="b792f-153">name</span></span>|<span data-ttu-id="b792f-154">字符串</span><span class="sxs-lookup"><span data-stu-id="b792f-154">String</span></span>|<span data-ttu-id="b792f-155">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="b792f-155">The name of the task folder.</span></span>|
|<span data-ttu-id="b792f-156">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="b792f-156">parentGroupKey</span></span>|<span data-ttu-id="b792f-157">Guid</span><span class="sxs-lookup"><span data-stu-id="b792f-157">Guid</span></span>|<span data-ttu-id="b792f-158">任务文件夹的父组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="b792f-158">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b792f-159">关系</span><span class="sxs-lookup"><span data-stu-id="b792f-159">Relationships</span></span>
| <span data-ttu-id="b792f-160">关系</span><span class="sxs-lookup"><span data-stu-id="b792f-160">Relationship</span></span> | <span data-ttu-id="b792f-161">类型</span><span class="sxs-lookup"><span data-stu-id="b792f-161">Type</span></span>   |<span data-ttu-id="b792f-162">说明</span><span class="sxs-lookup"><span data-stu-id="b792f-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b792f-163">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b792f-163">multiValueExtendedProperties</span></span>|<span data-ttu-id="b792f-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b792f-164">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="b792f-165">为任务文件夹定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="b792f-165">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="b792f-166">只读。</span><span class="sxs-lookup"><span data-stu-id="b792f-166">Read-only.</span></span> <span data-ttu-id="b792f-167">可为空。</span><span class="sxs-lookup"><span data-stu-id="b792f-167">Nullable.</span></span>|
|<span data-ttu-id="b792f-168">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b792f-168">singleValueExtendedProperties</span></span>|<span data-ttu-id="b792f-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="b792f-169">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="b792f-170">为任务文件夹定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="b792f-170">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="b792f-171">只读。</span><span class="sxs-lookup"><span data-stu-id="b792f-171">Read-only.</span></span> <span data-ttu-id="b792f-172">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b792f-172">Nullable.</span></span>|
|<span data-ttu-id="b792f-173">任务</span><span class="sxs-lookup"><span data-stu-id="b792f-173">tasks</span></span>|<span data-ttu-id="b792f-174">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b792f-174">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="b792f-175">此任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="b792f-175">The tasks in this task folder.</span></span> <span data-ttu-id="b792f-176">只读。</span><span class="sxs-lookup"><span data-stu-id="b792f-176">Read-only.</span></span> <span data-ttu-id="b792f-177">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b792f-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b792f-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b792f-178">JSON representation</span></span>
<span data-ttu-id="b792f-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b792f-179">Here is a JSON representation of the resource.</span></span>

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
