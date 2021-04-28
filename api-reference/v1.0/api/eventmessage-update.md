---
title: 更新 eventMessage
description: 更新 eventMessage 对象的属性。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6b523e12da00d4b0883d9e337edd288ded13bde2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052395"
---
# <a name="update-eventmessage"></a><span data-ttu-id="f2df6-103">更新 eventMessage</span><span class="sxs-lookup"><span data-stu-id="f2df6-103">Update eventMessage</span></span>

<span data-ttu-id="f2df6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2df6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2df6-105">更新 [eventMessage](../resources/eventmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2df6-105">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2df6-106">权限</span><span class="sxs-lookup"><span data-stu-id="f2df6-106">Permissions</span></span>
<span data-ttu-id="f2df6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2df6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2df6-109">Permission type</span></span>      | <span data-ttu-id="f2df6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2df6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2df6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2df6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2df6-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2df6-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f2df6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2df6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2df6-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2df6-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f2df6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2df6-115">Application</span></span> | <span data-ttu-id="f2df6-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2df6-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2df6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2df6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f2df6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2df6-118">Request headers</span></span>
| <span data-ttu-id="f2df6-119">名称</span><span class="sxs-lookup"><span data-stu-id="f2df6-119">Name</span></span>       | <span data-ttu-id="f2df6-120">类型</span><span class="sxs-lookup"><span data-stu-id="f2df6-120">Type</span></span> | <span data-ttu-id="f2df6-121">说明</span><span class="sxs-lookup"><span data-stu-id="f2df6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2df6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2df6-122">Authorization</span></span>  | <span data-ttu-id="f2df6-123">string</span><span class="sxs-lookup"><span data-stu-id="f2df6-123">string</span></span>  | <span data-ttu-id="f2df6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2df6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f2df6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2df6-126">Content-Type</span></span> | <span data-ttu-id="f2df6-127">string</span><span class="sxs-lookup"><span data-stu-id="f2df6-127">string</span></span>  | <span data-ttu-id="f2df6-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f2df6-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="f2df6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2df6-130">Request body</span></span>
<span data-ttu-id="f2df6-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性</span><span class="sxs-lookup"><span data-stu-id="f2df6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="f2df6-135">属性</span><span class="sxs-lookup"><span data-stu-id="f2df6-135">Property</span></span>     | <span data-ttu-id="f2df6-136">类型</span><span class="sxs-lookup"><span data-stu-id="f2df6-136">Type</span></span>   |<span data-ttu-id="f2df6-137">说明</span><span class="sxs-lookup"><span data-stu-id="f2df6-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2df6-138">categories</span><span class="sxs-lookup"><span data-stu-id="f2df6-138">categories</span></span>|<span data-ttu-id="f2df6-139">String</span><span class="sxs-lookup"><span data-stu-id="f2df6-139">String</span></span>|<span data-ttu-id="f2df6-140">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="f2df6-140">The categories associated with the message.</span></span>|
|<span data-ttu-id="f2df6-141">importance</span><span class="sxs-lookup"><span data-stu-id="f2df6-141">importance</span></span>|<span data-ttu-id="f2df6-142">String</span><span class="sxs-lookup"><span data-stu-id="f2df6-142">String</span></span>|<span data-ttu-id="f2df6-143">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="f2df6-143">The importance of the message.</span></span> <span data-ttu-id="f2df6-144">可能的值包括 `Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="f2df6-144">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="f2df6-145">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f2df6-145">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="f2df6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2df6-146">Boolean</span></span>|<span data-ttu-id="f2df6-147">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="f2df6-147">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="f2df6-148">isRead</span><span class="sxs-lookup"><span data-stu-id="f2df6-148">isRead</span></span>|<span data-ttu-id="f2df6-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2df6-149">Boolean</span></span>|<span data-ttu-id="f2df6-150">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="f2df6-150">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="f2df6-151">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f2df6-151">isReadReceiptRequested</span></span>|<span data-ttu-id="f2df6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2df6-152">Boolean</span></span>|<span data-ttu-id="f2df6-153">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="f2df6-153">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="f2df6-154">响应</span><span class="sxs-lookup"><span data-stu-id="f2df6-154">Response</span></span>

<span data-ttu-id="f2df6-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2df6-155">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2df6-156">示例</span><span class="sxs-lookup"><span data-stu-id="f2df6-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2df6-157">请求</span><span class="sxs-lookup"><span data-stu-id="f2df6-157">Request</span></span>
<span data-ttu-id="f2df6-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2df6-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2df6-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2df6-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": true,
}
```
# <a name="c"></a>[<span data-ttu-id="f2df6-160">C#</span><span class="sxs-lookup"><span data-stu-id="f2df6-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2df6-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2df6-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2df6-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2df6-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2df6-163">Java</span><span class="sxs-lookup"><span data-stu-id="f2df6-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f2df6-164">响应</span><span class="sxs-lookup"><span data-stu-id="f2df6-164">Response</span></span>
<span data-ttu-id="f2df6-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f2df6-165">Here is an example of the response.</span></span> <span data-ttu-id="f2df6-166">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f2df6-166">Note: The response object shown here might be shortened for readability.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

