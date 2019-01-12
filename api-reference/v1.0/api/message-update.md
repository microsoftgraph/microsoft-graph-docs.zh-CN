---
title: 更新邮件
description: 更新 message 对象的属性。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: c3564d5f48cb3b3e12e18a07d605fcd3eba01291
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922541"
---
# <a name="update-message"></a><span data-ttu-id="7e58e-103">更新邮件</span><span class="sxs-lookup"><span data-stu-id="7e58e-103">Update message</span></span>

<span data-ttu-id="7e58e-104">更新消息对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e58e-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e58e-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e58e-105">Permissions</span></span>
<span data-ttu-id="7e58e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e58e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e58e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e58e-108">Permission type</span></span>      | <span data-ttu-id="7e58e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e58e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e58e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e58e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e58e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e58e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7e58e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e58e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e58e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e58e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7e58e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e58e-114">Application</span></span> | <span data-ttu-id="7e58e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e58e-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e58e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e58e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7e58e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e58e-117">Request headers</span></span>
| <span data-ttu-id="7e58e-118">名称</span><span class="sxs-lookup"><span data-stu-id="7e58e-118">Name</span></span>       | <span data-ttu-id="7e58e-119">类型</span><span class="sxs-lookup"><span data-stu-id="7e58e-119">Type</span></span> | <span data-ttu-id="7e58e-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e58e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7e58e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e58e-121">Authorization</span></span>  | <span data-ttu-id="7e58e-122">string</span><span class="sxs-lookup"><span data-stu-id="7e58e-122">string</span></span>  | <span data-ttu-id="7e58e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e58e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e58e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e58e-125">Content-Type</span></span> | <span data-ttu-id="7e58e-126">string</span><span class="sxs-lookup"><span data-stu-id="7e58e-126">string</span></span>  | <span data-ttu-id="7e58e-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="7e58e-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="7e58e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e58e-129">Request body</span></span>
<span data-ttu-id="7e58e-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="7e58e-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7e58e-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="7e58e-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7e58e-132">为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7e58e-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="7e58e-133">以下属性可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="7e58e-133">The following properties can be updated.</span></span>

