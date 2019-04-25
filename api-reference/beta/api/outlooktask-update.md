---
title: 更新 outlooktask
description: 更改 Outlook 任务的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1908d9b918b13f87b1d5ab61dab912577f06da64
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539792"
---
# <a name="update-outlooktask"></a><span data-ttu-id="641b8-103">更新 outlooktask</span><span class="sxs-lookup"><span data-stu-id="641b8-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="641b8-104">更改 Outlook 任务的可写属性。</span><span class="sxs-lookup"><span data-stu-id="641b8-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="641b8-105">**completedDateTime**属性可以由**完整**操作进行设置, 也可以通过修补程序操作进行显式设置。</span><span class="sxs-lookup"><span data-stu-id="641b8-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="641b8-106">如果使用修补程序设置**completedDateTime**, 请确保同时将**状态**设置为`completed` 。</span><span class="sxs-lookup"><span data-stu-id="641b8-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="641b8-107">默认情况下, 此操作 (以及 POST、GET 和[complete](../api/outlooktask-complete.md)任务操作) 返回 UTC 格式的与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="641b8-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="641b8-108">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="641b8-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="641b8-109">权限</span><span class="sxs-lookup"><span data-stu-id="641b8-109">Permissions</span></span>

<span data-ttu-id="641b8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="641b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="641b8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="641b8-112">Permission type</span></span>      | <span data-ttu-id="641b8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="641b8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="641b8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="641b8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="641b8-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="641b8-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="641b8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="641b8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="641b8-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="641b8-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="641b8-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="641b8-118">Application</span></span> | <span data-ttu-id="641b8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="641b8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="641b8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="641b8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="641b8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="641b8-121">Request headers</span></span>

| <span data-ttu-id="641b8-122">名称</span><span class="sxs-lookup"><span data-stu-id="641b8-122">Name</span></span>       | <span data-ttu-id="641b8-123">说明</span><span class="sxs-lookup"><span data-stu-id="641b8-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="641b8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="641b8-124">Authorization</span></span>  | <span data-ttu-id="641b8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="641b8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="641b8-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="641b8-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="641b8-128">指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。</span><span class="sxs-lookup"><span data-stu-id="641b8-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="641b8-129">可选。</span><span class="sxs-lookup"><span data-stu-id="641b8-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="641b8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="641b8-130">Request body</span></span>

