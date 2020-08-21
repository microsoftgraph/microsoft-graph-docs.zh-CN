---
title: outlookTask 资源类型
description: '可用于跟踪工作项目的 Outlook 项目。 '
author: mashriv
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f580c9d39ad9252cc94274c50e6c2dfca704ceff
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849579"
---
# <a name="outlooktask-resource-type"></a><span data-ttu-id="e58a1-103">outlookTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="e58a1-103">outlookTask resource type</span></span>

<span data-ttu-id="e58a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e58a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]

<span data-ttu-id="e58a1-105">可用于跟踪工作项目的 Outlook 项目。</span><span class="sxs-lookup"><span data-stu-id="e58a1-105">An Outlook item that can track a work item.</span></span>

<span data-ttu-id="e58a1-106">你可以使用任务来跟踪开始、截止和实际完成日期及时间、其进度或状态、它是否为定期任务并且需要提醒。</span><span class="sxs-lookup"><span data-stu-id="e58a1-106">You can use a task to track the start, due and actual completion dates and times, its progress or status, whether it's recurring, and requires reminding.</span></span>

<span data-ttu-id="e58a1-107">**outlookTask** 资源中与日期相关的属性包括：</span><span class="sxs-lookup"><span data-stu-id="e58a1-107">Date-related properties in the **outlookTask** resource include the following:</span></span>

- <span data-ttu-id="e58a1-108">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-108">completedDateTime</span></span>
- <span data-ttu-id="e58a1-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-109">createdDateTime</span></span>
- <span data-ttu-id="e58a1-110">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-110">dueDateTime</span></span>
- <span data-ttu-id="e58a1-111">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-111">lastModifiedDateTime</span></span>
- <span data-ttu-id="e58a1-112">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-112">reminderDateTime</span></span>
- <span data-ttu-id="e58a1-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-113">startDateTime</span></span>

<span data-ttu-id="e58a1-114">默认情况下，POST、GET、PATCH 和[完成](../api/outlooktask-complete.md)操作会在 UTC 的 REST 响应中返回与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="e58a1-114">By default, the POST, GET, PATCH, and [complete](../api/outlooktask-complete.md) operations return date-related properties in their REST responses in UTC.</span></span>
<span data-ttu-id="e58a1-115">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="e58a1-115">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="e58a1-116">以下示例在对应响应的 EST 中返回与日期相关的属性：</span><span class="sxs-lookup"><span data-stu-id="e58a1-116">The following example returns date-related properties in EST in the corresponding response:</span></span>

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a><span data-ttu-id="e58a1-117">方法</span><span class="sxs-lookup"><span data-stu-id="e58a1-117">Methods</span></span>

