---
title: 更新 eventMessage
description: 更新 eventMessage 对象的属性。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9a6f6fa3a63d1c1e2db29e6eb01882982a832564
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965710"
---
# <a name="update-eventmessage"></a><span data-ttu-id="d6485-103">更新 eventMessage</span><span class="sxs-lookup"><span data-stu-id="d6485-103">Update eventMessage</span></span>

<span data-ttu-id="d6485-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6485-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6485-105">更新 [eventMessage](../resources/eventmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6485-105">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6485-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6485-106">Permissions</span></span>
<span data-ttu-id="d6485-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6485-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6485-109">Permission type</span></span>      | <span data-ttu-id="d6485-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6485-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6485-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6485-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6485-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6485-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6485-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6485-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6485-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6485-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6485-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6485-115">Application</span></span> | <span data-ttu-id="d6485-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6485-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6485-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6485-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d6485-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6485-118">Request headers</span></span>
| <span data-ttu-id="d6485-119">名称</span><span class="sxs-lookup"><span data-stu-id="d6485-119">Name</span></span>       | <span data-ttu-id="d6485-120">类型</span><span class="sxs-lookup"><span data-stu-id="d6485-120">Type</span></span> | <span data-ttu-id="d6485-121">说明</span><span class="sxs-lookup"><span data-stu-id="d6485-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d6485-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6485-122">Authorization</span></span>  | <span data-ttu-id="d6485-123">string</span><span class="sxs-lookup"><span data-stu-id="d6485-123">string</span></span>  | <span data-ttu-id="d6485-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6485-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6485-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6485-126">Content-Type</span></span> | <span data-ttu-id="d6485-127">string</span><span class="sxs-lookup"><span data-stu-id="d6485-127">string</span></span>  | <span data-ttu-id="d6485-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="d6485-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="d6485-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6485-130">Request body</span></span>
<span data-ttu-id="d6485-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性</span><span class="sxs-lookup"><span data-stu-id="d6485-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="d6485-135">属性</span><span class="sxs-lookup"><span data-stu-id="d6485-135">Property</span></span>     | <span data-ttu-id="d6485-136">类型</span><span class="sxs-lookup"><span data-stu-id="d6485-136">Type</span></span>   |<span data-ttu-id="d6485-137">说明</span><span class="sxs-lookup"><span data-stu-id="d6485-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6485-138">categories</span><span class="sxs-lookup"><span data-stu-id="d6485-138">categories</span></span>|<span data-ttu-id="d6485-139">String</span><span class="sxs-lookup"><span data-stu-id="d6485-139">String</span></span>|<span data-ttu-id="d6485-140">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="d6485-140">The categories associated with the message.</span></span>|
|<span data-ttu-id="d6485-141">importance</span><span class="sxs-lookup"><span data-stu-id="d6485-141">importance</span></span>|<span data-ttu-id="d6485-142">String</span><span class="sxs-lookup"><span data-stu-id="d6485-142">String</span></span>|<span data-ttu-id="d6485-p105">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="d6485-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="d6485-145">isAllDay</span><span class="sxs-lookup"><span data-stu-id="d6485-145">isAllDay</span></span> |<span data-ttu-id="d6485-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6485-146">Boolean</span></span>|<span data-ttu-id="d6485-147">指示事件是否持续一整天。</span><span class="sxs-lookup"><span data-stu-id="d6485-147">Indicates whether the event lasts the entire day.</span></span> <span data-ttu-id="d6485-148">调整此属性还需要调整事件的 **startDateTime** 和 **endDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="d6485-148">Adjusting this property requires adjusting the **startDateTime** and **endDateTime** properties of the event as well.</span></span>|
|<span data-ttu-id="d6485-149">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d6485-149">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="d6485-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6485-150">Boolean</span></span>|<span data-ttu-id="d6485-151">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="d6485-151">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="d6485-152">isRead</span><span class="sxs-lookup"><span data-stu-id="d6485-152">isRead</span></span>|<span data-ttu-id="d6485-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6485-153">Boolean</span></span>|<span data-ttu-id="d6485-154">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="d6485-154">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="d6485-155">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d6485-155">isReadReceiptRequested</span></span>|<span data-ttu-id="d6485-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6485-156">Boolean</span></span>|<span data-ttu-id="d6485-157">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="d6485-157">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="d6485-158">响应</span><span class="sxs-lookup"><span data-stu-id="d6485-158">Response</span></span>

<span data-ttu-id="d6485-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6485-159">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6485-160">示例</span><span class="sxs-lookup"><span data-stu-id="d6485-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6485-161">请求</span><span class="sxs-lookup"><span data-stu-id="d6485-161">Request</span></span>
<span data-ttu-id="d6485-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6485-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6485-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6485-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d6485-164">C#</span><span class="sxs-lookup"><span data-stu-id="d6485-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6485-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6485-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6485-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6485-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6485-167">Java</span><span class="sxs-lookup"><span data-stu-id="d6485-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6485-168">响应</span><span class="sxs-lookup"><span data-stu-id="d6485-168">Response</span></span>
<span data-ttu-id="d6485-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6485-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


