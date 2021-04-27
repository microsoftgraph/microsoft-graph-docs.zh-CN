---
title: 更新邮件
description: 更新 message 对象的属性。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cbc836f1476032d49d2fe33c4510ccab9634b5e0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050127"
---
# <a name="update-message"></a><span data-ttu-id="99a35-103">更新邮件</span><span class="sxs-lookup"><span data-stu-id="99a35-103">Update message</span></span>

<span data-ttu-id="99a35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99a35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99a35-105">更新 message 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="99a35-105">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="99a35-106">权限</span><span class="sxs-lookup"><span data-stu-id="99a35-106">Permissions</span></span>
<span data-ttu-id="99a35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99a35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99a35-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99a35-109">Permission type</span></span>      | <span data-ttu-id="99a35-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99a35-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99a35-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99a35-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99a35-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99a35-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="99a35-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99a35-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99a35-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99a35-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="99a35-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99a35-115">Application</span></span> | <span data-ttu-id="99a35-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99a35-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="99a35-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99a35-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="99a35-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="99a35-118">Request headers</span></span>
| <span data-ttu-id="99a35-119">名称</span><span class="sxs-lookup"><span data-stu-id="99a35-119">Name</span></span>       | <span data-ttu-id="99a35-120">类型</span><span class="sxs-lookup"><span data-stu-id="99a35-120">Type</span></span> | <span data-ttu-id="99a35-121">说明</span><span class="sxs-lookup"><span data-stu-id="99a35-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99a35-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99a35-122">Authorization</span></span>  | <span data-ttu-id="99a35-123">string</span><span class="sxs-lookup"><span data-stu-id="99a35-123">string</span></span>  | <span data-ttu-id="99a35-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99a35-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99a35-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99a35-126">Content-Type</span></span> | <span data-ttu-id="99a35-127">string</span><span class="sxs-lookup"><span data-stu-id="99a35-127">string</span></span>  | <span data-ttu-id="99a35-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="99a35-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="99a35-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="99a35-130">Request body</span></span>
<span data-ttu-id="99a35-131">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="99a35-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="99a35-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="99a35-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="99a35-133">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="99a35-133">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="99a35-134">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="99a35-134">The following properties can be updated.</span></span>