| <span data-ttu-id="e58a1-118">方法</span><span class="sxs-lookup"><span data-stu-id="e58a1-118">Method</span></span>           | <span data-ttu-id="e58a1-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="e58a1-119">Return Type</span></span>    |<span data-ttu-id="e58a1-120">说明</span><span class="sxs-lookup"><span data-stu-id="e58a1-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e58a1-121">获取 outlookTask</span><span class="sxs-lookup"><span data-stu-id="e58a1-121">Get outlookTask</span></span>](../api/outlooktask-get.md) | [<span data-ttu-id="e58a1-122">outlookTask</span><span class="sxs-lookup"><span data-stu-id="e58a1-122">outlookTask</span></span>](outlooktask.md) |<span data-ttu-id="e58a1-123">获取用户邮箱中的 Outlook 任务的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e58a1-123">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>|
|[<span data-ttu-id="e58a1-124">更新</span><span class="sxs-lookup"><span data-stu-id="e58a1-124">Update</span></span>](../api/outlooktask-update.md) | [<span data-ttu-id="e58a1-125">outlookTask</span><span class="sxs-lookup"><span data-stu-id="e58a1-125">outlookTask</span></span>](outlooktask.md) |<span data-ttu-id="e58a1-126">更改 Outlook 任务的可写属性。</span><span class="sxs-lookup"><span data-stu-id="e58a1-126">Change writeable properties of an Outlook task.</span></span> |
|[<span data-ttu-id="e58a1-127">删除</span><span class="sxs-lookup"><span data-stu-id="e58a1-127">Delete</span></span>](../api/outlooktask-delete.md) | <span data-ttu-id="e58a1-128">无</span><span class="sxs-lookup"><span data-stu-id="e58a1-128">None</span></span> |<span data-ttu-id="e58a1-129">删除用户邮箱中的指定任务。</span><span class="sxs-lookup"><span data-stu-id="e58a1-129">Delete the specified task in the user's mailbox.</span></span> |
|[<span data-ttu-id="e58a1-130">完成</span><span class="sxs-lookup"><span data-stu-id="e58a1-130">Complete</span></span>](../api/outlooktask-complete.md)|<span data-ttu-id="e58a1-131">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e58a1-131">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="e58a1-132">完成 Outlook 任务，它将 **completedDateTime** 属性设置为当前日期，并将 **status** 属性设置为 `completed`。</span><span class="sxs-lookup"><span data-stu-id="e58a1-132">Complete an Outlook task which sets the **completedDateTime** property to the current date, and **status** property to `completed`.</span></span>|
|<span data-ttu-id="e58a1-133">**附件**</span><span class="sxs-lookup"><span data-stu-id="e58a1-133">**Attachments**</span></span>| | |
|[<span data-ttu-id="e58a1-134">列出附件</span><span class="sxs-lookup"><span data-stu-id="e58a1-134">List attachments</span></span>](../api/outlooktask-list-attachments.md) |<span data-ttu-id="e58a1-135">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e58a1-135">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="e58a1-136">获取 Outlook 任务的所有附件。</span><span class="sxs-lookup"><span data-stu-id="e58a1-136">Get all attachments on an Outlook task.</span></span>|
|[<span data-ttu-id="e58a1-137">添加附件</span><span class="sxs-lookup"><span data-stu-id="e58a1-137">Add attachment</span></span>](../api/outlooktask-post-attachments.md) |[<span data-ttu-id="e58a1-138">附件</span><span class="sxs-lookup"><span data-stu-id="e58a1-138">attachment</span></span>](attachment.md)| <span data-ttu-id="e58a1-139">向任务添加作为附件的文件、项目（消息、事件或联系人）或文件链接。</span><span class="sxs-lookup"><span data-stu-id="e58a1-139">Add a file, item (message, event or contact), or link to a file as an attachment to a task.</span></span>|
|<span data-ttu-id="e58a1-140">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="e58a1-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="e58a1-141">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="e58a1-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="e58a1-142">outlookTask</span><span class="sxs-lookup"><span data-stu-id="e58a1-142">outlookTask</span></span>](outlooktask.md)  |<span data-ttu-id="e58a1-143">在新建或现有 Outlook 任务中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e58a1-143">Create one or more single-value extended properties in a new or existing Outlook task.</span></span>   |
|[<span data-ttu-id="e58a1-144">获取具有单值扩展属性的任务</span><span class="sxs-lookup"><span data-stu-id="e58a1-144">Get task with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e58a1-145">outlookTask</span><span class="sxs-lookup"><span data-stu-id="e58a1-145">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="e58a1-146">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="e58a1-146">Get Outlook tasks that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e58a1-147">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="e58a1-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="e58a1-148">outlookTask</span><span class="sxs-lookup"><span data-stu-id="e58a1-148">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="e58a1-149">在新建或现有的 Outlook 任务中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e58a1-149">Create one or more multi-value extended properties in a new or existing Outlook task.</span></span>  |
|[<span data-ttu-id="e58a1-150">获取具有多值扩展属性的任务</span><span class="sxs-lookup"><span data-stu-id="e58a1-150">Get task with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e58a1-151">outlookTask</span><span class="sxs-lookup"><span data-stu-id="e58a1-151">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="e58a1-152">使用 `$expand` 获取包含一个多值扩展属性的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="e58a1-152">Get an Outlook task that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="e58a1-153">属性</span><span class="sxs-lookup"><span data-stu-id="e58a1-153">Properties</span></span>
| <span data-ttu-id="e58a1-154">属性</span><span class="sxs-lookup"><span data-stu-id="e58a1-154">Property</span></span>     | <span data-ttu-id="e58a1-155">类型</span><span class="sxs-lookup"><span data-stu-id="e58a1-155">Type</span></span>   |<span data-ttu-id="e58a1-156">说明</span><span class="sxs-lookup"><span data-stu-id="e58a1-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e58a1-157">assignedTo</span><span class="sxs-lookup"><span data-stu-id="e58a1-157">assignedTo</span></span>|<span data-ttu-id="e58a1-158">String</span><span class="sxs-lookup"><span data-stu-id="e58a1-158">String</span></span>|<span data-ttu-id="e58a1-159">Outlook 中已为其分配任务的人员姓名。</span><span class="sxs-lookup"><span data-stu-id="e58a1-159">The name of the person who has been assigned the task in Outlook.</span></span> <span data-ttu-id="e58a1-160">只读。</span><span class="sxs-lookup"><span data-stu-id="e58a1-160">Read-only.</span></span>|
|<span data-ttu-id="e58a1-161">正文</span><span class="sxs-lookup"><span data-stu-id="e58a1-161">body</span></span>|[<span data-ttu-id="e58a1-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="e58a1-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="e58a1-163">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="e58a1-163">The task body that typically contains information about the task.</span></span> <span data-ttu-id="e58a1-164">请注意，仅支持 HTML 类型。</span><span class="sxs-lookup"><span data-stu-id="e58a1-164">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="e58a1-165">类别</span><span class="sxs-lookup"><span data-stu-id="e58a1-165">categories</span></span>|<span data-ttu-id="e58a1-166">String 集合</span><span class="sxs-lookup"><span data-stu-id="e58a1-166">String collection</span></span>|<span data-ttu-id="e58a1-167">与任务关联的类别。</span><span class="sxs-lookup"><span data-stu-id="e58a1-167">The categories associated with the task.</span></span> <span data-ttu-id="e58a1-168">每个类别对应于用户定义的 [outlookCategory](outlookcategory.md) 的 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="e58a1-168">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that the user has defined.</span></span>|
|<span data-ttu-id="e58a1-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="e58a1-169">changeKey</span></span>|<span data-ttu-id="e58a1-170">String</span><span class="sxs-lookup"><span data-stu-id="e58a1-170">String</span></span>|<span data-ttu-id="e58a1-171">任务的版本。</span><span class="sxs-lookup"><span data-stu-id="e58a1-171">The version of the task.</span></span>|
|<span data-ttu-id="e58a1-172">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-172">completedDateTime</span></span>|[<span data-ttu-id="e58a1-173">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e58a1-173">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e58a1-174">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="e58a1-174">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="e58a1-175">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-175">createdDateTime</span></span>|<span data-ttu-id="e58a1-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e58a1-176">DateTimeOffset</span></span>|<span data-ttu-id="e58a1-177">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e58a1-177">The date and time when the task was created.</span></span> <span data-ttu-id="e58a1-178">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="e58a1-178">By default, it is in UTC.</span></span> <span data-ttu-id="e58a1-179">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="e58a1-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="e58a1-180">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="e58a1-180">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="e58a1-181">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e58a1-181">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e58a1-182">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-182">dueDateTime</span></span>|[<span data-ttu-id="e58a1-183">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e58a1-183">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e58a1-184">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="e58a1-184">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="e58a1-185">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="e58a1-185">hasAttachments</span></span>|<span data-ttu-id="e58a1-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e58a1-186">Boolean</span></span>|<span data-ttu-id="e58a1-187">如果任务包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="e58a1-187">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="e58a1-188">id</span><span class="sxs-lookup"><span data-stu-id="e58a1-188">id</span></span>|<span data-ttu-id="e58a1-189">String</span><span class="sxs-lookup"><span data-stu-id="e58a1-189">String</span></span>| <span data-ttu-id="e58a1-190">任务的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e58a1-190">Unique identifier for the task.</span></span> <span data-ttu-id="e58a1-191">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 只读。</span><span class="sxs-lookup"><span data-stu-id="e58a1-191">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Read-only.</span></span> |
|<span data-ttu-id="e58a1-192">importance</span><span class="sxs-lookup"><span data-stu-id="e58a1-192">importance</span></span>|<span data-ttu-id="e58a1-193">string</span><span class="sxs-lookup"><span data-stu-id="e58a1-193">string</span></span>|<span data-ttu-id="e58a1-194">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="e58a1-194">The importance of the event.</span></span> <span data-ttu-id="e58a1-195">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e58a1-195">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="e58a1-196">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="e58a1-196">isReminderOn</span></span>|<span data-ttu-id="e58a1-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="e58a1-197">Boolean</span></span>|<span data-ttu-id="e58a1-198">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="e58a1-198">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="e58a1-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-199">lastModifiedDateTime</span></span>|<span data-ttu-id="e58a1-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e58a1-200">DateTimeOffset</span></span>|<span data-ttu-id="e58a1-201">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e58a1-201">The date and time when the task was last modified.</span></span> <span data-ttu-id="e58a1-202">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="e58a1-202">By default, it is in UTC.</span></span> <span data-ttu-id="e58a1-203">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="e58a1-203">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="e58a1-204">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e58a1-204">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e58a1-205">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e58a1-205">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e58a1-206">所有者</span><span class="sxs-lookup"><span data-stu-id="e58a1-206">owner</span></span>|<span data-ttu-id="e58a1-207">String</span><span class="sxs-lookup"><span data-stu-id="e58a1-207">String</span></span>|<span data-ttu-id="e58a1-208">任务创建者的姓名。</span><span class="sxs-lookup"><span data-stu-id="e58a1-208">The name of the person who created the task.</span></span>|
|<span data-ttu-id="e58a1-209">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e58a1-209">parentFolderId</span></span>|<span data-ttu-id="e58a1-210">String</span><span class="sxs-lookup"><span data-stu-id="e58a1-210">String</span></span>|<span data-ttu-id="e58a1-211">任务的父文件夹的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e58a1-211">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="e58a1-212">定期</span><span class="sxs-lookup"><span data-stu-id="e58a1-212">recurrence</span></span>|[<span data-ttu-id="e58a1-213">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e58a1-213">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="e58a1-214">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="e58a1-214">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="e58a1-215">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-215">reminderDateTime</span></span>|[<span data-ttu-id="e58a1-216">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e58a1-216">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e58a1-217">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e58a1-217">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="e58a1-218">敏感度</span><span class="sxs-lookup"><span data-stu-id="e58a1-218">sensitivity</span></span>|<span data-ttu-id="e58a1-219">string</span><span class="sxs-lookup"><span data-stu-id="e58a1-219">string</span></span>|<span data-ttu-id="e58a1-220">指示任务的隐私级别。</span><span class="sxs-lookup"><span data-stu-id="e58a1-220">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="e58a1-221">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="e58a1-221">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="e58a1-222">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e58a1-222">startDateTime</span></span>|[<span data-ttu-id="e58a1-223">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e58a1-223">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e58a1-224">要在指定时区内开始执行任务的日期。</span><span class="sxs-lookup"><span data-stu-id="e58a1-224">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="e58a1-225">状态</span><span class="sxs-lookup"><span data-stu-id="e58a1-225">status</span></span>|<span data-ttu-id="e58a1-226">string</span><span class="sxs-lookup"><span data-stu-id="e58a1-226">string</span></span>|<span data-ttu-id="e58a1-227">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="e58a1-227">Indicates the state or progress of the task.</span></span> <span data-ttu-id="e58a1-228">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="e58a1-228">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="e58a1-229">主题</span><span class="sxs-lookup"><span data-stu-id="e58a1-229">subject</span></span>|<span data-ttu-id="e58a1-230">String</span><span class="sxs-lookup"><span data-stu-id="e58a1-230">String</span></span>|<span data-ttu-id="e58a1-231">任务的简要说明或标题。</span><span class="sxs-lookup"><span data-stu-id="e58a1-231">A brief description or title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e58a1-232">关系</span><span class="sxs-lookup"><span data-stu-id="e58a1-232">Relationships</span></span>
| <span data-ttu-id="e58a1-233">关系</span><span class="sxs-lookup"><span data-stu-id="e58a1-233">Relationship</span></span> | <span data-ttu-id="e58a1-234">类型</span><span class="sxs-lookup"><span data-stu-id="e58a1-234">Type</span></span>   |<span data-ttu-id="e58a1-235">说明</span><span class="sxs-lookup"><span data-stu-id="e58a1-235">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e58a1-236">attachments</span><span class="sxs-lookup"><span data-stu-id="e58a1-236">attachments</span></span>|<span data-ttu-id="e58a1-237">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e58a1-237">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="e58a1-238">任务的 [fileAttachment](fileattachment.md)、[itemAttachment](itemattachment.md) 和 [referenceAttachment](referenceattachment.md) 附件的集合。</span><span class="sxs-lookup"><span data-stu-id="e58a1-238">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the task.</span></span>  <span data-ttu-id="e58a1-239">只读。</span><span class="sxs-lookup"><span data-stu-id="e58a1-239">Read-only.</span></span> <span data-ttu-id="e58a1-240">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e58a1-240">Nullable.</span></span>|
|<span data-ttu-id="e58a1-241">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e58a1-241">multiValueExtendedProperties</span></span>|<span data-ttu-id="e58a1-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e58a1-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="e58a1-243">为任务定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="e58a1-243">The collection of multi-value extended properties defined for the task.</span></span> <span data-ttu-id="e58a1-244">只读。</span><span class="sxs-lookup"><span data-stu-id="e58a1-244">Read-only.</span></span> <span data-ttu-id="e58a1-245">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e58a1-245">Nullable.</span></span>|
|<span data-ttu-id="e58a1-246">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e58a1-246">singleValueExtendedProperties</span></span>|<span data-ttu-id="e58a1-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e58a1-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="e58a1-248">为任务定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="e58a1-248">The collection of single-value extended properties defined for the task.</span></span> <span data-ttu-id="e58a1-249">只读。</span><span class="sxs-lookup"><span data-stu-id="e58a1-249">Read-only.</span></span> <span data-ttu-id="e58a1-250">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e58a1-250">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e58a1-251">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e58a1-251">JSON representation</span></span>
<span data-ttu-id="e58a1-252">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e58a1-252">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTask"
}-->

```json
{
  "assignedTo": "String",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["String"],
  "changeKey": "String",
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "sensitivity": "string",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "string",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
