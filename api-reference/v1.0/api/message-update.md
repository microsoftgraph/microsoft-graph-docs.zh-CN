---
title: 更新邮件
description: 更新 message 对象的属性。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9b79ec015cbfdb5172f5b43ae728100faea0c586
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511472"
---
# <a name="update-message"></a><span data-ttu-id="5436d-103">更新邮件</span><span class="sxs-lookup"><span data-stu-id="5436d-103">Update message</span></span>

<span data-ttu-id="5436d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5436d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5436d-105">更新 message 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5436d-105">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5436d-106">权限</span><span class="sxs-lookup"><span data-stu-id="5436d-106">Permissions</span></span>
<span data-ttu-id="5436d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5436d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5436d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5436d-109">Permission type</span></span>      | <span data-ttu-id="5436d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5436d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5436d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5436d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5436d-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5436d-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5436d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5436d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5436d-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5436d-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5436d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5436d-115">Application</span></span> | <span data-ttu-id="5436d-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5436d-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5436d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5436d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5436d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5436d-118">Request headers</span></span>
| <span data-ttu-id="5436d-119">名称</span><span class="sxs-lookup"><span data-stu-id="5436d-119">Name</span></span>       | <span data-ttu-id="5436d-120">类型</span><span class="sxs-lookup"><span data-stu-id="5436d-120">Type</span></span> | <span data-ttu-id="5436d-121">说明</span><span class="sxs-lookup"><span data-stu-id="5436d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5436d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5436d-122">Authorization</span></span>  | <span data-ttu-id="5436d-123">string</span><span class="sxs-lookup"><span data-stu-id="5436d-123">string</span></span>  | <span data-ttu-id="5436d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5436d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5436d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5436d-126">Content-Type</span></span> | <span data-ttu-id="5436d-127">string</span><span class="sxs-lookup"><span data-stu-id="5436d-127">string</span></span>  | <span data-ttu-id="5436d-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="5436d-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="5436d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5436d-130">Request body</span></span>
<span data-ttu-id="5436d-131">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5436d-131">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5436d-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5436d-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5436d-133">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="5436d-133">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="5436d-134">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="5436d-134">The following properties can be updated.</span></span>

