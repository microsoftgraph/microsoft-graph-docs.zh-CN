---
title: 更新邮件
description: 更新 message 对象的属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cb9145235a0ba4b45df5f0f89679aac68d76e98f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992820"
---
# <a name="update-message"></a><span data-ttu-id="a79fd-103">更新邮件</span><span class="sxs-lookup"><span data-stu-id="a79fd-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a79fd-104">更新 message 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a79fd-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a79fd-105">权限</span><span class="sxs-lookup"><span data-stu-id="a79fd-105">Permissions</span></span>
<span data-ttu-id="a79fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a79fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a79fd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a79fd-108">Permission type</span></span>      | <span data-ttu-id="a79fd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a79fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a79fd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a79fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a79fd-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a79fd-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a79fd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a79fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a79fd-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a79fd-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a79fd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a79fd-114">Application</span></span> | <span data-ttu-id="a79fd-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a79fd-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a79fd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a79fd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a79fd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a79fd-117">Request headers</span></span>
| <span data-ttu-id="a79fd-118">名称</span><span class="sxs-lookup"><span data-stu-id="a79fd-118">Name</span></span>       | <span data-ttu-id="a79fd-119">类型</span><span class="sxs-lookup"><span data-stu-id="a79fd-119">Type</span></span> | <span data-ttu-id="a79fd-120">说明</span><span class="sxs-lookup"><span data-stu-id="a79fd-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a79fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a79fd-121">Authorization</span></span>  | <span data-ttu-id="a79fd-122">string</span><span class="sxs-lookup"><span data-stu-id="a79fd-122">string</span></span>  | <span data-ttu-id="a79fd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a79fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a79fd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a79fd-125">Content-Type</span></span> | <span data-ttu-id="a79fd-126">string</span><span class="sxs-lookup"><span data-stu-id="a79fd-126">string</span></span>  | <span data-ttu-id="a79fd-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="a79fd-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="a79fd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a79fd-129">Request body</span></span>
<span data-ttu-id="a79fd-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a79fd-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a79fd-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a79fd-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a79fd-132">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="a79fd-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="a79fd-133">可更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="a79fd-133">The following properties can be updated.</span></span>

