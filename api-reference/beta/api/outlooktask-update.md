---
title: 更新 outlooktask
description: 更改 Outlook 任务的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cffd94b7e3d19a0f806116ec81a133878bf43efb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450616"
---
# <a name="update-outlooktask"></a><span data-ttu-id="47173-103">更新 outlooktask</span><span class="sxs-lookup"><span data-stu-id="47173-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47173-104">更改 Outlook 任务的可写属性。</span><span class="sxs-lookup"><span data-stu-id="47173-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="47173-105">**CompletedDateTime**属性可以由**完整**操作进行设置, 也可以通过修补程序操作进行显式设置。</span><span class="sxs-lookup"><span data-stu-id="47173-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="47173-106">如果使用修补程序设置**completedDateTime**, 请确保同时将**状态**设置为`completed` 。</span><span class="sxs-lookup"><span data-stu-id="47173-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="47173-107">默认情况下, 此操作 (以及 POST、GET 和[complete](../api/outlooktask-complete.md)任务操作) 返回 UTC 格式的与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="47173-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="47173-108">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="47173-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="47173-109">权限</span><span class="sxs-lookup"><span data-stu-id="47173-109">Permissions</span></span>

<span data-ttu-id="47173-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47173-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47173-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="47173-112">Permission type</span></span>      | <span data-ttu-id="47173-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47173-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47173-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47173-114">Delegated (work or school account)</span></span> | <span data-ttu-id="47173-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47173-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="47173-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47173-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47173-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47173-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="47173-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="47173-118">Application</span></span> | <span data-ttu-id="47173-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="47173-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47173-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47173-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="47173-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="47173-121">Request headers</span></span>

| <span data-ttu-id="47173-122">名称</span><span class="sxs-lookup"><span data-stu-id="47173-122">Name</span></span>       | <span data-ttu-id="47173-123">说明</span><span class="sxs-lookup"><span data-stu-id="47173-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="47173-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47173-124">Authorization</span></span>  | <span data-ttu-id="47173-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47173-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47173-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="47173-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="47173-128">指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。</span><span class="sxs-lookup"><span data-stu-id="47173-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="47173-129">可选。</span><span class="sxs-lookup"><span data-stu-id="47173-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47173-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="47173-130">Request body</span></span>