| <span data-ttu-id="5436d-135">属性</span><span class="sxs-lookup"><span data-stu-id="5436d-135">Property</span></span>     | <span data-ttu-id="5436d-136">类型</span><span class="sxs-lookup"><span data-stu-id="5436d-136">Type</span></span>   |<span data-ttu-id="5436d-137">说明</span><span class="sxs-lookup"><span data-stu-id="5436d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5436d-138">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="5436d-138">bccRecipients</span></span>|<span data-ttu-id="5436d-139">收件人</span><span class="sxs-lookup"><span data-stu-id="5436d-139">Recipient</span></span>|<span data-ttu-id="5436d-140">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="5436d-140">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="5436d-141">body</span><span class="sxs-lookup"><span data-stu-id="5436d-141">body</span></span>|<span data-ttu-id="5436d-142">ItemBody</span><span class="sxs-lookup"><span data-stu-id="5436d-142">ItemBody</span></span>|<span data-ttu-id="5436d-143">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="5436d-143">The body of the message.</span></span> <span data-ttu-id="5436d-144">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="5436d-144">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="5436d-145">categories</span><span class="sxs-lookup"><span data-stu-id="5436d-145">categories</span></span>|<span data-ttu-id="5436d-146">String collection</span><span class="sxs-lookup"><span data-stu-id="5436d-146">String collection</span></span>|<span data-ttu-id="5436d-147">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="5436d-147">The categories associated with the message.</span></span>|
|<span data-ttu-id="5436d-148">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="5436d-148">ccRecipients</span></span>|<span data-ttu-id="5436d-149">收件人集合</span><span class="sxs-lookup"><span data-stu-id="5436d-149">Recipient collection</span></span>|<span data-ttu-id="5436d-150">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="5436d-150">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="5436d-151">flag</span><span class="sxs-lookup"><span data-stu-id="5436d-151">flag</span></span>|[<span data-ttu-id="5436d-152">followupFlag</span><span class="sxs-lookup"><span data-stu-id="5436d-152">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="5436d-153">指示邮件的状态、开始日期、截止日期或完成日期的标志值。</span><span class="sxs-lookup"><span data-stu-id="5436d-153">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="5436d-154">发件人</span><span class="sxs-lookup"><span data-stu-id="5436d-154">from</span></span>|<span data-ttu-id="5436d-155">收件人</span><span class="sxs-lookup"><span data-stu-id="5436d-155">Recipient</span></span>|<span data-ttu-id="5436d-156">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="5436d-156">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="5436d-157">必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="5436d-157">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="5436d-158">importance</span><span class="sxs-lookup"><span data-stu-id="5436d-158">importance</span></span>|<span data-ttu-id="5436d-159">String</span><span class="sxs-lookup"><span data-stu-id="5436d-159">String</span></span>|<span data-ttu-id="5436d-160">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="5436d-160">The importance of the message.</span></span> <span data-ttu-id="5436d-161">可能的值包括 `Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="5436d-161">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="5436d-162">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="5436d-162">inferenceClassification</span></span> | <span data-ttu-id="5436d-163">String</span><span class="sxs-lookup"><span data-stu-id="5436d-163">String</span></span> | <span data-ttu-id="5436d-164">根据推导出的相关性或重要性或根据显式重写，对用户邮件的分类。</span><span class="sxs-lookup"><span data-stu-id="5436d-164">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="5436d-165">可能的值为：`focused` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="5436d-165">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="5436d-166">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="5436d-166">internetMessageId</span></span> |<span data-ttu-id="5436d-167">String</span><span class="sxs-lookup"><span data-stu-id="5436d-167">String</span></span> |<span data-ttu-id="5436d-168">由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="5436d-168">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="5436d-169">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="5436d-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="5436d-170">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5436d-170">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="5436d-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="5436d-171">Boolean</span></span>|<span data-ttu-id="5436d-172">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="5436d-172">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="5436d-173">isRead</span><span class="sxs-lookup"><span data-stu-id="5436d-173">isRead</span></span>|<span data-ttu-id="5436d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="5436d-174">Boolean</span></span>|<span data-ttu-id="5436d-175">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="5436d-175">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="5436d-176">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="5436d-176">isReadReceiptRequested</span></span>|<span data-ttu-id="5436d-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="5436d-177">Boolean</span></span>|<span data-ttu-id="5436d-178">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="5436d-178">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="5436d-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5436d-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="5436d-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5436d-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5436d-181">为邮件定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="5436d-181">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="5436d-182">可为空。</span><span class="sxs-lookup"><span data-stu-id="5436d-182">Nullable.</span></span>|
|<span data-ttu-id="5436d-183">replyTo</span><span class="sxs-lookup"><span data-stu-id="5436d-183">replyTo</span></span>|<span data-ttu-id="5436d-184">收件人集合</span><span class="sxs-lookup"><span data-stu-id="5436d-184">Recipient collection</span></span>|<span data-ttu-id="5436d-185">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5436d-185">The email addresses to use when replying.</span></span> <span data-ttu-id="5436d-186">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="5436d-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="5436d-187">sender</span><span class="sxs-lookup"><span data-stu-id="5436d-187">sender</span></span>|<span data-ttu-id="5436d-188">收件人</span><span class="sxs-lookup"><span data-stu-id="5436d-188">Recipient</span></span>|<span data-ttu-id="5436d-189">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="5436d-189">The account that is actually used to generate the message.</span></span> <span data-ttu-id="5436d-190">从[共享邮箱](/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件或将邮件作为[委托](https://support.office.com/zh-CN/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送时可更新。</span><span class="sxs-lookup"><span data-stu-id="5436d-190">Updatable when sending a message from a [shared mailbox](/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/zh-CN/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="5436d-191">在任何情况下，此值必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="5436d-191">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="5436d-192">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5436d-192">singleValueExtendedProperties</span></span>|<span data-ttu-id="5436d-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="5436d-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5436d-p113">为邮件定义的单值扩展属性的集合。可为空。</span><span class="sxs-lookup"><span data-stu-id="5436d-p113">The collection of single-value extended properties defined for the message. Nullable.</span></span>|
|<span data-ttu-id="5436d-196">subject</span><span class="sxs-lookup"><span data-stu-id="5436d-196">subject</span></span>|<span data-ttu-id="5436d-197">String</span><span class="sxs-lookup"><span data-stu-id="5436d-197">String</span></span>|<span data-ttu-id="5436d-198">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="5436d-198">The subject of the message.</span></span> <span data-ttu-id="5436d-199">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="5436d-199">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="5436d-200">toRecipients</span><span class="sxs-lookup"><span data-stu-id="5436d-200">toRecipients</span></span>|<span data-ttu-id="5436d-201">收件人集合</span><span class="sxs-lookup"><span data-stu-id="5436d-201">Recipient collection</span></span>|<span data-ttu-id="5436d-202">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="5436d-202">The To recipients for the message.</span></span>|

<span data-ttu-id="5436d-203">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="5436d-203">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="5436d-204">响应</span><span class="sxs-lookup"><span data-stu-id="5436d-204">Response</span></span>

<span data-ttu-id="5436d-205">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5436d-205">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5436d-206">示例</span><span class="sxs-lookup"><span data-stu-id="5436d-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5436d-207">请求</span><span class="sxs-lookup"><span data-stu-id="5436d-207">Request</span></span>
<span data-ttu-id="5436d-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5436d-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5436d-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="5436d-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5436d-210">C#</span><span class="sxs-lookup"><span data-stu-id="5436d-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5436d-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5436d-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5436d-212">Java</span><span class="sxs-lookup"><span data-stu-id="5436d-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5436d-213">响应</span><span class="sxs-lookup"><span data-stu-id="5436d-213">Response</span></span>
<span data-ttu-id="5436d-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5436d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5436d-217">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5436d-217">See also</span></span>

- [<span data-ttu-id="5436d-218">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5436d-218">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5436d-219">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5436d-219">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
