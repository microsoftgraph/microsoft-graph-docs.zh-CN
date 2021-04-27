---
title: 更新 outlooktask
description: 更改任务任务的可写Outlook属性。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 04fbf6862914b8ddcb1086197a0284fd482cbb53
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055461"
---
# <a name="update-outlooktask-deprecated"></a><span data-ttu-id="9d2a8-103">更新 outlooktask (已弃) </span><span class="sxs-lookup"><span data-stu-id="9d2a8-103">Update outlooktask (deprecated)</span></span>

<span data-ttu-id="9d2a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d2a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="9d2a8-105">更改任务任务的可写Outlook属性。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-105">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="9d2a8-106">**completedDateTime** 属性可通过完整操作设置，也可通过 PATCH 操作显式设置。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-106">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="9d2a8-107">如果使用 PATCH 设置 **completedDateTime，** 请确保同时将 **状态** 设置为 `completed` 。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-107">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="9d2a8-108">默认情况下，此操作 (POST、GET 和 [complete](../api/outlooktask-complete.md) 任务操作) UTC 格式返回与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-108">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="9d2a8-109">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d2a8-110">权限</span><span class="sxs-lookup"><span data-stu-id="9d2a8-110">Permissions</span></span>

<span data-ttu-id="9d2a8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d2a8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d2a8-113">Permission type</span></span>      | <span data-ttu-id="9d2a8-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d2a8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d2a8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d2a8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9d2a8-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d2a8-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9d2a8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d2a8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d2a8-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d2a8-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9d2a8-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d2a8-119">Application</span></span> | <span data-ttu-id="9d2a8-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d2a8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d2a8-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d2a8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d2a8-122">Request headers</span></span>

| <span data-ttu-id="9d2a8-123">名称</span><span class="sxs-lookup"><span data-stu-id="9d2a8-123">Name</span></span>       | <span data-ttu-id="9d2a8-124">说明</span><span class="sxs-lookup"><span data-stu-id="9d2a8-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d2a8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d2a8-125">Authorization</span></span>  | <span data-ttu-id="9d2a8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d2a8-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9d2a8-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="9d2a8-129">指定响应中时间属性的时区，如果未指定此标头，则其时区为 UTC。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="9d2a8-130">可选。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d2a8-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d2a8-131">Request body</span></span>

