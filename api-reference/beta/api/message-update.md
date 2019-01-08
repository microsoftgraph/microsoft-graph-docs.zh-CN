---
title: 更新邮件
description: 更新 message 对象的属性。
author: angelgolfer-ms
ms.openlocfilehash: 04a52e28728eda7d778ac76cdc69080cd5b9edf5
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748540"
---
# <a name="update-message"></a><span data-ttu-id="59366-103">更新邮件</span><span class="sxs-lookup"><span data-stu-id="59366-103">Update message</span></span>

> <span data-ttu-id="59366-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="59366-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59366-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="59366-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59366-106">更新消息对象的属性。</span><span class="sxs-lookup"><span data-stu-id="59366-106">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="59366-107">权限</span><span class="sxs-lookup"><span data-stu-id="59366-107">Permissions</span></span>
<span data-ttu-id="59366-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59366-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59366-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59366-110">Permission type</span></span>      | <span data-ttu-id="59366-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59366-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59366-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59366-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59366-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59366-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="59366-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59366-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59366-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59366-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="59366-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59366-116">Application</span></span> | <span data-ttu-id="59366-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59366-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59366-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59366-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="59366-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59366-119">Request headers</span></span>
| <span data-ttu-id="59366-120">名称</span><span class="sxs-lookup"><span data-stu-id="59366-120">Name</span></span>       | <span data-ttu-id="59366-121">类型</span><span class="sxs-lookup"><span data-stu-id="59366-121">Type</span></span> | <span data-ttu-id="59366-122">说明</span><span class="sxs-lookup"><span data-stu-id="59366-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59366-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59366-123">Authorization</span></span>  | <span data-ttu-id="59366-124">string</span><span class="sxs-lookup"><span data-stu-id="59366-124">string</span></span>  | <span data-ttu-id="59366-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59366-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59366-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59366-127">Content-Type</span></span> | <span data-ttu-id="59366-128">string</span><span class="sxs-lookup"><span data-stu-id="59366-128">string</span></span>  | <span data-ttu-id="59366-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="59366-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="59366-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="59366-131">Request body</span></span>
<span data-ttu-id="59366-132">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="59366-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="59366-133">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="59366-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="59366-134">为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="59366-134">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="59366-135">以下属性可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="59366-135">The following properties can be updated.</span></span>