| <span data-ttu-id="a79fd-134">属性</span><span class="sxs-lookup"><span data-stu-id="a79fd-134">Property</span></span>     | <span data-ttu-id="a79fd-135">类型</span><span class="sxs-lookup"><span data-stu-id="a79fd-135">Type</span></span>   |<span data-ttu-id="a79fd-136">说明</span><span class="sxs-lookup"><span data-stu-id="a79fd-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a79fd-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="a79fd-137">bccRecipients</span></span>|<span data-ttu-id="a79fd-138">收件人</span><span class="sxs-lookup"><span data-stu-id="a79fd-138">Recipient</span></span>|<span data-ttu-id="a79fd-139">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="a79fd-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="a79fd-140">body</span><span class="sxs-lookup"><span data-stu-id="a79fd-140">body</span></span>|<span data-ttu-id="a79fd-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="a79fd-141">ItemBody</span></span>|<span data-ttu-id="a79fd-142">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="a79fd-142">The body of the message.</span></span> <span data-ttu-id="a79fd-143">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="a79fd-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="a79fd-144">categories</span><span class="sxs-lookup"><span data-stu-id="a79fd-144">categories</span></span>|<span data-ttu-id="a79fd-145">String collection</span><span class="sxs-lookup"><span data-stu-id="a79fd-145">String collection</span></span>|<span data-ttu-id="a79fd-146">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="a79fd-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="a79fd-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="a79fd-147">ccRecipients</span></span>|<span data-ttu-id="a79fd-148">收件人集合</span><span class="sxs-lookup"><span data-stu-id="a79fd-148">Recipient collection</span></span>|<span data-ttu-id="a79fd-149">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="a79fd-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="a79fd-150">flag</span><span class="sxs-lookup"><span data-stu-id="a79fd-150">flag</span></span>|[<span data-ttu-id="a79fd-151">followupFlag</span><span class="sxs-lookup"><span data-stu-id="a79fd-151">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="a79fd-152">指示邮件的状态、开始日期、截止日期或完成日期的标志值。</span><span class="sxs-lookup"><span data-stu-id="a79fd-152">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="a79fd-153">发件人</span><span class="sxs-lookup"><span data-stu-id="a79fd-153">from</span></span>|<span data-ttu-id="a79fd-154">收件人</span><span class="sxs-lookup"><span data-stu-id="a79fd-154">Recipient</span></span>|<span data-ttu-id="a79fd-155">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="a79fd-155">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="a79fd-156">必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="a79fd-156">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="a79fd-157">importance</span><span class="sxs-lookup"><span data-stu-id="a79fd-157">importance</span></span>|<span data-ttu-id="a79fd-158">String</span><span class="sxs-lookup"><span data-stu-id="a79fd-158">String</span></span>|<span data-ttu-id="a79fd-p107">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="a79fd-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="a79fd-161">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="a79fd-161">inferenceClassification</span></span> | <span data-ttu-id="a79fd-162">String</span><span class="sxs-lookup"><span data-stu-id="a79fd-162">String</span></span> | <span data-ttu-id="a79fd-p108">根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="a79fd-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="a79fd-165">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="a79fd-165">internetMessageId</span></span> |<span data-ttu-id="a79fd-166">String</span><span class="sxs-lookup"><span data-stu-id="a79fd-166">String</span></span> |<span data-ttu-id="a79fd-167">由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="a79fd-167">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="a79fd-168">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="a79fd-168">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="a79fd-169">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="a79fd-169">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="a79fd-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="a79fd-170">Boolean</span></span>|<span data-ttu-id="a79fd-171">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="a79fd-171">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="a79fd-172">isRead</span><span class="sxs-lookup"><span data-stu-id="a79fd-172">isRead</span></span>|<span data-ttu-id="a79fd-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a79fd-173">Boolean</span></span>|<span data-ttu-id="a79fd-174">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="a79fd-174">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="a79fd-175">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="a79fd-175">isReadReceiptRequested</span></span>|<span data-ttu-id="a79fd-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="a79fd-176">Boolean</span></span>|<span data-ttu-id="a79fd-177">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="a79fd-177">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="a79fd-178">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a79fd-178">multiValueExtendedProperties</span></span>|<span data-ttu-id="a79fd-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a79fd-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a79fd-180">为邮件定义的多值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="a79fd-180">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="a79fd-181">可为空。</span><span class="sxs-lookup"><span data-stu-id="a79fd-181">Nullable.</span></span>|
|<span data-ttu-id="a79fd-182">replyTo</span><span class="sxs-lookup"><span data-stu-id="a79fd-182">replyTo</span></span>|<span data-ttu-id="a79fd-183">收件人集合</span><span class="sxs-lookup"><span data-stu-id="a79fd-183">Recipient collection</span></span>|<span data-ttu-id="a79fd-184">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a79fd-184">The email addresses to use when replying.</span></span> <span data-ttu-id="a79fd-185">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="a79fd-185">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="a79fd-186">sender</span><span class="sxs-lookup"><span data-stu-id="a79fd-186">sender</span></span>|<span data-ttu-id="a79fd-187">收件人</span><span class="sxs-lookup"><span data-stu-id="a79fd-187">Recipient</span></span>|<span data-ttu-id="a79fd-188">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="a79fd-188">The account that is actually used to generate the message.</span></span> <span data-ttu-id="a79fd-189">从[共享邮箱](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件或将邮件作为[委托](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送时可更新。</span><span class="sxs-lookup"><span data-stu-id="a79fd-189">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="a79fd-190">在任何情况下，此值必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="a79fd-190">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="a79fd-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a79fd-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="a79fd-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="a79fd-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a79fd-p113">为邮件定义的单值扩展属性的集合。可为空。</span><span class="sxs-lookup"><span data-stu-id="a79fd-p113">The collection of single-value extended properties defined for the message. Nullable.</span></span>|
|<span data-ttu-id="a79fd-195">subject</span><span class="sxs-lookup"><span data-stu-id="a79fd-195">subject</span></span>|<span data-ttu-id="a79fd-196">String</span><span class="sxs-lookup"><span data-stu-id="a79fd-196">String</span></span>|<span data-ttu-id="a79fd-197">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="a79fd-197">The subject of the message.</span></span> <span data-ttu-id="a79fd-198">仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="a79fd-198">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="a79fd-199">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a79fd-199">toRecipients</span></span>|<span data-ttu-id="a79fd-200">收件人集合</span><span class="sxs-lookup"><span data-stu-id="a79fd-200">Recipient collection</span></span>|<span data-ttu-id="a79fd-201">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="a79fd-201">The To recipients for the message.</span></span> |

<span data-ttu-id="a79fd-202">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="a79fd-202">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="a79fd-203">响应</span><span class="sxs-lookup"><span data-stu-id="a79fd-203">Response</span></span>

<span data-ttu-id="a79fd-204">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a79fd-204">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a79fd-205">示例</span><span class="sxs-lookup"><span data-stu-id="a79fd-205">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a79fd-206">请求</span><span class="sxs-lookup"><span data-stu-id="a79fd-206">Request</span></span>
<span data-ttu-id="a79fd-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a79fd-207">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a79fd-208">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a79fd-208">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a79fd-209">C#</span><span class="sxs-lookup"><span data-stu-id="a79fd-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a79fd-210">Javascript</span><span class="sxs-lookup"><span data-stu-id="a79fd-210">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a79fd-211">Java</span><span class="sxs-lookup"><span data-stu-id="a79fd-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a79fd-212">响应</span><span class="sxs-lookup"><span data-stu-id="a79fd-212">Response</span></span>
<span data-ttu-id="a79fd-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a79fd-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a79fd-216">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a79fd-216">See also</span></span>

- [<span data-ttu-id="a79fd-217">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a79fd-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a79fd-218">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a79fd-218">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a79fd-219">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="a79fd-219">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
