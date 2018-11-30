---
title: outlookTaskFolder 资源类型
description: '包含 Outlook 任务 （outlookTask 对象的集合） 的文件夹。 '
ms.openlocfilehash: e3fb9d73dbd9458048749331d14f933d838d4243
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046985"
---
# <a name="outlooktaskfolder-resource-type"></a><span data-ttu-id="55cd8-103">outlookTaskFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="55cd8-103">outlookTaskFolder resource type</span></span>

> <span data-ttu-id="55cd8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55cd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55cd8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55cd8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55cd8-106">包含 Outlook 任务 （ [outlookTask](outlooktask.md)对象的集合） 的文件夹。</span><span class="sxs-lookup"><span data-stu-id="55cd8-106">A folder that contains Outlook tasks (collection of [outlookTask](outlooktask.md) objects).</span></span> 

<span data-ttu-id="55cd8-107">在 Outlook 中，默认任务组中， `My Tasks`，包含默认任务文件夹， `Tasks`，用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="55cd8-107">In Outlook, the default task group, `My Tasks`, contains a default task folder, `Tasks`, for the user's mailbox.</span></span> <span data-ttu-id="55cd8-108">无法重命名或删除这些默认任务组和文件夹，但您可以创建其他任务组和任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="55cd8-108">You cannot rename or delete these default task group and folder, but you can create additional task groups and task folders.</span></span>


## <a name="methods"></a><span data-ttu-id="55cd8-109">方法</span><span class="sxs-lookup"><span data-stu-id="55cd8-109">Methods</span></span>