| <span data-ttu-id="59366-136">属性</span><span class="sxs-lookup"><span data-stu-id="59366-136">Property</span></span>     | <span data-ttu-id="59366-137">类型</span><span class="sxs-lookup"><span data-stu-id="59366-137">Type</span></span>   |<span data-ttu-id="59366-138">说明</span><span class="sxs-lookup"><span data-stu-id="59366-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59366-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="59366-139">bccRecipients</span></span>|<span data-ttu-id="59366-140">Recipient</span><span class="sxs-lookup"><span data-stu-id="59366-140">Recipient</span></span>|<span data-ttu-id="59366-141">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="59366-141">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="59366-142">body</span><span class="sxs-lookup"><span data-stu-id="59366-142">body</span></span>|<span data-ttu-id="59366-143">ItemBody</span><span class="sxs-lookup"><span data-stu-id="59366-143">ItemBody</span></span>|<span data-ttu-id="59366-144">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="59366-144">The body of the message.</span></span> <span data-ttu-id="59366-145">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="59366-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="59366-146">categories</span><span class="sxs-lookup"><span data-stu-id="59366-146">categories</span></span>|<span data-ttu-id="59366-147">String collection</span><span class="sxs-lookup"><span data-stu-id="59366-147">String collection</span></span>|<span data-ttu-id="59366-148">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="59366-148">The categories associated with the message.</span></span>|
|<span data-ttu-id="59366-149">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="59366-149">ccRecipients</span></span>|<span data-ttu-id="59366-150">收件人集合</span><span class="sxs-lookup"><span data-stu-id="59366-150">Recipient collection</span></span>|<span data-ttu-id="59366-151">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="59366-151">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="59366-152">发件人</span><span class="sxs-lookup"><span data-stu-id="59366-152">from</span></span>|<span data-ttu-id="59366-153">Recipient</span><span class="sxs-lookup"><span data-stu-id="59366-153">Recipient</span></span>|<span data-ttu-id="59366-154">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="59366-154">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="59366-155">必须为实际的邮箱使用相对应。</span><span class="sxs-lookup"><span data-stu-id="59366-155">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="59366-156">importance</span><span class="sxs-lookup"><span data-stu-id="59366-156">importance</span></span>|<span data-ttu-id="59366-157">String</span><span class="sxs-lookup"><span data-stu-id="59366-157">String</span></span>|<span data-ttu-id="59366-p108">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="59366-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="59366-160">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="59366-160">inferenceClassification</span></span> | <span data-ttu-id="59366-161">String</span><span class="sxs-lookup"><span data-stu-id="59366-161">String</span></span> | <span data-ttu-id="59366-p109">根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="59366-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="59366-164">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="59366-164">internetMessageId</span></span> |<span data-ttu-id="59366-165">String</span><span class="sxs-lookup"><span data-stu-id="59366-165">String</span></span> |<span data-ttu-id="59366-166">由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="59366-166">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="59366-167">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="59366-167">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="59366-168">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="59366-168">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="59366-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="59366-169">Boolean</span></span>|<span data-ttu-id="59366-170">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="59366-170">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="59366-171">isRead</span><span class="sxs-lookup"><span data-stu-id="59366-171">isRead</span></span>|<span data-ttu-id="59366-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="59366-172">Boolean</span></span>|<span data-ttu-id="59366-173">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="59366-173">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="59366-174">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="59366-174">isReadReceiptRequested</span></span>|<span data-ttu-id="59366-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="59366-175">Boolean</span></span>|<span data-ttu-id="59366-176">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="59366-176">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="59366-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="59366-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="59366-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59366-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="59366-179">多值为消息定义的扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="59366-179">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="59366-180">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="59366-180">Nullable.</span></span>|
|<span data-ttu-id="59366-181">replyTo</span><span class="sxs-lookup"><span data-stu-id="59366-181">replyTo</span></span>|<span data-ttu-id="59366-182">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="59366-182">Recipient collection</span></span>|<span data-ttu-id="59366-183">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="59366-183">The email addresses to use when replying.</span></span> <span data-ttu-id="59366-184">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="59366-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="59366-185">sender</span><span class="sxs-lookup"><span data-stu-id="59366-185">sender</span></span>|<span data-ttu-id="59366-186">Recipient</span><span class="sxs-lookup"><span data-stu-id="59366-186">Recipient</span></span>|<span data-ttu-id="59366-187">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="59366-187">The account that is actually used to generate the message.</span></span> <span data-ttu-id="59366-188">从[共享的邮箱](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)，或作为[委派](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送一条消息发送邮件时可更新。</span><span class="sxs-lookup"><span data-stu-id="59366-188">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="59366-189">在任何情况下的值必须为实际的邮箱使用对应。</span><span class="sxs-lookup"><span data-stu-id="59366-189">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="59366-190">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="59366-190">singleValueExtendedProperties</span></span>|<span data-ttu-id="59366-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="59366-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="59366-192">为消息定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="59366-192">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="59366-193">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="59366-193">Nullable.</span></span>|
|<span data-ttu-id="59366-194">subject</span><span class="sxs-lookup"><span data-stu-id="59366-194">subject</span></span>|<span data-ttu-id="59366-195">String</span><span class="sxs-lookup"><span data-stu-id="59366-195">String</span></span>|<span data-ttu-id="59366-196">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="59366-196">The subject of the message.</span></span> <span data-ttu-id="59366-197">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="59366-197">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="59366-198">toRecipients</span><span class="sxs-lookup"><span data-stu-id="59366-198">toRecipients</span></span>|<span data-ttu-id="59366-199">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="59366-199">Recipient collection</span></span>|<span data-ttu-id="59366-200">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="59366-200">The To recipients for the message.</span></span> |

<span data-ttu-id="59366-201">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="59366-201">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="59366-202">响应</span><span class="sxs-lookup"><span data-stu-id="59366-202">Response</span></span>

<span data-ttu-id="59366-203">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59366-203">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59366-204">示例</span><span class="sxs-lookup"><span data-stu-id="59366-204">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59366-205">请求</span><span class="sxs-lookup"><span data-stu-id="59366-205">Request</span></span>
<span data-ttu-id="59366-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59366-206">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="59366-207">响应</span><span class="sxs-lookup"><span data-stu-id="59366-207">Response</span></span>
<span data-ttu-id="59366-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59366-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="59366-211">另请参阅</span><span class="sxs-lookup"><span data-stu-id="59366-211">See also</span></span>

- [<span data-ttu-id="59366-212">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="59366-212">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="59366-213">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="59366-213">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="59366-214">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="59366-214">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