<span data-ttu-id="9d2a8-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d2a8-135">属性</span><span class="sxs-lookup"><span data-stu-id="9d2a8-135">Property</span></span> | <span data-ttu-id="9d2a8-136">类型</span><span class="sxs-lookup"><span data-stu-id="9d2a8-136">Type</span></span> | <span data-ttu-id="9d2a8-137">说明</span><span class="sxs-lookup"><span data-stu-id="9d2a8-137">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9d2a8-138">body</span><span class="sxs-lookup"><span data-stu-id="9d2a8-138">body</span></span>|[<span data-ttu-id="9d2a8-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="9d2a8-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="9d2a8-140">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-140">The task body that typically contains information about the task.</span></span> <span data-ttu-id="9d2a8-141">请注意，仅支持 HTML 类型。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-141">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="9d2a8-142">类别</span><span class="sxs-lookup"><span data-stu-id="9d2a8-142">categories</span></span>|<span data-ttu-id="9d2a8-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="9d2a8-143">String collection</span></span>|<span data-ttu-id="9d2a8-144">与任务关联的类别。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-144">The categories associated with the task.</span></span>|
|<span data-ttu-id="9d2a8-145">changeKey</span><span class="sxs-lookup"><span data-stu-id="9d2a8-145">changeKey</span></span>|<span data-ttu-id="9d2a8-146">String</span><span class="sxs-lookup"><span data-stu-id="9d2a8-146">String</span></span>|<span data-ttu-id="9d2a8-147">任务的版本。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-147">The version of the task.</span></span>|
|<span data-ttu-id="9d2a8-148">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d2a8-148">completedDateTime</span></span>|[<span data-ttu-id="9d2a8-149">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d2a8-149">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d2a8-150">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-150">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="9d2a8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d2a8-151">createdDateTime</span></span>|<span data-ttu-id="9d2a8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d2a8-152">DateTimeOffset</span></span>|<span data-ttu-id="9d2a8-153">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-153">The date and time when the task was created.</span></span> <span data-ttu-id="9d2a8-154">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-154">By default, it is in UTC.</span></span> <span data-ttu-id="9d2a8-155">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-155">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="9d2a8-156">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-156">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="9d2a8-157">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="9d2a8-158">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="9d2a8-158">dueDateTime</span></span>|[<span data-ttu-id="9d2a8-159">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d2a8-159">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d2a8-160">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-160">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="9d2a8-161">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="9d2a8-161">hasAttachments</span></span>|<span data-ttu-id="9d2a8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d2a8-162">Boolean</span></span>|<span data-ttu-id="9d2a8-163">如果任务包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-163">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="9d2a8-164">importance</span><span class="sxs-lookup"><span data-stu-id="9d2a8-164">importance</span></span>|<span data-ttu-id="9d2a8-165">string</span><span class="sxs-lookup"><span data-stu-id="9d2a8-165">string</span></span>|<span data-ttu-id="9d2a8-166">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-166">The importance of the event.</span></span> <span data-ttu-id="9d2a8-167">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-167">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="9d2a8-168">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="9d2a8-168">isReminderOn</span></span>|<span data-ttu-id="9d2a8-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d2a8-169">Boolean</span></span>|<span data-ttu-id="9d2a8-170">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-170">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="9d2a8-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d2a8-171">lastModifiedDateTime</span></span>|<span data-ttu-id="9d2a8-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d2a8-172">DateTimeOffset</span></span>|<span data-ttu-id="9d2a8-173">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-173">The date and time when the task was last modified.</span></span> <span data-ttu-id="9d2a8-174">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-174">By default, it is in UTC.</span></span> <span data-ttu-id="9d2a8-175">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-175">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="9d2a8-176">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-176">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9d2a8-177">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-177">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="9d2a8-178">Owner</span><span class="sxs-lookup"><span data-stu-id="9d2a8-178">owner</span></span>|<span data-ttu-id="9d2a8-179">String</span><span class="sxs-lookup"><span data-stu-id="9d2a8-179">String</span></span>|<span data-ttu-id="9d2a8-180">任务创建者的姓名。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-180">The name of the person who created the task.</span></span>|
|<span data-ttu-id="9d2a8-181">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="9d2a8-181">parentFolderId</span></span>|<span data-ttu-id="9d2a8-182">String</span><span class="sxs-lookup"><span data-stu-id="9d2a8-182">String</span></span>|<span data-ttu-id="9d2a8-183">任务的父文件夹的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-183">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="9d2a8-184">定期</span><span class="sxs-lookup"><span data-stu-id="9d2a8-184">recurrence</span></span>|[<span data-ttu-id="9d2a8-185">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d2a8-185">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="9d2a8-186">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-186">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="9d2a8-187">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="9d2a8-187">reminderDateTime</span></span>|[<span data-ttu-id="9d2a8-188">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d2a8-188">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d2a8-189">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-189">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="9d2a8-190">敏感度</span><span class="sxs-lookup"><span data-stu-id="9d2a8-190">sensitivity</span></span>|<span data-ttu-id="9d2a8-191">string</span><span class="sxs-lookup"><span data-stu-id="9d2a8-191">string</span></span>|<span data-ttu-id="9d2a8-192">指示任务的隐私级别。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-192">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="9d2a8-193">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-193">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="9d2a8-194">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9d2a8-194">startDateTime</span></span>|[<span data-ttu-id="9d2a8-195">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d2a8-195">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="9d2a8-196">要在指定时区内开始执行任务的日期。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-196">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="9d2a8-197">状态</span><span class="sxs-lookup"><span data-stu-id="9d2a8-197">status</span></span>|<span data-ttu-id="9d2a8-198">string</span><span class="sxs-lookup"><span data-stu-id="9d2a8-198">string</span></span>|<span data-ttu-id="9d2a8-199">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-199">Indicates the state or progress of the task.</span></span> <span data-ttu-id="9d2a8-200">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-200">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="9d2a8-201">主题</span><span class="sxs-lookup"><span data-stu-id="9d2a8-201">subject</span></span>|<span data-ttu-id="9d2a8-202">String</span><span class="sxs-lookup"><span data-stu-id="9d2a8-202">String</span></span>|<span data-ttu-id="9d2a8-203">任务的简要说明或标题。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-203">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="9d2a8-204">响应</span><span class="sxs-lookup"><span data-stu-id="9d2a8-204">Response</span></span>

<span data-ttu-id="9d2a8-205">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [outlookTask](../resources/outlooktask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-205">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d2a8-206">示例</span><span class="sxs-lookup"><span data-stu-id="9d2a8-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d2a8-207">请求</span><span class="sxs-lookup"><span data-stu-id="9d2a8-207">Request</span></span>

<span data-ttu-id="9d2a8-208">下面的示例修改 **dueDateTime** 属性，并使用 标头指定在东部标准时间 (EST 响应中表示与日期相关的 `Prefer: outlook.timezone`) 。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-208">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>

# <a name="http"></a>[<span data-ttu-id="9d2a8-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d2a8-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTHgwAAA=
Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9d2a8-210">C#</span><span class="sxs-lookup"><span data-stu-id="9d2a8-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d2a8-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d2a8-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d2a8-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d2a8-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d2a8-213">Java</span><span class="sxs-lookup"><span data-stu-id="9d2a8-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d2a8-214">响应</span><span class="sxs-lookup"><span data-stu-id="9d2a8-214">Response</span></span>

<span data-ttu-id="9d2a8-215">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-215">Here is an example of the response.</span></span> <span data-ttu-id="9d2a8-216">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9d2a8-216">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "hasAttachments":false,
    "importance": "normal",
    "isReminderOn": false,
    "owner": "Administrator",
    "parentFolderId": "AQMkADA1MTIBEgAAAA==",
    "recurrence": null,
    "reminderDateTime": null,
    "sensitivity": "normal",
    "startDateTime": {
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "status": "notStarted",
    "subject": "Shop for children's weekend"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


