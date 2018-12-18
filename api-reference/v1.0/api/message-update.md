---
title: 更新邮件
description: 更新 message 对象的属性。
author: angelgolfer-ms
ms.openlocfilehash: b8f39dc9648203f86749ba06b88bf2f74b79d88a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337539"
---
# <a name="update-message"></a><span data-ttu-id="3faf9-103">更新邮件</span><span class="sxs-lookup"><span data-stu-id="3faf9-103">Update message</span></span>

<span data-ttu-id="3faf9-104">更新 message 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3faf9-104">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3faf9-105">权限</span><span class="sxs-lookup"><span data-stu-id="3faf9-105">Permissions</span></span>
<span data-ttu-id="3faf9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3faf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3faf9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3faf9-108">Permission type</span></span>      | <span data-ttu-id="3faf9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3faf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3faf9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3faf9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3faf9-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3faf9-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3faf9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3faf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3faf9-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3faf9-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3faf9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3faf9-114">Application</span></span> | <span data-ttu-id="3faf9-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3faf9-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3faf9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3faf9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3faf9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3faf9-117">Request headers</span></span>
| <span data-ttu-id="3faf9-118">Name</span><span class="sxs-lookup"><span data-stu-id="3faf9-118">Name</span></span>       | <span data-ttu-id="3faf9-119">类型</span><span class="sxs-lookup"><span data-stu-id="3faf9-119">Type</span></span> | <span data-ttu-id="3faf9-120">说明</span><span class="sxs-lookup"><span data-stu-id="3faf9-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3faf9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3faf9-121">Authorization</span></span>  | <span data-ttu-id="3faf9-122">string</span><span class="sxs-lookup"><span data-stu-id="3faf9-122">string</span></span>  | <span data-ttu-id="3faf9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3faf9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3faf9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3faf9-125">Content-Type</span></span> | <span data-ttu-id="3faf9-126">string</span><span class="sxs-lookup"><span data-stu-id="3faf9-126">string</span></span>  | <span data-ttu-id="3faf9-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="3faf9-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="3faf9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3faf9-129">Request body</span></span>
<span data-ttu-id="3faf9-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性</span><span class="sxs-lookup"><span data-stu-id="3faf9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="3faf9-134">属性</span><span class="sxs-lookup"><span data-stu-id="3faf9-134">Property</span></span>     | <span data-ttu-id="3faf9-135">类型</span><span class="sxs-lookup"><span data-stu-id="3faf9-135">Type</span></span>   |<span data-ttu-id="3faf9-136">说明</span><span class="sxs-lookup"><span data-stu-id="3faf9-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3faf9-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="3faf9-137">bccRecipients</span></span>|<span data-ttu-id="3faf9-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="3faf9-138">Recipient</span></span>|<span data-ttu-id="3faf9-139">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="3faf9-139">The Bcc recipients for the message.</span></span> <span data-ttu-id="3faf9-140">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-140">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="3faf9-141">categories</span><span class="sxs-lookup"><span data-stu-id="3faf9-141">categories</span></span>|<span data-ttu-id="3faf9-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3faf9-142">String collection</span></span>|<span data-ttu-id="3faf9-143">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="3faf9-143">The categories associated with the message.</span></span>|
|<span data-ttu-id="3faf9-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="3faf9-144">ccRecipients</span></span>|<span data-ttu-id="3faf9-145">收件人集合</span><span class="sxs-lookup"><span data-stu-id="3faf9-145">Recipient collection</span></span>|<span data-ttu-id="3faf9-146">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="3faf9-146">The Cc recipients for the message.</span></span> <span data-ttu-id="3faf9-147">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-147">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="3faf9-148">发件人</span><span class="sxs-lookup"><span data-stu-id="3faf9-148">from</span></span>|<span data-ttu-id="3faf9-149">Recipient</span><span class="sxs-lookup"><span data-stu-id="3faf9-149">Recipient</span></span>|<span data-ttu-id="3faf9-150">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="3faf9-150">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="3faf9-151">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-151">Updatable only if isDraft = true.</span></span> <span data-ttu-id="3faf9-152">必须为实际的邮箱使用相对应。</span><span class="sxs-lookup"><span data-stu-id="3faf9-152">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="3faf9-153">importance</span><span class="sxs-lookup"><span data-stu-id="3faf9-153">importance</span></span>|<span data-ttu-id="3faf9-154">String</span><span class="sxs-lookup"><span data-stu-id="3faf9-154">String</span></span>|<span data-ttu-id="3faf9-155">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="3faf9-155">The importance of the message.</span></span> <span data-ttu-id="3faf9-156">可能的值为： `Low`， `Normal`， `High`。</span><span class="sxs-lookup"><span data-stu-id="3faf9-156">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="3faf9-157">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="3faf9-157">inferenceClassification</span></span> | <span data-ttu-id="3faf9-158">字符串</span><span class="sxs-lookup"><span data-stu-id="3faf9-158">String</span></span> | <span data-ttu-id="3faf9-159">为用户、 基于推测的相关性或重要性-或显式重写的邮件分类。</span><span class="sxs-lookup"><span data-stu-id="3faf9-159">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="3faf9-160">可能的值为：`focused`或`other`。</span><span class="sxs-lookup"><span data-stu-id="3faf9-160">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="3faf9-161">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="3faf9-161">internetMessageId</span></span> |<span data-ttu-id="3faf9-162">String</span><span class="sxs-lookup"><span data-stu-id="3faf9-162">String</span></span> |<span data-ttu-id="3faf9-163">由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="3faf9-163">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="3faf9-164">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-164">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="3faf9-165">isRead</span><span class="sxs-lookup"><span data-stu-id="3faf9-165">isRead</span></span>|<span data-ttu-id="3faf9-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="3faf9-166">Boolean</span></span>|<span data-ttu-id="3faf9-167">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="3faf9-167">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="3faf9-168">replyTo</span><span class="sxs-lookup"><span data-stu-id="3faf9-168">replyTo</span></span>|<span data-ttu-id="3faf9-169">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="3faf9-169">Recipient collection</span></span>|<span data-ttu-id="3faf9-170">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3faf9-170">The email addresses to use when replying.</span></span> <span data-ttu-id="3faf9-171">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-171">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="3faf9-172">sender</span><span class="sxs-lookup"><span data-stu-id="3faf9-172">sender</span></span>|<span data-ttu-id="3faf9-173">Recipient</span><span class="sxs-lookup"><span data-stu-id="3faf9-173">Recipient</span></span>|<span data-ttu-id="3faf9-174">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="3faf9-174">The account that is actually used to generate the message.</span></span> <span data-ttu-id="3faf9-175">可更新才 isDraft = true，以及何时从[共享的邮箱](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送消息或[委派](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送一条消息。</span><span class="sxs-lookup"><span data-stu-id="3faf9-175">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="3faf9-176">在任何情况下的值必须为实际的邮箱使用对应。</span><span class="sxs-lookup"><span data-stu-id="3faf9-176">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="3faf9-177">toRecipients</span><span class="sxs-lookup"><span data-stu-id="3faf9-177">toRecipients</span></span>|<span data-ttu-id="3faf9-178">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="3faf9-178">Recipient collection</span></span>|<span data-ttu-id="3faf9-179">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="3faf9-179">The To recipients for the message.</span></span> <span data-ttu-id="3faf9-180">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-180">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="3faf9-181">body</span><span class="sxs-lookup"><span data-stu-id="3faf9-181">body</span></span>|<span data-ttu-id="3faf9-182">ItemBody</span><span class="sxs-lookup"><span data-stu-id="3faf9-182">ItemBody</span></span>|<span data-ttu-id="3faf9-183">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="3faf9-183">The body of the message.</span></span> <span data-ttu-id="3faf9-184">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="3faf9-185">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3faf9-185">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="3faf9-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="3faf9-186">Boolean</span></span>|<span data-ttu-id="3faf9-187">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="3faf9-187">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="3faf9-188">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="3faf9-188">isReadReceiptRequested</span></span>|<span data-ttu-id="3faf9-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="3faf9-189">Boolean</span></span>|<span data-ttu-id="3faf9-190">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="3faf9-190">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="3faf9-191">subject</span><span class="sxs-lookup"><span data-stu-id="3faf9-191">subject</span></span>|<span data-ttu-id="3faf9-192">String</span><span class="sxs-lookup"><span data-stu-id="3faf9-192">String</span></span>|<span data-ttu-id="3faf9-193">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="3faf9-193">The subject of the message.</span></span> <span data-ttu-id="3faf9-194">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="3faf9-194">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="3faf9-195">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="3faf9-195">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="3faf9-196">响应</span><span class="sxs-lookup"><span data-stu-id="3faf9-196">Response</span></span>

<span data-ttu-id="3faf9-197">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3faf9-197">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3faf9-198">示例</span><span class="sxs-lookup"><span data-stu-id="3faf9-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3faf9-199">请求</span><span class="sxs-lookup"><span data-stu-id="3faf9-199">Request</span></span>
<span data-ttu-id="3faf9-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3faf9-200">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a><span data-ttu-id="3faf9-201">响应</span><span class="sxs-lookup"><span data-stu-id="3faf9-201">Response</span></span>
<span data-ttu-id="3faf9-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3faf9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
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
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a><span data-ttu-id="3faf9-205">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3faf9-205">See also</span></span>

- [<span data-ttu-id="3faf9-206">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3faf9-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3faf9-207">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="3faf9-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