| <span data-ttu-id="99a35-135">属性</span><span class="sxs-lookup"><span data-stu-id="99a35-135">Property</span></span>     | <span data-ttu-id="99a35-136">类型</span><span class="sxs-lookup"><span data-stu-id="99a35-136">Type</span></span>   |<span data-ttu-id="99a35-137">说明</span><span class="sxs-lookup"><span data-stu-id="99a35-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99a35-138">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="99a35-138">bccRecipients</span></span>|<span data-ttu-id="99a35-139">收件人</span><span class="sxs-lookup"><span data-stu-id="99a35-139">Recipient</span></span>|<span data-ttu-id="99a35-140">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="99a35-140">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="99a35-141">body</span><span class="sxs-lookup"><span data-stu-id="99a35-141">body</span></span>|<span data-ttu-id="99a35-142">ItemBody</span><span class="sxs-lookup"><span data-stu-id="99a35-142">ItemBody</span></span>|<span data-ttu-id="99a35-143">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="99a35-143">The body of the message.</span></span> <span data-ttu-id="99a35-144">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="99a35-144">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="99a35-145">categories</span><span class="sxs-lookup"><span data-stu-id="99a35-145">categories</span></span>|<span data-ttu-id="99a35-146">String collection</span><span class="sxs-lookup"><span data-stu-id="99a35-146">String collection</span></span>|<span data-ttu-id="99a35-147">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="99a35-147">The categories associated with the message.</span></span>|
|<span data-ttu-id="99a35-148">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="99a35-148">ccRecipients</span></span>|<span data-ttu-id="99a35-149">收件人集合</span><span class="sxs-lookup"><span data-stu-id="99a35-149">Recipient collection</span></span>|<span data-ttu-id="99a35-150">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="99a35-150">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="99a35-151">flag</span><span class="sxs-lookup"><span data-stu-id="99a35-151">flag</span></span>|[<span data-ttu-id="99a35-152">followupFlag</span><span class="sxs-lookup"><span data-stu-id="99a35-152">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="99a35-153">指示邮件的状态、开始日期、截止日期或完成日期的标志值。</span><span class="sxs-lookup"><span data-stu-id="99a35-153">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="99a35-154">发件人</span><span class="sxs-lookup"><span data-stu-id="99a35-154">from</span></span>|<span data-ttu-id="99a35-155">收件人</span><span class="sxs-lookup"><span data-stu-id="99a35-155">Recipient</span></span>|<span data-ttu-id="99a35-156">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="99a35-156">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="99a35-157">必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="99a35-157">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="99a35-158">importance</span><span class="sxs-lookup"><span data-stu-id="99a35-158">importance</span></span>|<span data-ttu-id="99a35-159">String</span><span class="sxs-lookup"><span data-stu-id="99a35-159">String</span></span>|<span data-ttu-id="99a35-p107">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="99a35-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="99a35-162">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="99a35-162">inferenceClassification</span></span> | <span data-ttu-id="99a35-163">String</span><span class="sxs-lookup"><span data-stu-id="99a35-163">String</span></span> | <span data-ttu-id="99a35-p108">根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="99a35-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="99a35-166">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="99a35-166">internetMessageId</span></span> |<span data-ttu-id="99a35-167">String</span><span class="sxs-lookup"><span data-stu-id="99a35-167">String</span></span> |<span data-ttu-id="99a35-168">由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="99a35-168">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="99a35-169">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="99a35-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="99a35-170">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="99a35-170">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="99a35-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="99a35-171">Boolean</span></span>|<span data-ttu-id="99a35-172">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="99a35-172">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="99a35-173">isRead</span><span class="sxs-lookup"><span data-stu-id="99a35-173">isRead</span></span>|<span data-ttu-id="99a35-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="99a35-174">Boolean</span></span>|<span data-ttu-id="99a35-175">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="99a35-175">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="99a35-176">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="99a35-176">isReadReceiptRequested</span></span>|<span data-ttu-id="99a35-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="99a35-177">Boolean</span></span>|<span data-ttu-id="99a35-178">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="99a35-178">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="99a35-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="99a35-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="99a35-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99a35-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="99a35-181">为邮件定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="99a35-181">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="99a35-182">可为空。</span><span class="sxs-lookup"><span data-stu-id="99a35-182">Nullable.</span></span>|
|<span data-ttu-id="99a35-183">replyTo</span><span class="sxs-lookup"><span data-stu-id="99a35-183">replyTo</span></span>|<span data-ttu-id="99a35-184">收件人集合</span><span class="sxs-lookup"><span data-stu-id="99a35-184">Recipient collection</span></span>|<span data-ttu-id="99a35-185">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="99a35-185">The email addresses to use when replying.</span></span> <span data-ttu-id="99a35-186">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="99a35-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="99a35-187">sender</span><span class="sxs-lookup"><span data-stu-id="99a35-187">sender</span></span>|<span data-ttu-id="99a35-188">收件人</span><span class="sxs-lookup"><span data-stu-id="99a35-188">Recipient</span></span>|<span data-ttu-id="99a35-189">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="99a35-189">The account that is actually used to generate the message.</span></span> <span data-ttu-id="99a35-190">从[共享邮箱](/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件或将邮件作为[委托](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送时可更新。</span><span class="sxs-lookup"><span data-stu-id="99a35-190">Updatable when sending a message from a [shared mailbox](/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="99a35-191">在任何情况下，此值必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="99a35-191">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="99a35-192">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="99a35-192">singleValueExtendedProperties</span></span>|<span data-ttu-id="99a35-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="99a35-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="99a35-p113">为邮件定义的单值扩展属性的集合。可为空。</span><span class="sxs-lookup"><span data-stu-id="99a35-p113">The collection of single-value extended properties defined for the message. Nullable.</span></span>|
|<span data-ttu-id="99a35-196">subject</span><span class="sxs-lookup"><span data-stu-id="99a35-196">subject</span></span>|<span data-ttu-id="99a35-197">String</span><span class="sxs-lookup"><span data-stu-id="99a35-197">String</span></span>|<span data-ttu-id="99a35-198">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="99a35-198">The subject of the message.</span></span> <span data-ttu-id="99a35-199">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="99a35-199">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="99a35-200">toRecipients</span><span class="sxs-lookup"><span data-stu-id="99a35-200">toRecipients</span></span>|<span data-ttu-id="99a35-201">收件人集合</span><span class="sxs-lookup"><span data-stu-id="99a35-201">Recipient collection</span></span>|<span data-ttu-id="99a35-202">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="99a35-202">The To recipients for the message.</span></span> |

<span data-ttu-id="99a35-203">由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有 **邮件** 实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="99a35-203">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="99a35-204">响应</span><span class="sxs-lookup"><span data-stu-id="99a35-204">Response</span></span>

<span data-ttu-id="99a35-205">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99a35-205">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99a35-206">示例</span><span class="sxs-lookup"><span data-stu-id="99a35-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99a35-207">请求</span><span class="sxs-lookup"><span data-stu-id="99a35-207">Request</span></span>
<span data-ttu-id="99a35-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99a35-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99a35-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="99a35-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
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
# <a name="c"></a>[<span data-ttu-id="99a35-210">C#</span><span class="sxs-lookup"><span data-stu-id="99a35-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99a35-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99a35-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99a35-212">Java</span><span class="sxs-lookup"><span data-stu-id="99a35-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99a35-213">响应</span><span class="sxs-lookup"><span data-stu-id="99a35-213">Response</span></span>
<span data-ttu-id="99a35-214">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99a35-214">Here is an example of the response.</span></span> <span data-ttu-id="99a35-215">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="99a35-215">Note: The response object shown here might be shortened for readability.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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

## <a name="see-also"></a><span data-ttu-id="99a35-216">另请参阅</span><span class="sxs-lookup"><span data-stu-id="99a35-216">See also</span></span>

- [<span data-ttu-id="99a35-217">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="99a35-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="99a35-218">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="99a35-218">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="99a35-219">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="99a35-219">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


