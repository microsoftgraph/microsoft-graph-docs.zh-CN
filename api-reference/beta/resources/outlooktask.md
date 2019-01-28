---
title: outlookTask 资源类型
description: '可用于跟踪工作项目的 Outlook 项目。 '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 63ab43dd33cb50ff643316865a942659e92304d4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513345"
---
# <a name="outlooktask-resource-type"></a><span data-ttu-id="2cff1-103">outlookTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cff1-103">outlookTask resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cff1-104">可用于跟踪工作项目的 Outlook 项目。</span><span class="sxs-lookup"><span data-stu-id="2cff1-104">An Outlook item that can track a work item.</span></span> 

<span data-ttu-id="2cff1-105">你可以使用任务来跟踪开始、截止和实际完成日期及时间、其进度或状态、它是否为定期任务并且需要提醒。</span><span class="sxs-lookup"><span data-stu-id="2cff1-105">You can use a task to track the start, due and actual completion dates and times, its progress or status, whether it's recurring, and requires reminding.</span></span>

<span data-ttu-id="2cff1-106">**outlookTask** 资源中与日期相关的属性包括：</span><span class="sxs-lookup"><span data-stu-id="2cff1-106">Date-related properties in the **outlookTask** resource include the following:</span></span>

- <span data-ttu-id="2cff1-107">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-107">completedDateTime</span></span>
- <span data-ttu-id="2cff1-108">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-108">createdDateTime</span></span>
- <span data-ttu-id="2cff1-109">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-109">dueDateTime</span></span>
- <span data-ttu-id="2cff1-110">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-110">lastModifiedDateTime</span></span>
- <span data-ttu-id="2cff1-111">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-111">reminderDateTime</span></span>
- <span data-ttu-id="2cff1-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-112">startDateTime</span></span>

<span data-ttu-id="2cff1-113">默认情况下，POST、GET、PATCH 和[完成](../api/outlooktask-complete.md)操作会在 UTC 的 REST 响应中返回与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="2cff1-113">By default, the POST, GET, PATCH, and [complete](../api/outlooktask-complete.md) operations return date-related properties in their REST responses in UTC.</span></span> <span data-ttu-id="2cff1-114">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="2cff1-114">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="2cff1-115">以下示例在对应响应的 EST 中返回与日期相关的属性：</span><span class="sxs-lookup"><span data-stu-id="2cff1-115">The following example returns date-related properties in EST in the corresponding response:</span></span>

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a><span data-ttu-id="2cff1-116">方法</span><span class="sxs-lookup"><span data-stu-id="2cff1-116">Methods</span></span>

