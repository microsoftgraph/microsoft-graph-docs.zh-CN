---
title: 更新 outlooktask
description: 更改 Outlook 任务的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1908d9b918b13f87b1d5ab61dab912577f06da64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526884"
---
# <a name="update-outlooktask"></a><span data-ttu-id="8e36e-103">更新 outlooktask</span><span class="sxs-lookup"><span data-stu-id="8e36e-103">Update outlooktask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e36e-104">更改 Outlook 任务的可写属性。</span><span class="sxs-lookup"><span data-stu-id="8e36e-104">Change writable properties of an Outlook task.</span></span>

<span data-ttu-id="8e36e-105">通过**完成**操作，或明确的修补程序操作，可以设置**completedDateTime**属性。</span><span class="sxs-lookup"><span data-stu-id="8e36e-105">The **completedDateTime** property can be set by the **complete** action, or explicitly by a PATCH operation.</span></span> <span data-ttu-id="8e36e-106">如果您使用的修补程序设置**completedDateTime**，请确保将**状态**设置为`completed`以及。</span><span class="sxs-lookup"><span data-stu-id="8e36e-106">If you use PATCH to set **completedDateTime**, make sure you set **status** to `completed` as well.</span></span>

<span data-ttu-id="8e36e-107">默认情况下，此操作 （和文章、 GET，和[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="8e36e-107">By default, this operation (and the POST, GET, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="8e36e-108">您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="8e36e-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e36e-109">权限</span><span class="sxs-lookup"><span data-stu-id="8e36e-109">Permissions</span></span>

<span data-ttu-id="8e36e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e36e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e36e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e36e-112">Permission type</span></span>      | <span data-ttu-id="8e36e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e36e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e36e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e36e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8e36e-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e36e-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8e36e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e36e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e36e-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e36e-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8e36e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e36e-118">Application</span></span> | <span data-ttu-id="8e36e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e36e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e36e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e36e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8e36e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e36e-121">Request headers</span></span>

| <span data-ttu-id="8e36e-122">名称</span><span class="sxs-lookup"><span data-stu-id="8e36e-122">Name</span></span>       | <span data-ttu-id="8e36e-123">说明</span><span class="sxs-lookup"><span data-stu-id="8e36e-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8e36e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e36e-124">Authorization</span></span>  | <span data-ttu-id="8e36e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e36e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e36e-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8e36e-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8e36e-128">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="8e36e-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="8e36e-129">可选。</span><span class="sxs-lookup"><span data-stu-id="8e36e-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e36e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e36e-130">Request body</span></span>

<span data-ttu-id="8e36e-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8e36e-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e36e-134">属性</span><span class="sxs-lookup"><span data-stu-id="8e36e-134">Property</span></span> | <span data-ttu-id="8e36e-135">类型</span><span class="sxs-lookup"><span data-stu-id="8e36e-135">Type</span></span> | <span data-ttu-id="8e36e-136">说明</span><span class="sxs-lookup"><span data-stu-id="8e36e-136">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8e36e-137">AssignedTo</span><span class="sxs-lookup"><span data-stu-id="8e36e-137">assignedTo</span></span>|<span data-ttu-id="8e36e-138">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-138">String</span></span>|<span data-ttu-id="8e36e-139">已分配任务的人员的名称。</span><span class="sxs-lookup"><span data-stu-id="8e36e-139">The name of the person who has been assigned the task.</span></span>|
|<span data-ttu-id="8e36e-140">body</span><span class="sxs-lookup"><span data-stu-id="8e36e-140">body</span></span>|[<span data-ttu-id="8e36e-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="8e36e-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="8e36e-142">任务正文通常包含有关任务的信息。</span><span class="sxs-lookup"><span data-stu-id="8e36e-142">The task body that typically contains information about the task.</span></span> <span data-ttu-id="8e36e-143">请注意，仅 HTML 支持类型。</span><span class="sxs-lookup"><span data-stu-id="8e36e-143">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="8e36e-144">categories</span><span class="sxs-lookup"><span data-stu-id="8e36e-144">categories</span></span>|<span data-ttu-id="8e36e-145">String collection</span><span class="sxs-lookup"><span data-stu-id="8e36e-145">String collection</span></span>|<span data-ttu-id="8e36e-146">类别与任务关联。</span><span class="sxs-lookup"><span data-stu-id="8e36e-146">The categories associated with the task.</span></span>|
|<span data-ttu-id="8e36e-147">changeKey</span><span class="sxs-lookup"><span data-stu-id="8e36e-147">changeKey</span></span>|<span data-ttu-id="8e36e-148">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-148">String</span></span>|<span data-ttu-id="8e36e-149">任务的版本。</span><span class="sxs-lookup"><span data-stu-id="8e36e-149">The version of the task.</span></span>|
|<span data-ttu-id="8e36e-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e36e-150">completedDateTime</span></span>|[<span data-ttu-id="8e36e-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8e36e-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="8e36e-152">中指定的时区任务已完成的日期。</span><span class="sxs-lookup"><span data-stu-id="8e36e-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="8e36e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e36e-153">createdDateTime</span></span>|<span data-ttu-id="8e36e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e36e-154">DateTimeOffset</span></span>|<span data-ttu-id="8e36e-155">日期和时间创建任务时。</span><span class="sxs-lookup"><span data-stu-id="8e36e-155">The date and time when the task was created.</span></span> <span data-ttu-id="8e36e-156">默认情况下，它是采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="8e36e-156">By default, it is in UTC.</span></span> <span data-ttu-id="8e36e-157">您可以提供请求标头中自定义时区。</span><span class="sxs-lookup"><span data-stu-id="8e36e-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="8e36e-158">该属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="8e36e-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="8e36e-159">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8e36e-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8e36e-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="8e36e-160">dueDateTime</span></span>|[<span data-ttu-id="8e36e-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8e36e-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="8e36e-162">在指定时区的任务完成日期。</span><span class="sxs-lookup"><span data-stu-id="8e36e-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="8e36e-163">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="8e36e-163">hasAttachments</span></span>|<span data-ttu-id="8e36e-164">布尔</span><span class="sxs-lookup"><span data-stu-id="8e36e-164">Boolean</span></span>|<span data-ttu-id="8e36e-165">设置为 true 如果任务的附件。</span><span class="sxs-lookup"><span data-stu-id="8e36e-165">Set to true if the task has attachments.</span></span>|
|<span data-ttu-id="8e36e-166">importance</span><span class="sxs-lookup"><span data-stu-id="8e36e-166">importance</span></span>|<span data-ttu-id="8e36e-167">string</span><span class="sxs-lookup"><span data-stu-id="8e36e-167">string</span></span>|<span data-ttu-id="8e36e-168">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="8e36e-168">The importance of the event.</span></span> <span data-ttu-id="8e36e-169">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="8e36e-169">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="8e36e-170">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="8e36e-170">isReminderOn</span></span>|<span data-ttu-id="8e36e-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e36e-171">Boolean</span></span>|<span data-ttu-id="8e36e-172">如果，设置为 true 设置通知提醒的用户的任务。</span><span class="sxs-lookup"><span data-stu-id="8e36e-172">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="8e36e-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e36e-173">lastModifiedDateTime</span></span>|<span data-ttu-id="8e36e-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e36e-174">DateTimeOffset</span></span>|<span data-ttu-id="8e36e-175">日期和上次修改任务的时间。</span><span class="sxs-lookup"><span data-stu-id="8e36e-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="8e36e-176">默认情况下，它是采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="8e36e-176">By default, it is in UTC.</span></span> <span data-ttu-id="8e36e-177">您可以提供请求标头中自定义时区。</span><span class="sxs-lookup"><span data-stu-id="8e36e-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="8e36e-178">该属性值使用 ISO 8601 格式，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8e36e-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8e36e-179">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8e36e-179">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8e36e-180">owner</span><span class="sxs-lookup"><span data-stu-id="8e36e-180">owner</span></span>|<span data-ttu-id="8e36e-181">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-181">String</span></span>|<span data-ttu-id="8e36e-182">创建任务的人员的名称。</span><span class="sxs-lookup"><span data-stu-id="8e36e-182">The name of the person who created the task.</span></span>|
|<span data-ttu-id="8e36e-183">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="8e36e-183">parentFolderId</span></span>|<span data-ttu-id="8e36e-184">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-184">String</span></span>|<span data-ttu-id="8e36e-185">任务的父文件夹的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8e36e-185">The unique identifier for the task's parent folder.</span></span>|
|<span data-ttu-id="8e36e-186">recurrence</span><span class="sxs-lookup"><span data-stu-id="8e36e-186">recurrence</span></span>|[<span data-ttu-id="8e36e-187">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8e36e-187">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="8e36e-188">定期模式的任务。</span><span class="sxs-lookup"><span data-stu-id="8e36e-188">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="8e36e-189">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="8e36e-189">reminderDateTime</span></span>|[<span data-ttu-id="8e36e-190">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8e36e-190">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="8e36e-191">发生的日期和时间的任务的提醒通知。</span><span class="sxs-lookup"><span data-stu-id="8e36e-191">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="8e36e-192">sensitivity</span><span class="sxs-lookup"><span data-stu-id="8e36e-192">sensitivity</span></span>|<span data-ttu-id="8e36e-193">string</span><span class="sxs-lookup"><span data-stu-id="8e36e-193">string</span></span>|<span data-ttu-id="8e36e-194">指示任务的隐私级别。</span><span class="sxs-lookup"><span data-stu-id="8e36e-194">Indicates the level of privacy for the task.</span></span> <span data-ttu-id="8e36e-195">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="8e36e-195">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="8e36e-196">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8e36e-196">startDateTime</span></span>|[<span data-ttu-id="8e36e-197">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8e36e-197">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="8e36e-198">在指定时区时的任务是开始日期。</span><span class="sxs-lookup"><span data-stu-id="8e36e-198">The date in the specified time zone when the task is to begin.</span></span>|
|<span data-ttu-id="8e36e-199">status</span><span class="sxs-lookup"><span data-stu-id="8e36e-199">status</span></span>|<span data-ttu-id="8e36e-200">string</span><span class="sxs-lookup"><span data-stu-id="8e36e-200">string</span></span>|<span data-ttu-id="8e36e-201">指示的状态或任务进度。</span><span class="sxs-lookup"><span data-stu-id="8e36e-201">Indicates the state or progress of the task.</span></span> <span data-ttu-id="8e36e-202">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="8e36e-202">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="8e36e-203">subject</span><span class="sxs-lookup"><span data-stu-id="8e36e-203">subject</span></span>|<span data-ttu-id="8e36e-204">String</span><span class="sxs-lookup"><span data-stu-id="8e36e-204">String</span></span>|<span data-ttu-id="8e36e-205">简要说明或任务的标题。</span><span class="sxs-lookup"><span data-stu-id="8e36e-205">A brief description or title of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="8e36e-206">响应</span><span class="sxs-lookup"><span data-stu-id="8e36e-206">Response</span></span>

<span data-ttu-id="8e36e-207">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8e36e-207">If successful, this method returns a `200 OK` response code and updated [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e36e-208">示例</span><span class="sxs-lookup"><span data-stu-id="8e36e-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e36e-209">请求</span><span class="sxs-lookup"><span data-stu-id="8e36e-209">Request</span></span>

<span data-ttu-id="8e36e-210">下面的示例修改**dueDateTime**属性，并使用`Prefer: outlook.timezone`标头以指定表达东部标准时间 (EST) 的响应中与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="8e36e-210">The following example modifies the **dueDateTime** property and uses the `Prefer: outlook.timezone` header to specify expressing the date-related properties in the response in Eastern Standard Time (EST).</span></span>
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

### <a name="response"></a><span data-ttu-id="8e36e-211">响应</span><span class="sxs-lookup"><span data-stu-id="8e36e-211">Response</span></span>

<span data-ttu-id="8e36e-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e36e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