| <span data-ttu-id="7e58e-134">属性</span><span class="sxs-lookup"><span data-stu-id="7e58e-134">Property</span></span>     | <span data-ttu-id="7e58e-135">类型</span><span class="sxs-lookup"><span data-stu-id="7e58e-135">Type</span></span>   |<span data-ttu-id="7e58e-136">说明</span><span class="sxs-lookup"><span data-stu-id="7e58e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e58e-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="7e58e-137">bccRecipients</span></span>|<span data-ttu-id="7e58e-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="7e58e-138">Recipient</span></span>|<span data-ttu-id="7e58e-139">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="7e58e-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="7e58e-140">body</span><span class="sxs-lookup"><span data-stu-id="7e58e-140">body</span></span>|<span data-ttu-id="7e58e-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="7e58e-141">ItemBody</span></span>|<span data-ttu-id="7e58e-142">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="7e58e-142">The body of the message.</span></span> <span data-ttu-id="7e58e-143">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="7e58e-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7e58e-144">categories</span><span class="sxs-lookup"><span data-stu-id="7e58e-144">categories</span></span>|<span data-ttu-id="7e58e-145">String collection</span><span class="sxs-lookup"><span data-stu-id="7e58e-145">String collection</span></span>|<span data-ttu-id="7e58e-146">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="7e58e-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="7e58e-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="7e58e-147">ccRecipients</span></span>|<span data-ttu-id="7e58e-148">收件人集合</span><span class="sxs-lookup"><span data-stu-id="7e58e-148">Recipient collection</span></span>|<span data-ttu-id="7e58e-149">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="7e58e-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="7e58e-150">发件人</span><span class="sxs-lookup"><span data-stu-id="7e58e-150">from</span></span>|<span data-ttu-id="7e58e-151">Recipient</span><span class="sxs-lookup"><span data-stu-id="7e58e-151">Recipient</span></span>|<span data-ttu-id="7e58e-152">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="7e58e-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="7e58e-153">必须为实际的邮箱使用相对应。</span><span class="sxs-lookup"><span data-stu-id="7e58e-153">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="7e58e-154">importance</span><span class="sxs-lookup"><span data-stu-id="7e58e-154">importance</span></span>|<span data-ttu-id="7e58e-155">String</span><span class="sxs-lookup"><span data-stu-id="7e58e-155">String</span></span>|<span data-ttu-id="7e58e-156">邮件的重要性。</span><span class="sxs-lookup"><span data-stu-id="7e58e-156">The importance of the message.</span></span> <span data-ttu-id="7e58e-157">可能的值为： `Low`， `Normal`， `High`。</span><span class="sxs-lookup"><span data-stu-id="7e58e-157">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="7e58e-158">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="7e58e-158">inferenceClassification</span></span> | <span data-ttu-id="7e58e-159">字符串</span><span class="sxs-lookup"><span data-stu-id="7e58e-159">String</span></span> | <span data-ttu-id="7e58e-160">为用户、 基于推测的相关性或重要性-或显式重写的邮件分类。</span><span class="sxs-lookup"><span data-stu-id="7e58e-160">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="7e58e-161">可能的值为：`focused`或`other`。</span><span class="sxs-lookup"><span data-stu-id="7e58e-161">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="7e58e-162">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="7e58e-162">internetMessageId</span></span> |<span data-ttu-id="7e58e-163">String</span><span class="sxs-lookup"><span data-stu-id="7e58e-163">String</span></span> |<span data-ttu-id="7e58e-164">由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。</span><span class="sxs-lookup"><span data-stu-id="7e58e-164">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="7e58e-165">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="7e58e-165">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7e58e-166">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="7e58e-166">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="7e58e-167">布尔</span><span class="sxs-lookup"><span data-stu-id="7e58e-167">Boolean</span></span>|<span data-ttu-id="7e58e-168">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="7e58e-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="7e58e-169">isRead</span><span class="sxs-lookup"><span data-stu-id="7e58e-169">isRead</span></span>|<span data-ttu-id="7e58e-170">布尔</span><span class="sxs-lookup"><span data-stu-id="7e58e-170">Boolean</span></span>|<span data-ttu-id="7e58e-171">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="7e58e-171">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="7e58e-172">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="7e58e-172">isReadReceiptRequested</span></span>|<span data-ttu-id="7e58e-173">布尔</span><span class="sxs-lookup"><span data-stu-id="7e58e-173">Boolean</span></span>|<span data-ttu-id="7e58e-174">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="7e58e-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="7e58e-175">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7e58e-175">multiValueExtendedProperties</span></span>|<span data-ttu-id="7e58e-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e58e-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7e58e-177">多值为消息定义的扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="7e58e-177">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="7e58e-178">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7e58e-178">Nullable.</span></span>|
|<span data-ttu-id="7e58e-179">replyTo</span><span class="sxs-lookup"><span data-stu-id="7e58e-179">replyTo</span></span>|<span data-ttu-id="7e58e-180">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="7e58e-180">Recipient collection</span></span>|<span data-ttu-id="7e58e-181">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7e58e-181">The email addresses to use when replying.</span></span> <span data-ttu-id="7e58e-182">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="7e58e-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7e58e-183">sender</span><span class="sxs-lookup"><span data-stu-id="7e58e-183">sender</span></span>|<span data-ttu-id="7e58e-184">Recipient</span><span class="sxs-lookup"><span data-stu-id="7e58e-184">Recipient</span></span>|<span data-ttu-id="7e58e-185">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="7e58e-185">The account that is actually used to generate the message.</span></span> <span data-ttu-id="7e58e-186">从[共享的邮箱](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)，或作为[委派](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送一条消息发送邮件时可更新。</span><span class="sxs-lookup"><span data-stu-id="7e58e-186">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="7e58e-187">在任何情况下的值必须为实际的邮箱使用对应。</span><span class="sxs-lookup"><span data-stu-id="7e58e-187">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="7e58e-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7e58e-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="7e58e-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="7e58e-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7e58e-190">为消息定义的单值扩展属性的集合。</span><span class="sxs-lookup"><span data-stu-id="7e58e-190">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="7e58e-191">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7e58e-191">Nullable.</span></span>|
|<span data-ttu-id="7e58e-192">subject</span><span class="sxs-lookup"><span data-stu-id="7e58e-192">subject</span></span>|<span data-ttu-id="7e58e-193">String</span><span class="sxs-lookup"><span data-stu-id="7e58e-193">String</span></span>|<span data-ttu-id="7e58e-194">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="7e58e-194">The subject of the message.</span></span> <span data-ttu-id="7e58e-195">可更新才 isDraft = true。</span><span class="sxs-lookup"><span data-stu-id="7e58e-195">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7e58e-196">toRecipients</span><span class="sxs-lookup"><span data-stu-id="7e58e-196">toRecipients</span></span>|<span data-ttu-id="7e58e-197">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="7e58e-197">Recipient collection</span></span>|<span data-ttu-id="7e58e-198">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="7e58e-198">The To recipients for the message.</span></span>|

<span data-ttu-id="7e58e-199">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="7e58e-199">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="7e58e-200">响应</span><span class="sxs-lookup"><span data-stu-id="7e58e-200">Response</span></span>

<span data-ttu-id="7e58e-201">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e58e-201">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e58e-202">示例</span><span class="sxs-lookup"><span data-stu-id="7e58e-202">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e58e-203">请求</span><span class="sxs-lookup"><span data-stu-id="7e58e-203">Request</span></span>
<span data-ttu-id="7e58e-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e58e-204">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="7e58e-205">响应</span><span class="sxs-lookup"><span data-stu-id="7e58e-205">Response</span></span>
<span data-ttu-id="7e58e-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e58e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7e58e-209">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7e58e-209">See also</span></span>

- [<span data-ttu-id="7e58e-210">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7e58e-210">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7e58e-211">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7e58e-211">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
