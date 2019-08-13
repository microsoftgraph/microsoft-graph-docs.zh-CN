---
title: 更新 eventMessage
description: 更新 eventMessage 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 781c95e1ed955458ce952ede8ddf4c18879299db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319167"
---
# <a name="update-eventmessage"></a><span data-ttu-id="b030e-103">更新 eventMessage</span><span class="sxs-lookup"><span data-stu-id="b030e-103">Update eventMessage</span></span>

<span data-ttu-id="b030e-104">更新 [eventMessage](../resources/eventmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b030e-104">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b030e-105">权限</span><span class="sxs-lookup"><span data-stu-id="b030e-105">Permissions</span></span>
<span data-ttu-id="b030e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b030e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b030e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b030e-108">Permission type</span></span>      | <span data-ttu-id="b030e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b030e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b030e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b030e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b030e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b030e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b030e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b030e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b030e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b030e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b030e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b030e-114">Application</span></span> | <span data-ttu-id="b030e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b030e-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b030e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b030e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b030e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b030e-117">Request headers</span></span>
| <span data-ttu-id="b030e-118">名称</span><span class="sxs-lookup"><span data-stu-id="b030e-118">Name</span></span>       | <span data-ttu-id="b030e-119">类型</span><span class="sxs-lookup"><span data-stu-id="b030e-119">Type</span></span> | <span data-ttu-id="b030e-120">说明</span><span class="sxs-lookup"><span data-stu-id="b030e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b030e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b030e-121">Authorization</span></span>  | <span data-ttu-id="b030e-122">string</span><span class="sxs-lookup"><span data-stu-id="b030e-122">string</span></span>  | <span data-ttu-id="b030e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b030e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b030e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b030e-125">Content-Type</span></span> | <span data-ttu-id="b030e-126">string</span><span class="sxs-lookup"><span data-stu-id="b030e-126">string</span></span>  | <span data-ttu-id="b030e-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="b030e-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="b030e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b030e-129">Request body</span></span>
<span data-ttu-id="b030e-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性</span><span class="sxs-lookup"><span data-stu-id="b030e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="b030e-134">属性</span><span class="sxs-lookup"><span data-stu-id="b030e-134">Property</span></span>     | <span data-ttu-id="b030e-135">类型</span><span class="sxs-lookup"><span data-stu-id="b030e-135">Type</span></span>   |<span data-ttu-id="b030e-136">说明</span><span class="sxs-lookup"><span data-stu-id="b030e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b030e-137">categories</span><span class="sxs-lookup"><span data-stu-id="b030e-137">categories</span></span>|<span data-ttu-id="b030e-138">String</span><span class="sxs-lookup"><span data-stu-id="b030e-138">String</span></span>|<span data-ttu-id="b030e-139">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="b030e-139">The categories associated with the message.</span></span>|
|<span data-ttu-id="b030e-140">importance</span><span class="sxs-lookup"><span data-stu-id="b030e-140">importance</span></span>|<span data-ttu-id="b030e-141">String</span><span class="sxs-lookup"><span data-stu-id="b030e-141">String</span></span>|<span data-ttu-id="b030e-142">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="b030e-142">The importance of the message.</span></span> <span data-ttu-id="b030e-143">可能的值包括 `Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="b030e-143">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="b030e-144">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b030e-144">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="b030e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b030e-145">Boolean</span></span>|<span data-ttu-id="b030e-146">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="b030e-146">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="b030e-147">isRead</span><span class="sxs-lookup"><span data-stu-id="b030e-147">isRead</span></span>|<span data-ttu-id="b030e-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="b030e-148">Boolean</span></span>|<span data-ttu-id="b030e-149">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="b030e-149">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="b030e-150">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b030e-150">isReadReceiptRequested</span></span>|<span data-ttu-id="b030e-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b030e-151">Boolean</span></span>|<span data-ttu-id="b030e-152">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="b030e-152">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="b030e-153">响应</span><span class="sxs-lookup"><span data-stu-id="b030e-153">Response</span></span>

<span data-ttu-id="b030e-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b030e-154">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b030e-155">示例</span><span class="sxs-lookup"><span data-stu-id="b030e-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b030e-156">请求</span><span class="sxs-lookup"><span data-stu-id="b030e-156">Request</span></span>
<span data-ttu-id="b030e-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b030e-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b030e-158">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b030e-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b030e-159">C#</span><span class="sxs-lookup"><span data-stu-id="b030e-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b030e-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b030e-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b030e-161">目标-C</span><span class="sxs-lookup"><span data-stu-id="b030e-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b030e-162">Java</span><span class="sxs-lookup"><span data-stu-id="b030e-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b030e-163">响应</span><span class="sxs-lookup"><span data-stu-id="b030e-163">Response</span></span>
<span data-ttu-id="b030e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b030e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
