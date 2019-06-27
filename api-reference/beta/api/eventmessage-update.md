---
title: 更新 eventMessage
description: 更新 eventMessage 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 704f27852a6fd57437905b589f73e1b9032e1404
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259050"
---
# <a name="update-eventmessage"></a><span data-ttu-id="9bd2f-103">更新 eventMessage</span><span class="sxs-lookup"><span data-stu-id="9bd2f-103">Update eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd2f-104">更新 [eventMessage](../resources/eventmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9bd2f-105">权限</span><span class="sxs-lookup"><span data-stu-id="9bd2f-105">Permissions</span></span>
<span data-ttu-id="9bd2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd2f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bd2f-108">Permission type</span></span>      | <span data-ttu-id="9bd2f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bd2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bd2f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9bd2f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd2f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9bd2f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bd2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bd2f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd2f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9bd2f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bd2f-114">Application</span></span> | <span data-ttu-id="9bd2f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bd2f-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bd2f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bd2f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9bd2f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bd2f-117">Request headers</span></span>
| <span data-ttu-id="9bd2f-118">名称</span><span class="sxs-lookup"><span data-stu-id="9bd2f-118">Name</span></span>       | <span data-ttu-id="9bd2f-119">类型</span><span class="sxs-lookup"><span data-stu-id="9bd2f-119">Type</span></span> | <span data-ttu-id="9bd2f-120">说明</span><span class="sxs-lookup"><span data-stu-id="9bd2f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9bd2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd2f-121">Authorization</span></span>  | <span data-ttu-id="9bd2f-122">string</span><span class="sxs-lookup"><span data-stu-id="9bd2f-122">string</span></span>  | <span data-ttu-id="9bd2f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9bd2f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bd2f-125">Content-Type</span></span> | <span data-ttu-id="9bd2f-126">string</span><span class="sxs-lookup"><span data-stu-id="9bd2f-126">string</span></span>  | <span data-ttu-id="9bd2f-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="9bd2f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bd2f-129">Request body</span></span>
<span data-ttu-id="9bd2f-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性</span><span class="sxs-lookup"><span data-stu-id="9bd2f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="9bd2f-134">属性</span><span class="sxs-lookup"><span data-stu-id="9bd2f-134">Property</span></span>     | <span data-ttu-id="9bd2f-135">类型</span><span class="sxs-lookup"><span data-stu-id="9bd2f-135">Type</span></span>   |<span data-ttu-id="9bd2f-136">说明</span><span class="sxs-lookup"><span data-stu-id="9bd2f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bd2f-137">categories</span><span class="sxs-lookup"><span data-stu-id="9bd2f-137">categories</span></span>|<span data-ttu-id="9bd2f-138">String</span><span class="sxs-lookup"><span data-stu-id="9bd2f-138">String</span></span>|<span data-ttu-id="9bd2f-139">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="9bd2f-140">importance</span><span class="sxs-lookup"><span data-stu-id="9bd2f-140">importance</span></span>|<span data-ttu-id="9bd2f-141">String</span><span class="sxs-lookup"><span data-stu-id="9bd2f-141">String</span></span>|<span data-ttu-id="9bd2f-p105">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="9bd2f-144">isAllDay</span><span class="sxs-lookup"><span data-stu-id="9bd2f-144">isAllDay</span></span> |<span data-ttu-id="9bd2f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd2f-145">Boolean</span></span>|<span data-ttu-id="9bd2f-146">指示事件是否持续一整天。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-146">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="9bd2f-147">调整此属性还需要调整事件的**startDateTime**和**endDateTime**属性。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-147">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="9bd2f-148">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="9bd2f-148">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="9bd2f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd2f-149">Boolean</span></span>|<span data-ttu-id="9bd2f-150">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-150">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="9bd2f-151">isRead</span><span class="sxs-lookup"><span data-stu-id="9bd2f-151">isRead</span></span>|<span data-ttu-id="9bd2f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd2f-152">Boolean</span></span>|<span data-ttu-id="9bd2f-153">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-153">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="9bd2f-154">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="9bd2f-154">isReadReceiptRequested</span></span>|<span data-ttu-id="9bd2f-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd2f-155">Boolean</span></span>|<span data-ttu-id="9bd2f-156">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-156">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="9bd2f-157">响应</span><span class="sxs-lookup"><span data-stu-id="9bd2f-157">Response</span></span>

<span data-ttu-id="9bd2f-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-158">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9bd2f-159">示例</span><span class="sxs-lookup"><span data-stu-id="9bd2f-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bd2f-160">请求</span><span class="sxs-lookup"><span data-stu-id="9bd2f-160">Request</span></span>
<span data-ttu-id="9bd2f-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-161">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9bd2f-162">响应</span><span class="sxs-lookup"><span data-stu-id="9bd2f-162">Response</span></span>
<span data-ttu-id="9bd2f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bd2f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9bd2f-166">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9bd2f-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9bd2f-167">C#</span><span class="sxs-lookup"><span data-stu-id="9bd2f-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9bd2f-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="9bd2f-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9bd2f-169">目标-C</span><span class="sxs-lookup"><span data-stu-id="9bd2f-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/eventmessage-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/eventmessage-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
