---
title: 更新 eventMessage
description: 更新 eventMessage 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dbfb68954acb93e66ea09c3b71ec405d9754e407
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951297"
---
# <a name="update-eventmessage"></a><span data-ttu-id="3fd66-103">更新 eventMessage</span><span class="sxs-lookup"><span data-stu-id="3fd66-103">Update eventMessage</span></span>

> <span data-ttu-id="3fd66-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3fd66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fd66-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3fd66-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3fd66-106">更新 [eventMessage](../resources/eventmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3fd66-106">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3fd66-107">权限</span><span class="sxs-lookup"><span data-stu-id="3fd66-107">Permissions</span></span>
<span data-ttu-id="3fd66-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3fd66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fd66-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fd66-110">Permission type</span></span>      | <span data-ttu-id="3fd66-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3fd66-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fd66-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fd66-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3fd66-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fd66-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3fd66-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fd66-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fd66-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fd66-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3fd66-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fd66-116">Application</span></span> | <span data-ttu-id="3fd66-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fd66-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fd66-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fd66-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3fd66-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fd66-119">Request headers</span></span>
| <span data-ttu-id="3fd66-120">名称</span><span class="sxs-lookup"><span data-stu-id="3fd66-120">Name</span></span>       | <span data-ttu-id="3fd66-121">类型</span><span class="sxs-lookup"><span data-stu-id="3fd66-121">Type</span></span> | <span data-ttu-id="3fd66-122">说明</span><span class="sxs-lookup"><span data-stu-id="3fd66-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3fd66-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fd66-123">Authorization</span></span>  | <span data-ttu-id="3fd66-124">string</span><span class="sxs-lookup"><span data-stu-id="3fd66-124">string</span></span>  | <span data-ttu-id="3fd66-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3fd66-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fd66-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3fd66-127">Content-Type</span></span> | <span data-ttu-id="3fd66-128">string</span><span class="sxs-lookup"><span data-stu-id="3fd66-128">string</span></span>  | <span data-ttu-id="3fd66-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="3fd66-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="3fd66-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fd66-131">Request body</span></span>
<span data-ttu-id="3fd66-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性</span><span class="sxs-lookup"><span data-stu-id="3fd66-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="3fd66-136">属性</span><span class="sxs-lookup"><span data-stu-id="3fd66-136">Property</span></span>     | <span data-ttu-id="3fd66-137">类型</span><span class="sxs-lookup"><span data-stu-id="3fd66-137">Type</span></span>   |<span data-ttu-id="3fd66-138">说明</span><span class="sxs-lookup"><span data-stu-id="3fd66-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fd66-139">categories</span><span class="sxs-lookup"><span data-stu-id="3fd66-139">categories</span></span>|<span data-ttu-id="3fd66-140">String</span><span class="sxs-lookup"><span data-stu-id="3fd66-140">String</span></span>|<span data-ttu-id="3fd66-141">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="3fd66-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="3fd66-142">重要性</span><span class="sxs-lookup"><span data-stu-id="3fd66-142">importance</span></span>|<span data-ttu-id="3fd66-143">String</span><span class="sxs-lookup"><span data-stu-id="3fd66-143">String</span></span>|<span data-ttu-id="3fd66-p106">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="3fd66-p106">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="3fd66-146">isAllDay</span><span class="sxs-lookup"><span data-stu-id="3fd66-146">isAllDay</span></span> |<span data-ttu-id="3fd66-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fd66-147">Boolean</span></span>|<span data-ttu-id="3fd66-148">指示是否事件持续的整个天。</span><span class="sxs-lookup"><span data-stu-id="3fd66-148">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="3fd66-149">调整此属性需要调整事件以及的**开始日期时间**和**endDateTime**属性。</span><span class="sxs-lookup"><span data-stu-id="3fd66-149">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="3fd66-150">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3fd66-150">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="3fd66-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fd66-151">Boolean</span></span>|<span data-ttu-id="3fd66-152">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="3fd66-152">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="3fd66-153">isRead</span><span class="sxs-lookup"><span data-stu-id="3fd66-153">isRead</span></span>|<span data-ttu-id="3fd66-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fd66-154">Boolean</span></span>|<span data-ttu-id="3fd66-155">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="3fd66-155">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="3fd66-156">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3fd66-156">isReadReceiptRequested</span></span>|<span data-ttu-id="3fd66-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fd66-157">Boolean</span></span>|<span data-ttu-id="3fd66-158">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="3fd66-158">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="3fd66-159">响应</span><span class="sxs-lookup"><span data-stu-id="3fd66-159">Response</span></span>

<span data-ttu-id="3fd66-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3fd66-160">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3fd66-161">示例</span><span class="sxs-lookup"><span data-stu-id="3fd66-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fd66-162">请求</span><span class="sxs-lookup"><span data-stu-id="3fd66-162">Request</span></span>
<span data-ttu-id="3fd66-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3fd66-163">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="3fd66-164">响应</span><span class="sxs-lookup"><span data-stu-id="3fd66-164">Response</span></span>
<span data-ttu-id="3fd66-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3fd66-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