<span data-ttu-id="641b8-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="641b8-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="641b8-134">属性</span><span class="sxs-lookup"><span data-stu-id="641b8-134">Property</span></span> | <span data-ttu-id="641b8-135">类型</span><span class="sxs-lookup"><span data-stu-id="641b8-135">Type</span></span> | <span data-ttu-id="641b8-136">说明</span><span class="sxs-lookup"><span data-stu-id="641b8-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="641b8-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="641b8-137">assignedTo</span></span>|<span data-ttu-id="641b8-138">String</span><span class="sxs-lookup"><span data-stu-id="641b8-138">String</span></span>|<span data-ttu-id="641b8-139">已为其分配任务的人员姓名。</span><span class="sxs-lookup"><span data-stu-id="641b8-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="641b8-140">body</span><span class="sxs-lookup"><span data-stu-id="641b8-140">body</span></span>|[<span data-ttu-id="641b8-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="641b8-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="641b8-142">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="641b8-142">The task body that typically contains information about the task.</span></span> <span data-ttu-id="641b8-143">请注意，仅支持 HTML 类型。</span><span class="sxs-lookup"><span data-stu-id="641b8-143">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="641b8-144">categories</span><span class="sxs-lookup"><span data-stu-id="641b8-144">categories</span></span>|<span data-ttu-id="641b8-145">String collection</span><span class="sxs-lookup"><span data-stu-id="641b8-145">String collection</span></span>|<span data-ttu-id="641b8-146">与任务关联的类别。</span><span class="sxs-lookup"><span data-stu-id="641b8-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="641b8-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="641b8-147">changeKey</span></span>|<span data-ttu-id="641b8-148">String</span><span class="sxs-lookup"><span data-stu-id="641b8-148">String</span></span>|<span data-ttu-id="641b8-149">任务的版本。</span><span class="sxs-lookup"><span data-stu-id="641b8-149">The version of the task.</span></span>|
|<span data-ttu-id="641b8-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="641b8-150">completedDateTime</span></span>|[<span data-ttu-id="641b8-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="641b8-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="641b8-152">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="641b8-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="641b8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="641b8-153">createdDateTime</span></span>|<span data-ttu-id="641b8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="641b8-154">DateTimeOffset</span></span>|<span data-ttu-id="641b8-155">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="641b8-155">The date and time when the task was created.</span></span> <span data-ttu-id="641b8-156">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="641b8-156">By default, it is in UTC.</span></span> <span data-ttu-id="641b8-157">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="641b8-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="641b8-158">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="641b8-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="641b8-159">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="641b8-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="641b8-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="641b8-160">dueDateTime</span></span>|[<span data-ttu-id="641b8-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="641b8-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="641b8-162">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="641b8-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="641b8-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="641b8-163">hasAttachments</span></span>|<span data-ttu-id="641b8-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="641b8-164">Boolean</span></span>|<span data-ttu-id="641b8-165">如果任务包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="641b8-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="641b8-166">重要性</span><span class="sxs-lookup"><span data-stu-id="641b8-166">importance</span></span>|<span data-ttu-id="641b8-167">string</span><span class="sxs-lookup"><span data-stu-id="641b8-167">string</span></span>|<span data-ttu-id="641b8-168">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="641b8-168">The importance of the event.</span></span> <span data-ttu-id="641b8-169">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="641b8-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="641b8-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="641b8-170">isReminderOn</span></span>|<span data-ttu-id="641b8-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="641b8-171">Boolean</span></span>|<span data-ttu-id="641b8-172">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="641b8-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="641b8-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="641b8-173">lastModifiedDateTime</span></span>|<span data-ttu-id="641b8-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="641b8-174">DateTimeOffset</span></span>|<span data-ttu-id="641b8-175">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="641b8-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="641b8-176">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="641b8-176">By default, it is in UTC.</span></span> <span data-ttu-id="641b8-177">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="641b8-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="641b8-178">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="641b8-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="641b8-179">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="641b8-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="641b8-180">所有者</span><span class="sxs-lookup"><span data-stu-id="641b8-180">owner</span></span>|<span data-ttu-id="641b8-181">字符串</span><span class="sxs-lookup"><span data-stu-id="641b8-181">String</span></span>|<span data-ttu-id="641b8-182">任务创建者的姓名。</span><span class="sxs-lookup"><span data-stu-id="641b8-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="641b8-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="641b8-183">parentFolderId</span></span>|<span data-ttu-id="641b8-184">String</span><span class="sxs-lookup"><span data-stu-id="641b8-184">String</span></span>|<span data-ttu-id="641b8-185">任务的父文件夹的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="641b8-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="641b8-186">定期</span><span class="sxs-lookup"><span data-stu-id="641b8-186">recurrence</span></span>|[<span data-ttu-id="641b8-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="641b8-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="641b8-188">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="641b8-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="641b8-189">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="641b8-189">reminderDateTime</span></span>|[<span data-ttu-id="641b8-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="641b8-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="641b8-191">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="641b8-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="641b8-192">敏感度</span><span class="sxs-lookup"><span data-stu-id="641b8-192">sensitivity</span></span>|<span data-ttu-id="641b8-193">string</span><span class="sxs-lookup"><span data-stu-id="641b8-193">string</span></span>|<span data-ttu-id="641b8-194">指示任务的隐私级别。</span><span class="sxs-lookup"><span data-stu-id="641b8-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="641b8-195">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="641b8-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="641b8-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="641b8-196">startDateTime</span></span>|[<span data-ttu-id="641b8-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="641b8-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="641b8-198">要在指定时区内开始执行任务的日期。</span><span class="sxs-lookup"><span data-stu-id="641b8-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="641b8-199">状态</span><span class="sxs-lookup"><span data-stu-id="641b8-199">status</span></span>|<span data-ttu-id="641b8-200">string</span><span class="sxs-lookup"><span data-stu-id="641b8-200">string</span></span>|<span data-ttu-id="641b8-201">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="641b8-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="641b8-202">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="641b8-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="641b8-203">subject</span><span class="sxs-lookup"><span data-stu-id="641b8-203">subject</span></span>|<span data-ttu-id="641b8-204">String</span><span class="sxs-lookup"><span data-stu-id="641b8-204">String</span></span>|<span data-ttu-id="641b8-205">任务的简要说明或标题。</span><span class="sxs-lookup"><span data-stu-id="641b8-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="641b8-206">响应</span><span class="sxs-lookup"><span data-stu-id="641b8-206">Response</span></span>

<span data-ttu-id="641b8-207">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="641b8-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="641b8-208">示例</span><span class="sxs-lookup"><span data-stu-id="641b8-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="641b8-209">请求</span><span class="sxs-lookup"><span data-stu-id="641b8-209">Request</span></span>

<span data-ttu-id="641b8-210">下面的示例修改**dueDateTime**属性, 并使用`Prefer: outlook.timezone`头指定表示以东部标准时间 (EST) 响应中与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="641b8-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
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

### <a name="response"></a><span data-ttu-id="641b8-211">响应</span><span class="sxs-lookup"><span data-stu-id="641b8-211">Response</span></span>

<span data-ttu-id="641b8-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="641b8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/outlooktask-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
