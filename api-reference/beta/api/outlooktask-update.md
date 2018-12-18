---
title: 更新 outlooktask
description: 更改 Outlook 任务的可写属性。
author: angelgolfer-ms
ms.openlocfilehash: 0a162c81ef32cb35e930b000678234ede20e4874
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325702"
---
# <a name="update-outlooktask"></a><span data-ttu-id="300f4-103">更新 outlooktask</span><span class="sxs-lookup"><span data-stu-id="300f4-103">Update outlooktask</span></span>

> <span data-ttu-id="300f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="300f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="300f4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="300f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="300f4-106">更改 Outlook 任务的可写属性。</span><span class="sxs-lookup"><span data-stu-id="300f4-106">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="300f4-107">通过**完成**操作，或明确的修补程序操作，可以设置**completedDateTime**属性。</span><span class="sxs-lookup"><span data-stu-id="300f4-107">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="300f4-108">如果您使用的修补程序设置**completedDateTime**，请确保将**状态**设置为`completed`以及。</span><span class="sxs-lookup"><span data-stu-id="300f4-108">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="300f4-109">默认情况下，此操作 （和文章、 GET，和[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="300f4-109">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="300f4-110">您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="300f4-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="300f4-111">权限</span><span class="sxs-lookup"><span data-stu-id="300f4-111">Permissions</span></span>
<span data-ttu-id="300f4-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="300f4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="300f4-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="300f4-114">Permission type</span></span>      | <span data-ttu-id="300f4-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="300f4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="300f4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="300f4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="300f4-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="300f4-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="300f4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="300f4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="300f4-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="300f4-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="300f4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="300f4-120">Application</span></span> | <span data-ttu-id="300f4-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="300f4-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="300f4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="300f4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="300f4-123">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="300f4-123">Optional request headers</span></span>
| <span data-ttu-id="300f4-124">Name</span><span class="sxs-lookup"><span data-stu-id="300f4-124">Name</span></span>       | <span data-ttu-id="300f4-125">说明</span><span class="sxs-lookup"><span data-stu-id="300f4-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="300f4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="300f4-126">Authorization</span></span>  | <span data-ttu-id="300f4-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="300f4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="300f4-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="300f4-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="300f4-130">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="300f4-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="300f4-131">可选。</span><span class="sxs-lookup"><span data-stu-id="300f4-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="300f4-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="300f4-132">Request body</span></span>
<span data-ttu-id="300f4-p107">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="300f4-p107">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="300f4-136">属性</span><span class="sxs-lookup"><span data-stu-id="300f4-136">Property</span></span>     | <span data-ttu-id="300f4-137">类型</span><span class="sxs-lookup"><span data-stu-id="300f4-137">Type</span></span>   |<span data-ttu-id="300f4-138">说明</span><span class="sxs-lookup"><span data-stu-id="300f4-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="300f4-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="300f4-139">assignedTo</span></span>|<span data-ttu-id="300f4-140">字符串</span><span class="sxs-lookup"><span data-stu-id="300f4-140">String</span></span>|<span data-ttu-id="300f4-141">已分配任务的人员的名称。</span><span class="sxs-lookup"><span data-stu-id="300f4-141">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="300f4-142">body</span><span class="sxs-lookup"><span data-stu-id="300f4-142">body</span></span>|[<span data-ttu-id="300f4-143">itemBody</span><span class="sxs-lookup"><span data-stu-id="300f4-143">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="300f4-144">任务正文通常包含有关任务的信息。</span><span class="sxs-lookup"><span data-stu-id="300f4-144">The task body that typically contains information about the task.</span></span> <span data-ttu-id="300f4-145">请注意，仅 HTML 支持类型。</span><span class="sxs-lookup"><span data-stu-id="300f4-145">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="300f4-146">categories</span><span class="sxs-lookup"><span data-stu-id="300f4-146">categories</span></span>|<span data-ttu-id="300f4-147">String collection</span><span class="sxs-lookup"><span data-stu-id="300f4-147">String collection</span></span>|<span data-ttu-id="300f4-148">类别与任务关联。</span><span class="sxs-lookup"><span data-stu-id="300f4-148">The categories associated with the task.</span></span>|
|<span data-ttu-id="300f4-149">changeKey</span><span class="sxs-lookup"><span data-stu-id="300f4-149">changeKey</span></span>|<span data-ttu-id="300f4-150">字符串</span><span class="sxs-lookup"><span data-stu-id="300f4-150">String</span></span>|<span data-ttu-id="300f4-151">任务的版本。</span><span class="sxs-lookup"><span data-stu-id="300f4-151">The version of the task.</span></span>|
|<span data-ttu-id="300f4-152">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="300f4-152">completedDateTime</span></span>|[<span data-ttu-id="300f4-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="300f4-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="300f4-154">中指定的时区任务已完成的日期。</span><span class="sxs-lookup"><span data-stu-id="300f4-154">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="300f4-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="300f4-155">createdDateTime</span></span>|<span data-ttu-id="300f4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="300f4-156">DateTimeOffset</span></span>|<span data-ttu-id="300f4-157">日期和时间创建任务时。</span><span class="sxs-lookup"><span data-stu-id="300f4-157">The date and time when the task was created.</span></span> <span data-ttu-id="300f4-158">默认情况下，它是采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="300f4-158">By default, it is in UTC.</span></span> <span data-ttu-id="300f4-159">您可以提供请求标头中自定义时区。</span><span class="sxs-lookup"><span data-stu-id="300f4-159">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="300f4-160">该属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="300f4-160">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="300f4-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="300f4-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="300f4-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="300f4-162">dueDateTime</span></span>|[<span data-ttu-id="300f4-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="300f4-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="300f4-164">在指定时区的任务完成日期。</span><span class="sxs-lookup"><span data-stu-id="300f4-164">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="300f4-165">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="300f4-165">hasAttachments</span></span>|<span data-ttu-id="300f4-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="300f4-166">Boolean</span></span>|<span data-ttu-id="300f4-167">设置为 true 如果任务的附件。</span><span class="sxs-lookup"><span data-stu-id="300f4-167">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="300f4-168">importance</span><span class="sxs-lookup"><span data-stu-id="300f4-168">importance</span></span>|<span data-ttu-id="300f4-169">string</span><span class="sxs-lookup"><span data-stu-id="300f4-169">string</span></span>|<span data-ttu-id="300f4-170">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="300f4-170">The importance of the event.</span></span> <span data-ttu-id="300f4-171">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="300f4-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="300f4-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="300f4-172">isReminderOn</span></span>|<span data-ttu-id="300f4-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="300f4-173">Boolean</span></span>|<span data-ttu-id="300f4-174">如果，设置为 true 设置通知提醒的用户的任务。</span><span class="sxs-lookup"><span data-stu-id="300f4-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="300f4-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="300f4-175">lastModifiedDateTime</span></span>|<span data-ttu-id="300f4-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="300f4-176">DateTimeOffset</span></span>|<span data-ttu-id="300f4-177">日期和上次修改任务的时间。</span><span class="sxs-lookup"><span data-stu-id="300f4-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="300f4-178">默认情况下，它是采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="300f4-178">By default, it is in UTC.</span></span> <span data-ttu-id="300f4-179">您可以提供请求标头中自定义时区。</span><span class="sxs-lookup"><span data-stu-id="300f4-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="300f4-180">该属性值使用 ISO 8601 格式，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="300f4-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="300f4-181">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="300f4-181">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="300f4-182">owner</span><span class="sxs-lookup"><span data-stu-id="300f4-182">owner</span></span>|<span data-ttu-id="300f4-183">字符串</span><span class="sxs-lookup"><span data-stu-id="300f4-183">String</span></span>|<span data-ttu-id="300f4-184">创建任务的人员的名称。</span><span class="sxs-lookup"><span data-stu-id="300f4-184">The name of the person who created the task.</span></span>|
|<span data-ttu-id="300f4-185">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="300f4-185">parentFolderId</span></span>|<span data-ttu-id="300f4-186">String</span><span class="sxs-lookup"><span data-stu-id="300f4-186">String</span></span>|<span data-ttu-id="300f4-187">任务的父文件夹的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="300f4-187">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="300f4-188">recurrence</span><span class="sxs-lookup"><span data-stu-id="300f4-188">recurrence</span></span>|[<span data-ttu-id="300f4-189">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="300f4-189">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="300f4-190">定期模式的任务。</span><span class="sxs-lookup"><span data-stu-id="300f4-190">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="300f4-191">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="300f4-191">reminderDateTime</span></span>|[<span data-ttu-id="300f4-192">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="300f4-192">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="300f4-193">发生的日期和时间的任务的提醒通知。</span><span class="sxs-lookup"><span data-stu-id="300f4-193">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="300f4-194">sensitivity</span><span class="sxs-lookup"><span data-stu-id="300f4-194">sensitivity</span></span>|<span data-ttu-id="300f4-195">string</span><span class="sxs-lookup"><span data-stu-id="300f4-195">string</span></span>|<span data-ttu-id="300f4-196">指示任务的隐私级别。</span><span class="sxs-lookup"><span data-stu-id="300f4-196">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="300f4-197">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="300f4-197">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="300f4-198">startDateTime</span><span class="sxs-lookup"><span data-stu-id="300f4-198">startDateTime</span></span>|[<span data-ttu-id="300f4-199">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="300f4-199">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="300f4-200">在指定时区时的任务是开始日期。</span><span class="sxs-lookup"><span data-stu-id="300f4-200">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="300f4-201">status</span><span class="sxs-lookup"><span data-stu-id="300f4-201">status</span></span>|<span data-ttu-id="300f4-202">string</span><span class="sxs-lookup"><span data-stu-id="300f4-202">string</span></span>|<span data-ttu-id="300f4-203">指示的状态或任务进度。</span><span class="sxs-lookup"><span data-stu-id="300f4-203">Indicates the state or progress of the task.</span></span> <span data-ttu-id="300f4-204">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="300f4-204">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="300f4-205">subject</span><span class="sxs-lookup"><span data-stu-id="300f4-205">subject</span></span>|<span data-ttu-id="300f4-206">字符串</span><span class="sxs-lookup"><span data-stu-id="300f4-206">String</span></span>|<span data-ttu-id="300f4-207">简要说明或任务的标题。</span><span class="sxs-lookup"><span data-stu-id="300f4-207">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="300f4-208">响应</span><span class="sxs-lookup"><span data-stu-id="300f4-208">Response</span></span>

<span data-ttu-id="300f4-209">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="300f4-209">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="300f4-210">示例</span><span class="sxs-lookup"><span data-stu-id="300f4-210">Example</span></span>
##### <a name="request"></a><span data-ttu-id="300f4-211">请求</span><span class="sxs-lookup"><span data-stu-id="300f4-211">Request</span></span>
<span data-ttu-id="300f4-212">下面的示例修改**dueDateTime**属性，并使用`Prefer: outlook.timezone`标头以指定表达东部标准时间 (EST) 的响应中与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="300f4-212">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

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
##### <a name="response"></a><span data-ttu-id="300f4-213">响应</span><span class="sxs-lookup"><span data-stu-id="300f4-213">Response</span></span>
<span data-ttu-id="300f4-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="300f4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->