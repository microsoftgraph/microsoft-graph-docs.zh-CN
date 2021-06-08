---
title: timecard 资源类型
description: 计划中的考勤卡条目。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 25818e091ac2d4f6590fd7ea2c395752d0238bd0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786383"
---
# <a name="timecard-resource-type"></a><span data-ttu-id="ec55b-103">timecard 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec55b-103">timecard resource type</span></span>

<span data-ttu-id="ec55b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec55b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec55b-105">表示计划中的一个考勤卡条目。</span><span class="sxs-lookup"><span data-stu-id="ec55b-105">Represents a timecard entry in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="ec55b-106">方法</span><span class="sxs-lookup"><span data-stu-id="ec55b-106">Methods</span></span>

| <span data-ttu-id="ec55b-107">方法</span><span class="sxs-lookup"><span data-stu-id="ec55b-107">Method</span></span>       | <span data-ttu-id="ec55b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ec55b-108">Return type</span></span>  |<span data-ttu-id="ec55b-109">Description</span><span class="sxs-lookup"><span data-stu-id="ec55b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec55b-110">List</span><span class="sxs-lookup"><span data-stu-id="ec55b-110">List</span></span>](../api/timecard-list.md) | <span data-ttu-id="ec55b-111">[timeCard](timecard.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ec55b-111">[timeCard](timecard.md) collection</span></span> | <span data-ttu-id="ec55b-112">获取此 **计划中的 timecard** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ec55b-112">Get the list of **timecard** objects in this schedule.</span></span>|
|[<span data-ttu-id="ec55b-113">创建</span><span class="sxs-lookup"><span data-stu-id="ec55b-113">Create</span></span>](../api/timecard-post.md) | [<span data-ttu-id="ec55b-114">timeCard</span><span class="sxs-lookup"><span data-stu-id="ec55b-114">timeCard</span></span>](timecard.md) | <span data-ttu-id="ec55b-115">创建新的 **时间卡** 对象。</span><span class="sxs-lookup"><span data-stu-id="ec55b-115">Create a new **timecard** object.</span></span>|
|[<span data-ttu-id="ec55b-116">获取</span><span class="sxs-lookup"><span data-stu-id="ec55b-116">Get</span></span>](../api/timecard-get.md) | [<span data-ttu-id="ec55b-117">timeCard</span><span class="sxs-lookup"><span data-stu-id="ec55b-117">timeCard</span></span>](timecard.md) | <span data-ttu-id="ec55b-118">按 ID **获取** 时间卡对象。</span><span class="sxs-lookup"><span data-stu-id="ec55b-118">Get a **timecard** object by ID.</span></span>|
|[<span data-ttu-id="ec55b-119">Replace</span><span class="sxs-lookup"><span data-stu-id="ec55b-119">Replace</span></span>](../api/timecard-replace.md) | <span data-ttu-id="ec55b-120">无</span><span class="sxs-lookup"><span data-stu-id="ec55b-120">None</span></span> | <span data-ttu-id="ec55b-121">替换 **一个时间卡** 对象。</span><span class="sxs-lookup"><span data-stu-id="ec55b-121">Replace a **timecard** object.</span></span>|
|[<span data-ttu-id="ec55b-122">删除</span><span class="sxs-lookup"><span data-stu-id="ec55b-122">Delete</span></span>](../api/timecard-delete.md) | <span data-ttu-id="ec55b-123">无</span><span class="sxs-lookup"><span data-stu-id="ec55b-123">None</span></span> | <span data-ttu-id="ec55b-124">从 **计划中删除** 一个时间卡对象。</span><span class="sxs-lookup"><span data-stu-id="ec55b-124">Delete a **timecard** object from the schedule.</span></span>|
|[<span data-ttu-id="ec55b-125">clockIn</span><span class="sxs-lookup"><span data-stu-id="ec55b-125">clockIn</span></span>](../api/timecard-clockin.md) | [<span data-ttu-id="ec55b-126">timeCard</span><span class="sxs-lookup"><span data-stu-id="ec55b-126">timeCard</span></span>](timecard.md) | <span data-ttu-id="ec55b-127">Clock in to start a **timecard**.</span><span class="sxs-lookup"><span data-stu-id="ec55b-127">Clock in to start a **timecard**.</span></span>|
|[<span data-ttu-id="ec55b-128">clockOut</span><span class="sxs-lookup"><span data-stu-id="ec55b-128">clockOut</span></span>](../api/timecard-clockout.md) | <span data-ttu-id="ec55b-129">无</span><span class="sxs-lookup"><span data-stu-id="ec55b-129">None</span></span> | <span data-ttu-id="ec55b-130">时钟以结束打开的 **Timecard**。</span><span class="sxs-lookup"><span data-stu-id="ec55b-130">Clock out to end an open **timecard**.</span></span>|
|[<span data-ttu-id="ec55b-131">startBreak</span><span class="sxs-lookup"><span data-stu-id="ec55b-131">startBreak</span></span>](../api/timecard-startbreak.md) | <span data-ttu-id="ec55b-132">无</span><span class="sxs-lookup"><span data-stu-id="ec55b-132">None</span></span> | <span data-ttu-id="ec55b-133">启动特定时间卡 中的 **timeCardBreak** **。**</span><span class="sxs-lookup"><span data-stu-id="ec55b-133">Start a **timeCardBreak** in a specific **timecard**.</span></span>|
|[<span data-ttu-id="ec55b-134">endBreak</span><span class="sxs-lookup"><span data-stu-id="ec55b-134">endBreak</span></span>](../api/timecard-endbreak.md) | <span data-ttu-id="ec55b-135">无</span><span class="sxs-lookup"><span data-stu-id="ec55b-135">None</span></span> | <span data-ttu-id="ec55b-136">结束特定时间卡中打开的 **timeCardBreak。** </span><span class="sxs-lookup"><span data-stu-id="ec55b-136">End the open **timeCardBreak** in a specific **timecard**.</span></span>|
|[<span data-ttu-id="ec55b-137">confirmTimeCard</span><span class="sxs-lookup"><span data-stu-id="ec55b-137">confirmTimeCard</span></span>](../api/timecard-confirm.md) | <span data-ttu-id="ec55b-138">无</span><span class="sxs-lookup"><span data-stu-id="ec55b-138">None</span></span> | <span data-ttu-id="ec55b-139">确认 **一条时间卡** 记录。</span><span class="sxs-lookup"><span data-stu-id="ec55b-139">Confirm a **timecard** record.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec55b-140">属性</span><span class="sxs-lookup"><span data-stu-id="ec55b-140">Properties</span></span>
|<span data-ttu-id="ec55b-141">属性</span><span class="sxs-lookup"><span data-stu-id="ec55b-141">Property</span></span>               |<span data-ttu-id="ec55b-142">类型</span><span class="sxs-lookup"><span data-stu-id="ec55b-142">Type</span></span>           |<span data-ttu-id="ec55b-143">说明</span><span class="sxs-lookup"><span data-stu-id="ec55b-143">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="ec55b-144">id</span><span class="sxs-lookup"><span data-stu-id="ec55b-144">id</span></span>                    |`string`  |<span data-ttu-id="ec55b-145">timeCard的 ID。</span><span class="sxs-lookup"><span data-stu-id="ec55b-145">ID of the **timeCard**.</span></span>|
| <span data-ttu-id="ec55b-146">userId</span><span class="sxs-lookup"><span data-stu-id="ec55b-146">userId</span></span>                    |`string` |<span data-ttu-id="ec55b-147">**timeCard** 所属的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="ec55b-147">User ID to which  the **timeCard** belongs.</span></span> |
| <span data-ttu-id="ec55b-148">state</span><span class="sxs-lookup"><span data-stu-id="ec55b-148">state</span></span>                 |`timeCardState`  | <span data-ttu-id="ec55b-149">**timeCard** 在其生命周期中的当前状态。可能的值是 `clockedIn` `onBreak` `clockedOut` ：、、、。 `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="ec55b-149">The current state of the **timeCard** during its life cycle.Possible values are: `clockedIn`, `onBreak`, `clockedOut`, `unknownFutureValue`.</span></span>|
| <span data-ttu-id="ec55b-150">clockInEvent</span><span class="sxs-lookup"><span data-stu-id="ec55b-150">clockInEvent</span></span>       |[<span data-ttu-id="ec55b-151">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="ec55b-151">timeCardEvent</span></span>](../resources/timecardevent.md)    | <span data-ttu-id="ec55b-152">timeCard 的 **时钟事件**。</span><span class="sxs-lookup"><span data-stu-id="ec55b-152">The clock-in event of the **timeCard**.</span></span> |
| <span data-ttu-id="ec55b-153">clockOutEvent</span><span class="sxs-lookup"><span data-stu-id="ec55b-153">clockOutEvent</span></span>                 |[<span data-ttu-id="ec55b-154">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="ec55b-154">timeCardEvent</span></span>](../resources/timecardevent.md)  |<span data-ttu-id="ec55b-155">timeCard 的 **时钟出事件**。</span><span class="sxs-lookup"><span data-stu-id="ec55b-155">The clock-out event of the **timeCard**.</span></span> |
| <span data-ttu-id="ec55b-156">notes</span><span class="sxs-lookup"><span data-stu-id="ec55b-156">notes</span></span>                 | [<span data-ttu-id="ec55b-157">itemBody</span><span class="sxs-lookup"><span data-stu-id="ec55b-157">itemBody</span></span>](itembody.md)  |<span data-ttu-id="ec55b-158">有关 **timeCard 的注释**。</span><span class="sxs-lookup"><span data-stu-id="ec55b-158">Notes about the **timeCard**.</span></span> |
| <span data-ttu-id="ec55b-159">breaks</span><span class="sxs-lookup"><span data-stu-id="ec55b-159">breaks</span></span>    |<span data-ttu-id="ec55b-160">[timeCardBreak](timecardbreak.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ec55b-160">[timeCardBreak](timecardbreak.md) collection</span></span>  |<span data-ttu-id="ec55b-161">与 **timeCard** 关联的中断列表。</span><span class="sxs-lookup"><span data-stu-id="ec55b-161">The list of breaks associated with the **timeCard**.</span></span>|
| <span data-ttu-id="ec55b-162">originalEntry</span><span class="sxs-lookup"><span data-stu-id="ec55b-162">originalEntry</span></span>| [<span data-ttu-id="ec55b-163">timeCardEntry</span><span class="sxs-lookup"><span data-stu-id="ec55b-163">timeCardEntry</span></span>](../resources/timecardentry.md) | <span data-ttu-id="ec55b-164">用户编辑之前 timeCard 的原始 **timeCardEntry。** </span><span class="sxs-lookup"><span data-stu-id="ec55b-164">The original **timeCardEntry** of the **timeCard**, before user edits.</span></span> |
| <span data-ttu-id="ec55b-165">confirmedBy</span><span class="sxs-lookup"><span data-stu-id="ec55b-165">confirmedBy</span></span> |`confirmedBy`    | <span data-ttu-id="ec55b-166">指示此 **timeCard** 条目是否得到确认。</span><span class="sxs-lookup"><span data-stu-id="ec55b-166">Indicate if this **timeCard** entry is confirmed.</span></span> <span data-ttu-id="ec55b-167">可取值为：`none`、`user`、`manager`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ec55b-167">Possible values are `none`, `user`, `manager`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ec55b-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec55b-168">createdDateTime</span></span>|`Edm.dateTimeOffset`| <span data-ttu-id="ec55b-169">创建 **timeCard** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ec55b-169">The timestamp in which the **timeCard** was created.</span></span> |
|<span data-ttu-id="ec55b-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="ec55b-170">createdBy</span></span>|`IdentitySet`| <span data-ttu-id="ec55b-171">创建实体的人的标识。</span><span class="sxs-lookup"><span data-stu-id="ec55b-171">Identity of the person who created the entity.</span></span> |
|<span data-ttu-id="ec55b-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec55b-172">lastModifiedDateTime</span></span>|`dateTimeOffset`| <span data-ttu-id="ec55b-173">上次修改 **timeCard** 的时间戳。</span><span class="sxs-lookup"><span data-stu-id="ec55b-173">The timestamp in which the **timeCard** was last modified.</span></span>|
|<span data-ttu-id="ec55b-174">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ec55b-174">lastModifiedBy</span></span>| `IdentitySet`| <span data-ttu-id="ec55b-175">上次修改实体的人的标识。</span><span class="sxs-lookup"><span data-stu-id="ec55b-175">Identity of the person who last modified the entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec55b-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec55b-176">JSON representation</span></span>

<span data-ttu-id="ec55b-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec55b-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCard",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "clockInEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "clockOutEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "notes" : {"@odata.type":"microsoft.graph.itemBody"},
  "breaks" : [{"@odata.type":"microsoft.graph.timeCardEvent"}],
  "originalEntry" : {"@odata.type":"microsoft.graph.timeCardEntry"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCard resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