| <span data-ttu-id="55cd8-110">方法</span><span class="sxs-lookup"><span data-stu-id="55cd8-110">Method</span></span>           | <span data-ttu-id="55cd8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="55cd8-111">Return Type</span></span>    |<span data-ttu-id="55cd8-112">说明</span><span class="sxs-lookup"><span data-stu-id="55cd8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55cd8-113">获取 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-113">Get outlookTaskFolder</span></span>](../api/outlooktaskfolder-get.md) | [<span data-ttu-id="55cd8-114">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-114">outlookTaskFolder</span></span>](outlooktaskfolder.md) |<span data-ttu-id="55cd8-115">要获取的属性和指定 Outlook 任务文件夹的关系。</span><span class="sxs-lookup"><span data-stu-id="55cd8-115">Get the properties and relationships of the specified Outlook task folder.</span></span>|
|[<span data-ttu-id="55cd8-116">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="55cd8-116">Create outlookTask</span></span>](../api/outlooktaskfolder-post-tasks.md) |[<span data-ttu-id="55cd8-117">outlookTask</span><span class="sxs-lookup"><span data-stu-id="55cd8-117">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="55cd8-118">在指定的任务文件夹中创建 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="55cd8-118">Create an Outlook task in the specified task folder.</span></span>|
|[<span data-ttu-id="55cd8-119">List tasks</span><span class="sxs-lookup"><span data-stu-id="55cd8-119">List tasks</span></span>](../api/outlooktaskfolder-list-tasks.md) |<span data-ttu-id="55cd8-120">[outlookTask](outlooktask.md)集合</span><span class="sxs-lookup"><span data-stu-id="55cd8-120">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="55cd8-121">在指定文件夹中获取所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="55cd8-121">Get all the Outlook tasks in the specified folder.</span></span>|
|[<span data-ttu-id="55cd8-122">Update</span><span class="sxs-lookup"><span data-stu-id="55cd8-122">Update</span></span>](../api/outlooktaskfolder-update.md) | [<span data-ttu-id="55cd8-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)   |<span data-ttu-id="55cd8-124">更新 Outlook 任务文件夹的可写属性。</span><span class="sxs-lookup"><span data-stu-id="55cd8-124">Update the writable properties of an Outlook task folder.</span></span> |
|[<span data-ttu-id="55cd8-125">删除</span><span class="sxs-lookup"><span data-stu-id="55cd8-125">Delete</span></span>](../api/outlooktaskfolder-delete.md) | <span data-ttu-id="55cd8-126">无</span><span class="sxs-lookup"><span data-stu-id="55cd8-126">None</span></span> |<span data-ttu-id="55cd8-127">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="55cd8-127">Delete the specified Outlook task folder.</span></span>|
|<span data-ttu-id="55cd8-128">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="55cd8-128">**Extended properties**</span></span>| | |
|[<span data-ttu-id="55cd8-129">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="55cd8-129">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="55cd8-130">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-130">outlookTaskFolder</span></span>](outlooktaskfolder.md)  |<span data-ttu-id="55cd8-131">在新的或现有的 Outlook 任务文件夹中创建一个或多个单值扩展的属性。</span><span class="sxs-lookup"><span data-stu-id="55cd8-131">Create one or more single-value extended properties in a new or existing Outlook task folder.</span></span>   |
|[<span data-ttu-id="55cd8-132">使用单值扩展属性获取任务文件夹</span><span class="sxs-lookup"><span data-stu-id="55cd8-132">Get task folder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="55cd8-133">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-133">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="55cd8-134">获取包含一个单值使用扩展属性的 Outlook 任务文件夹`$expand`或`$filter`。</span><span class="sxs-lookup"><span data-stu-id="55cd8-134">Get Outlook task folders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="55cd8-135">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="55cd8-135">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="55cd8-136">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-136">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="55cd8-137">在新的或现有的 Outlook 任务文件夹中创建一个或多个多值扩展的属性。</span><span class="sxs-lookup"><span data-stu-id="55cd8-137">Create one or more multi-value extended properties in a new or existing Outlook task folder.</span></span>  |
|[<span data-ttu-id="55cd8-138">多值扩展属性获取任务文件夹</span><span class="sxs-lookup"><span data-stu-id="55cd8-138">Get task folder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="55cd8-139">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-139">outlookTaskFolder</span></span>](outlooktaskfolder.md) | <span data-ttu-id="55cd8-140">获取包含多值扩展的属性，通过使用 Outlook 任务文件夹`$expand`。</span><span class="sxs-lookup"><span data-stu-id="55cd8-140">Get an Outlook task folder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="55cd8-141">属性</span><span class="sxs-lookup"><span data-stu-id="55cd8-141">Properties</span></span>
| <span data-ttu-id="55cd8-142">属性</span><span class="sxs-lookup"><span data-stu-id="55cd8-142">Property</span></span>     | <span data-ttu-id="55cd8-143">类型</span><span class="sxs-lookup"><span data-stu-id="55cd8-143">Type</span></span>   |<span data-ttu-id="55cd8-144">说明</span><span class="sxs-lookup"><span data-stu-id="55cd8-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55cd8-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="55cd8-145">changeKey</span></span>|<span data-ttu-id="55cd8-146">字符串</span><span class="sxs-lookup"><span data-stu-id="55cd8-146">String</span></span>|<span data-ttu-id="55cd8-147">任务文件夹的版本。</span><span class="sxs-lookup"><span data-stu-id="55cd8-147">The version of the task folder.</span></span>|
|<span data-ttu-id="55cd8-148">id</span><span class="sxs-lookup"><span data-stu-id="55cd8-148">id</span></span>|<span data-ttu-id="55cd8-149">字符串</span><span class="sxs-lookup"><span data-stu-id="55cd8-149">String</span></span>|<span data-ttu-id="55cd8-150">任务文件夹中，用户的邮箱中的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="55cd8-150">The identifier of the task folder, unique in the user's mailbox.</span></span> <span data-ttu-id="55cd8-151">只读。</span><span class="sxs-lookup"><span data-stu-id="55cd8-151">Read-only.</span></span>|
|<span data-ttu-id="55cd8-152">isDefaultFolder</span><span class="sxs-lookup"><span data-stu-id="55cd8-152">isDefaultFolder</span></span>|<span data-ttu-id="55cd8-153">布尔</span><span class="sxs-lookup"><span data-stu-id="55cd8-153">Boolean</span></span>|<span data-ttu-id="55cd8-154">如果文件夹为默认的任务文件夹，则为 true。</span><span class="sxs-lookup"><span data-stu-id="55cd8-154">True if the folder is the default task folder.</span></span>|
|<span data-ttu-id="55cd8-155">name</span><span class="sxs-lookup"><span data-stu-id="55cd8-155">name</span></span>|<span data-ttu-id="55cd8-156">字符串</span><span class="sxs-lookup"><span data-stu-id="55cd8-156">String</span></span>|<span data-ttu-id="55cd8-157">任务文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="55cd8-157">The name of the task folder.</span></span>|
|<span data-ttu-id="55cd8-158">parentGroupKey</span><span class="sxs-lookup"><span data-stu-id="55cd8-158">parentGroupKey</span></span>|<span data-ttu-id="55cd8-159">Guid</span><span class="sxs-lookup"><span data-stu-id="55cd8-159">Guid</span></span>|<span data-ttu-id="55cd8-160">任务文件夹的父组的唯一 GUID 标识符。</span><span class="sxs-lookup"><span data-stu-id="55cd8-160">The unique GUID identifier for the task folder's parent group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55cd8-161">Relationships</span><span class="sxs-lookup"><span data-stu-id="55cd8-161">Relationships</span></span>
| <span data-ttu-id="55cd8-162">关系</span><span class="sxs-lookup"><span data-stu-id="55cd8-162">Relationship</span></span> | <span data-ttu-id="55cd8-163">类型</span><span class="sxs-lookup"><span data-stu-id="55cd8-163">Type</span></span>   |<span data-ttu-id="55cd8-164">说明</span><span class="sxs-lookup"><span data-stu-id="55cd8-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55cd8-165">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="55cd8-165">multiValueExtendedProperties</span></span>|<span data-ttu-id="55cd8-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55cd8-166">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="55cd8-167">多值定义的任务文件夹的扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="55cd8-167">The collection of multi-value extended properties defined for the task folder.</span></span> <span data-ttu-id="55cd8-168">只读。</span><span class="sxs-lookup"><span data-stu-id="55cd8-168">Read-only.</span></span> <span data-ttu-id="55cd8-169">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="55cd8-169">Nullable.</span></span>|
|<span data-ttu-id="55cd8-170">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="55cd8-170">singleValueExtendedProperties</span></span>|<span data-ttu-id="55cd8-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="55cd8-171">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="55cd8-172">定义的任务文件夹的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="55cd8-172">The collection of single-value extended properties defined for the task folder.</span></span> <span data-ttu-id="55cd8-173">只读。</span><span class="sxs-lookup"><span data-stu-id="55cd8-173">Read-only.</span></span> <span data-ttu-id="55cd8-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="55cd8-174">Nullable.</span></span>|
|<span data-ttu-id="55cd8-175">tasks</span><span class="sxs-lookup"><span data-stu-id="55cd8-175">tasks</span></span>|<span data-ttu-id="55cd8-176">[outlookTask](outlooktask.md)集合</span><span class="sxs-lookup"><span data-stu-id="55cd8-176">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="55cd8-177">此任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="55cd8-177">The tasks in this task folder.</span></span> <span data-ttu-id="55cd8-178">只读。</span><span class="sxs-lookup"><span data-stu-id="55cd8-178">Read-only.</span></span> <span data-ttu-id="55cd8-179">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="55cd8-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55cd8-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55cd8-180">JSON representation</span></span>
<span data-ttu-id="55cd8-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55cd8-181">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->