| <span data-ttu-id="2cff1-117">方法</span><span class="sxs-lookup"><span data-stu-id="2cff1-117">Method</span></span>           | <span data-ttu-id="2cff1-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="2cff1-118">Return Type</span></span>    |<span data-ttu-id="2cff1-119">说明</span><span class="sxs-lookup"><span data-stu-id="2cff1-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2cff1-120">获取 outlookTask</span><span class="sxs-lookup"><span data-stu-id="2cff1-120">Get outlookTask</span></span>](../api/outlooktask-get.md) | [<span data-ttu-id="2cff1-121">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2cff1-121">outlookTask</span></span>](outlooktask.md) |<span data-ttu-id="2cff1-122">获取用户邮箱中的 Outlook 任务的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cff1-122">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>|
|[<span data-ttu-id="2cff1-123">更新</span><span class="sxs-lookup"><span data-stu-id="2cff1-123">Update</span></span>](../api/outlooktask-update.md) | [<span data-ttu-id="2cff1-124">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2cff1-124">outlookTask</span></span>](outlooktask.md) |<span data-ttu-id="2cff1-125">更改 Outlook 任务的可写属性。</span><span class="sxs-lookup"><span data-stu-id="2cff1-125">Change writeable properties of an Outlook task.</span></span> |
|[<span data-ttu-id="2cff1-126">删除</span><span class="sxs-lookup"><span data-stu-id="2cff1-126">Delete</span></span>](../api/outlooktask-delete.md) | <span data-ttu-id="2cff1-127">无</span><span class="sxs-lookup"><span data-stu-id="2cff1-127">None</span></span> |<span data-ttu-id="2cff1-128">删除用户邮箱中的指定任务。</span><span class="sxs-lookup"><span data-stu-id="2cff1-128">Delete the specified task in the user's mailbox.</span></span> |
|[<span data-ttu-id="2cff1-129">完成</span><span class="sxs-lookup"><span data-stu-id="2cff1-129">Complete</span></span>](../api/outlooktask-complete.md)|<span data-ttu-id="2cff1-130">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2cff1-130">[outlookTask](outlooktask.md) collection</span></span>|<span data-ttu-id="2cff1-131">完成 Outlook 任务，它将 **completedDateTime** 属性设置为当前日期，并将 **status** 属性设置为 `completed`。</span><span class="sxs-lookup"><span data-stu-id="2cff1-131">Complete an Outlook task which sets the **completedDateTime** property to the current date, and **status** property to `completed`.</span></span>|
|<span data-ttu-id="2cff1-132">**附件**</span><span class="sxs-lookup"><span data-stu-id="2cff1-132">**Attachments**</span></span>| | |
|[<span data-ttu-id="2cff1-133">列出附件</span><span class="sxs-lookup"><span data-stu-id="2cff1-133">List attachments</span></span>](../api/outlooktask-list-attachments.md) |<span data-ttu-id="2cff1-134">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2cff1-134">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="2cff1-135">获取 Outlook 任务的所有附件。</span><span class="sxs-lookup"><span data-stu-id="2cff1-135">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="2cff1-136">添加附件</span><span class="sxs-lookup"><span data-stu-id="2cff1-136">Add attachment</span></span>](../api/outlooktask-post-attachments.md) |[<span data-ttu-id="2cff1-137">附件</span><span class="sxs-lookup"><span data-stu-id="2cff1-137">attachment</span></span>](attachment.md)| <span data-ttu-id="2cff1-138">向任务添加作为附件的文件、项目（消息、事件或联系人）或文件链接。</span><span class="sxs-lookup"><span data-stu-id="2cff1-138">Add a file, item (message, event or contact), or link to a file as an attachment to a task.</span></span>|
|<span data-ttu-id="2cff1-139">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="2cff1-139">**Extended properties**</span></span>| | |
|[<span data-ttu-id="2cff1-140">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="2cff1-140">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="2cff1-141">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2cff1-141">outlookTask</span></span>](outlooktask.md)  |<span data-ttu-id="2cff1-142">在新建或现有 Outlook 任务中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="2cff1-142">Create one or more single-value extended properties in a new or existing Outlook task.</span></span>   |
|[<span data-ttu-id="2cff1-143">获取具有单值扩展属性的任务</span><span class="sxs-lookup"><span data-stu-id="2cff1-143">Get task with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="2cff1-144">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2cff1-144">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="2cff1-145">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="2cff1-145">Get Outlook tasks that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="2cff1-146">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="2cff1-146">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="2cff1-147">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2cff1-147">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="2cff1-148">在新建或现有的 Outlook 任务中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="2cff1-148">Create one or more multi-value extended properties in a new or existing Outlook task.</span></span>  |
|[<span data-ttu-id="2cff1-149">获取具有多值扩展属性的任务</span><span class="sxs-lookup"><span data-stu-id="2cff1-149">Get task with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="2cff1-150">outlookTask</span><span class="sxs-lookup"><span data-stu-id="2cff1-150">outlookTask</span></span>](outlooktask.md) | <span data-ttu-id="2cff1-151">使用 `$expand` 获取包含一个多值扩展属性的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="2cff1-151">Get an Outlook task that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="2cff1-152">属性</span><span class="sxs-lookup"><span data-stu-id="2cff1-152">Properties</span></span>
| <span data-ttu-id="2cff1-153">属性</span><span class="sxs-lookup"><span data-stu-id="2cff1-153">Property</span></span>     | <span data-ttu-id="2cff1-154">类型</span><span class="sxs-lookup"><span data-stu-id="2cff1-154">Type</span></span>   |<span data-ttu-id="2cff1-155">说明</span><span class="sxs-lookup"><span data-stu-id="2cff1-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cff1-156">assignedTo</span><span class="sxs-lookup"><span data-stu-id="2cff1-156">assignedTo</span></span>|<span data-ttu-id="2cff1-157">String</span><span class="sxs-lookup"><span data-stu-id="2cff1-157">String</span></span>|<span data-ttu-id="2cff1-158">已为其分配任务的人员姓名。</span><span class="sxs-lookup"><span data-stu-id="2cff1-158">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="2cff1-159">正文</span><span class="sxs-lookup"><span data-stu-id="2cff1-159">body</span></span>|[<span data-ttu-id="2cff1-160">itemBody</span><span class="sxs-lookup"><span data-stu-id="2cff1-160">itemBody</span></span>](itembody.md)|<span data-ttu-id="2cff1-161">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="2cff1-161">The task body that typically contains information about the task.</span></span> <span data-ttu-id="2cff1-162">请注意，仅支持 HTML 类型。</span><span class="sxs-lookup"><span data-stu-id="2cff1-162">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="2cff1-163">类别</span><span class="sxs-lookup"><span data-stu-id="2cff1-163">categories</span></span>|<span data-ttu-id="2cff1-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="2cff1-164">String collection</span></span>|<span data-ttu-id="2cff1-165">与任务关联的类别。</span><span class="sxs-lookup"><span data-stu-id="2cff1-165">The categories associated with the task.</span></span> <span data-ttu-id="2cff1-166">每个类别对应于用户定义的 [outlookCategory](outlookcategory.md) 的 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="2cff1-166">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) that the user has defined.</span></span>|
|<span data-ttu-id="2cff1-167">changeKey</span><span class="sxs-lookup"><span data-stu-id="2cff1-167">changeKey</span></span>|<span data-ttu-id="2cff1-168">String</span><span class="sxs-lookup"><span data-stu-id="2cff1-168">String</span></span>|<span data-ttu-id="2cff1-169">任务的版本。</span><span class="sxs-lookup"><span data-stu-id="2cff1-169">The version of the task.</span></span>|
|<span data-ttu-id="2cff1-170">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-170">completedDateTime</span></span>|[<span data-ttu-id="2cff1-171">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2cff1-171">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2cff1-172">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="2cff1-172">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="2cff1-173">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-173">createdDateTime</span></span>|<span data-ttu-id="2cff1-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cff1-174">DateTimeOffset</span></span>|<span data-ttu-id="2cff1-175">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2cff1-175">The date and time when the task was created.</span></span> <span data-ttu-id="2cff1-176">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="2cff1-176">By default, it is in UTC.</span></span> <span data-ttu-id="2cff1-177">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="2cff1-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="2cff1-178">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="2cff1-178">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="2cff1-179">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="2cff1-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2cff1-180">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-180">dueDateTime</span></span>|[<span data-ttu-id="2cff1-181">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2cff1-181">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2cff1-182">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="2cff1-182">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="2cff1-183">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="2cff1-183">hasAttachments</span></span>|<span data-ttu-id="2cff1-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cff1-184">Boolean</span></span>|<span data-ttu-id="2cff1-185">如果任务包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="2cff1-185">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="2cff1-186">id</span><span class="sxs-lookup"><span data-stu-id="2cff1-186">id</span></span>|<span data-ttu-id="2cff1-187">String</span><span class="sxs-lookup"><span data-stu-id="2cff1-187">String</span></span>|<span data-ttu-id="2cff1-188">任务的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2cff1-188">The unique identifier of the task.</span></span> <span data-ttu-id="2cff1-189">只读。</span><span class="sxs-lookup"><span data-stu-id="2cff1-189">Read-only.</span></span>|
|<span data-ttu-id="2cff1-190">重要性</span><span class="sxs-lookup"><span data-stu-id="2cff1-190">importance</span></span>|<span data-ttu-id="2cff1-191">string</span><span class="sxs-lookup"><span data-stu-id="2cff1-191">string</span></span>|<span data-ttu-id="2cff1-192">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="2cff1-192">The importance of the event.</span></span> <span data-ttu-id="2cff1-193">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="2cff1-193">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="2cff1-194">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="2cff1-194">isReminderOn</span></span>|<span data-ttu-id="2cff1-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cff1-195">Boolean</span></span>|<span data-ttu-id="2cff1-196">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="2cff1-196">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="2cff1-197">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-197">lastModifiedDateTime</span></span>|<span data-ttu-id="2cff1-198">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cff1-198">DateTimeOffset</span></span>|<span data-ttu-id="2cff1-199">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2cff1-199">The date and time when the task was last modified.</span></span> <span data-ttu-id="2cff1-200">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="2cff1-200">By default, it is in UTC.</span></span> <span data-ttu-id="2cff1-201">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="2cff1-201">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="2cff1-202">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2cff1-202">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2cff1-203">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="2cff1-203">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2cff1-204">所有者</span><span class="sxs-lookup"><span data-stu-id="2cff1-204">owner</span></span>|<span data-ttu-id="2cff1-205">String</span><span class="sxs-lookup"><span data-stu-id="2cff1-205">String</span></span>|<span data-ttu-id="2cff1-206">任务创建者的姓名。</span><span class="sxs-lookup"><span data-stu-id="2cff1-206">The name of the person who created the task.</span></span>|
|<span data-ttu-id="2cff1-207">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="2cff1-207">parentFolderId</span></span>|<span data-ttu-id="2cff1-208">String</span><span class="sxs-lookup"><span data-stu-id="2cff1-208">String</span></span>|<span data-ttu-id="2cff1-209">任务的父文件夹的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2cff1-209">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="2cff1-210">定期</span><span class="sxs-lookup"><span data-stu-id="2cff1-210">recurrence</span></span>|[<span data-ttu-id="2cff1-211">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="2cff1-211">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="2cff1-212">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="2cff1-212">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="2cff1-213">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-213">reminderDateTime</span></span>|[<span data-ttu-id="2cff1-214">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2cff1-214">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2cff1-215">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2cff1-215">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="2cff1-216">敏感度</span><span class="sxs-lookup"><span data-stu-id="2cff1-216">sensitivity</span></span>|<span data-ttu-id="2cff1-217">string</span><span class="sxs-lookup"><span data-stu-id="2cff1-217">string</span></span>|<span data-ttu-id="2cff1-218">指示任务的隐私级别。</span><span class="sxs-lookup"><span data-stu-id="2cff1-218">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="2cff1-219">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="2cff1-219">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="2cff1-220">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2cff1-220">startDateTime</span></span>|[<span data-ttu-id="2cff1-221">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2cff1-221">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2cff1-222">要在指定时区内开始执行任务的日期。</span><span class="sxs-lookup"><span data-stu-id="2cff1-222">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="2cff1-223">状态</span><span class="sxs-lookup"><span data-stu-id="2cff1-223">status</span></span>|<span data-ttu-id="2cff1-224">string</span><span class="sxs-lookup"><span data-stu-id="2cff1-224">string</span></span>|<span data-ttu-id="2cff1-225">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="2cff1-225">Indicates the state or progress of the task.</span></span> <span data-ttu-id="2cff1-226">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="2cff1-226">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="2cff1-227">主题</span><span class="sxs-lookup"><span data-stu-id="2cff1-227">subject</span></span>|<span data-ttu-id="2cff1-228">String</span><span class="sxs-lookup"><span data-stu-id="2cff1-228">String</span></span>|<span data-ttu-id="2cff1-229">任务的简要说明或标题。</span><span class="sxs-lookup"><span data-stu-id="2cff1-229">A brief description or title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cff1-230">关系</span><span class="sxs-lookup"><span data-stu-id="2cff1-230">Relationships</span></span>
| <span data-ttu-id="2cff1-231">关系</span><span class="sxs-lookup"><span data-stu-id="2cff1-231">Relationship</span></span> | <span data-ttu-id="2cff1-232">类型</span><span class="sxs-lookup"><span data-stu-id="2cff1-232">Type</span></span>   |<span data-ttu-id="2cff1-233">说明</span><span class="sxs-lookup"><span data-stu-id="2cff1-233">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cff1-234">attachments</span><span class="sxs-lookup"><span data-stu-id="2cff1-234">attachments</span></span>|<span data-ttu-id="2cff1-235">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2cff1-235">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="2cff1-236">任务的 [fileAttachment](fileattachment.md)、[itemAttachment](itemattachment.md) 和 [referenceAttachment](referenceattachment.md) 附件的集合。</span><span class="sxs-lookup"><span data-stu-id="2cff1-236">The collection of [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md), and [referenceAttachment](referenceattachment.md) attachments for the task.</span></span>  <span data-ttu-id="2cff1-237">只读。</span><span class="sxs-lookup"><span data-stu-id="2cff1-237">Read-only.</span></span> <span data-ttu-id="2cff1-238">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2cff1-238">Nullable.</span></span>|
|<span data-ttu-id="2cff1-239">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2cff1-239">multiValueExtendedProperties</span></span>|<span data-ttu-id="2cff1-240">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2cff1-240">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="2cff1-241">为任务定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="2cff1-241">The collection of multi-value extended properties defined for the task.</span></span> <span data-ttu-id="2cff1-242">只读。</span><span class="sxs-lookup"><span data-stu-id="2cff1-242">Read-only.</span></span> <span data-ttu-id="2cff1-243">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2cff1-243">Nullable.</span></span>|
|<span data-ttu-id="2cff1-244">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2cff1-244">singleValueExtendedProperties</span></span>|<span data-ttu-id="2cff1-245">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2cff1-245">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>|<span data-ttu-id="2cff1-246">为任务定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="2cff1-246">The collection of single-value extended properties defined for the task.</span></span> <span data-ttu-id="2cff1-247">只读。</span><span class="sxs-lookup"><span data-stu-id="2cff1-247">Read-only.</span></span> <span data-ttu-id="2cff1-248">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2cff1-248">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2cff1-249">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cff1-249">JSON representation</span></span>
<span data-ttu-id="2cff1-250">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cff1-250">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktask.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