<span data-ttu-id="47173-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="47173-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="47173-134">属性</span><span class="sxs-lookup"><span data-stu-id="47173-134">Property</span></span> | <span data-ttu-id="47173-135">类型</span><span class="sxs-lookup"><span data-stu-id="47173-135">Type</span></span> | <span data-ttu-id="47173-136">说明</span><span class="sxs-lookup"><span data-stu-id="47173-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="47173-137">body</span><span class="sxs-lookup"><span data-stu-id="47173-137">body</span></span>|[<span data-ttu-id="47173-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="47173-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="47173-139">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="47173-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="47173-140">请注意，仅支持 HTML 类型。</span><span class="sxs-lookup"><span data-stu-id="47173-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="47173-141">类别</span><span class="sxs-lookup"><span data-stu-id="47173-141">categories</span></span>|<span data-ttu-id="47173-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="47173-142">String collection</span></span>|<span data-ttu-id="47173-143">与任务关联的类别。</span><span class="sxs-lookup"><span data-stu-id="47173-143">The categories associated with the task.</span></span>|
|<span data-ttu-id="47173-144">changeKey</span><span class="sxs-lookup"><span data-stu-id="47173-144">changeKey</span></span>|<span data-ttu-id="47173-145">String</span><span class="sxs-lookup"><span data-stu-id="47173-145">String</span></span>|<span data-ttu-id="47173-146">任务的版本。</span><span class="sxs-lookup"><span data-stu-id="47173-146">The version of the task.</span></span>|
|<span data-ttu-id="47173-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="47173-147">completedDateTime</span></span>|[<span data-ttu-id="47173-148">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="47173-148">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="47173-149">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="47173-149">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="47173-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47173-150">createdDateTime</span></span>|<span data-ttu-id="47173-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47173-151">DateTimeOffset</span></span>|<span data-ttu-id="47173-152">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="47173-152">The date and time when the task was created.</span></span> <span data-ttu-id="47173-153">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="47173-153">By default, it is in UTC.</span></span> <span data-ttu-id="47173-154">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="47173-154">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="47173-155">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="47173-155">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="47173-156">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="47173-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="47173-157">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="47173-157">dueDateTime</span></span>|[<span data-ttu-id="47173-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="47173-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="47173-159">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="47173-159">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="47173-160">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="47173-160">hasAttachments</span></span>|<span data-ttu-id="47173-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="47173-161">Boolean</span></span>|<span data-ttu-id="47173-162">如果任务包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="47173-162">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="47173-163">重要性</span><span class="sxs-lookup"><span data-stu-id="47173-163">importance</span></span>|<span data-ttu-id="47173-164">string</span><span class="sxs-lookup"><span data-stu-id="47173-164">string</span></span>|<span data-ttu-id="47173-165">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="47173-165">The importance of the event.</span></span> <span data-ttu-id="47173-166">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="47173-166">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="47173-167">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="47173-167">isReminderOn</span></span>|<span data-ttu-id="47173-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="47173-168">Boolean</span></span>|<span data-ttu-id="47173-169">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="47173-169">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="47173-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47173-170">lastModifiedDateTime</span></span>|<span data-ttu-id="47173-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47173-171">DateTimeOffset</span></span>|<span data-ttu-id="47173-172">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="47173-172">The date and time when the task was last modified.</span></span> <span data-ttu-id="47173-173">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="47173-173">By default, it is in UTC.</span></span> <span data-ttu-id="47173-174">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="47173-174">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="47173-175">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="47173-175">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="47173-176">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="47173-176">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="47173-177">所有者</span><span class="sxs-lookup"><span data-stu-id="47173-177">owner</span></span>|<span data-ttu-id="47173-178">字符串</span><span class="sxs-lookup"><span data-stu-id="47173-178">String</span></span>|<span data-ttu-id="47173-179">任务创建者的姓名。</span><span class="sxs-lookup"><span data-stu-id="47173-179">The name of the person who created the task.</span></span>|
|<span data-ttu-id="47173-180">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="47173-180">parentFolderId</span></span>|<span data-ttu-id="47173-181">String</span><span class="sxs-lookup"><span data-stu-id="47173-181">String</span></span>|<span data-ttu-id="47173-182">任务的父文件夹的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="47173-182">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="47173-183">定期</span><span class="sxs-lookup"><span data-stu-id="47173-183">recurrence</span></span>|[<span data-ttu-id="47173-184">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="47173-184">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="47173-185">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="47173-185">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="47173-186">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="47173-186">reminderDateTime</span></span>|[<span data-ttu-id="47173-187">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="47173-187">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="47173-188">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="47173-188">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="47173-189">敏感度</span><span class="sxs-lookup"><span data-stu-id="47173-189">sensitivity</span></span>|<span data-ttu-id="47173-190">string</span><span class="sxs-lookup"><span data-stu-id="47173-190">string</span></span>|<span data-ttu-id="47173-191">指示任务的隐私级别。</span><span class="sxs-lookup"><span data-stu-id="47173-191">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="47173-192">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="47173-192">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="47173-193">startDateTime</span><span class="sxs-lookup"><span data-stu-id="47173-193">startDateTime</span></span>|[<span data-ttu-id="47173-194">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="47173-194">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="47173-195">要在指定时区内开始执行任务的日期。</span><span class="sxs-lookup"><span data-stu-id="47173-195">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="47173-196">状态</span><span class="sxs-lookup"><span data-stu-id="47173-196">status</span></span>|<span data-ttu-id="47173-197">string</span><span class="sxs-lookup"><span data-stu-id="47173-197">string</span></span>|<span data-ttu-id="47173-198">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="47173-198">Indicates the state or progress of the task.</span></span> <span data-ttu-id="47173-199">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="47173-199">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="47173-200">主题</span><span class="sxs-lookup"><span data-stu-id="47173-200">subject</span></span>|<span data-ttu-id="47173-201">String</span><span class="sxs-lookup"><span data-stu-id="47173-201">String</span></span>|<span data-ttu-id="47173-202">任务的简要说明或标题。</span><span class="sxs-lookup"><span data-stu-id="47173-202">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="47173-203">响应</span><span class="sxs-lookup"><span data-stu-id="47173-203">Response</span></span>

<span data-ttu-id="47173-204">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47173-204">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47173-205">示例</span><span class="sxs-lookup"><span data-stu-id="47173-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="47173-206">请求</span><span class="sxs-lookup"><span data-stu-id="47173-206">Request</span></span>

<span data-ttu-id="47173-207">下面的示例修改**dueDateTime**属性, 并使用`Prefer: outlook.timezone`头指定表示以东部标准时间 (EST) 响应中与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="47173-207">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="47173-208">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="47173-208">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="47173-209">C#</span><span class="sxs-lookup"><span data-stu-id="47173-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47173-210">Javascript</span><span class="sxs-lookup"><span data-stu-id="47173-210">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47173-211">目标-C</span><span class="sxs-lookup"><span data-stu-id="47173-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47173-212">响应</span><span class="sxs-lookup"><span data-stu-id="47173-212">Response</span></span>

<span data-ttu-id="47173-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47173-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
