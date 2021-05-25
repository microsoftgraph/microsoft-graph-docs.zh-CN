---
title: 更新邮件
description: 更新 message 对象的属性。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c9c3e9f13a592738ebd4245015a9458a0856dda8
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645337"
---
# <a name="update-message"></a><span data-ttu-id="f1a93-103">更新邮件</span><span class="sxs-lookup"><span data-stu-id="f1a93-103">Update message</span></span>

<span data-ttu-id="f1a93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1a93-105">更新 message 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f1a93-105">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1a93-106">权限</span><span class="sxs-lookup"><span data-stu-id="f1a93-106">Permissions</span></span>
<span data-ttu-id="f1a93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a93-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1a93-109">Permission type</span></span>      | <span data-ttu-id="f1a93-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1a93-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1a93-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1a93-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1a93-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a93-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f1a93-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1a93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a93-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a93-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f1a93-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1a93-115">Application</span></span> | <span data-ttu-id="f1a93-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1a93-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1a93-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1a93-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f1a93-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1a93-118">Request headers</span></span>
| <span data-ttu-id="f1a93-119">名称</span><span class="sxs-lookup"><span data-stu-id="f1a93-119">Name</span></span>       | <span data-ttu-id="f1a93-120">类型</span><span class="sxs-lookup"><span data-stu-id="f1a93-120">Type</span></span> | <span data-ttu-id="f1a93-121">说明</span><span class="sxs-lookup"><span data-stu-id="f1a93-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1a93-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1a93-122">Authorization</span></span>  | <span data-ttu-id="f1a93-123">string</span><span class="sxs-lookup"><span data-stu-id="f1a93-123">string</span></span>  | <span data-ttu-id="f1a93-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1a93-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1a93-126">Content-Type</span></span> | <span data-ttu-id="f1a93-127">string</span><span class="sxs-lookup"><span data-stu-id="f1a93-127">string</span></span>  | <span data-ttu-id="f1a93-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1a93-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1a93-130">Request body</span></span>
<span data-ttu-id="f1a93-p104">在请求正文中，提供应更新的相关属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可进行以下属性的更新。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following properties can be updated.</span></span>

| <span data-ttu-id="f1a93-135">属性</span><span class="sxs-lookup"><span data-stu-id="f1a93-135">Property</span></span>     | <span data-ttu-id="f1a93-136">类型</span><span class="sxs-lookup"><span data-stu-id="f1a93-136">Type</span></span>   |<span data-ttu-id="f1a93-137">说明</span><span class="sxs-lookup"><span data-stu-id="f1a93-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1a93-138">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="f1a93-138">bccRecipients</span></span>|<span data-ttu-id="f1a93-139">收件人</span><span class="sxs-lookup"><span data-stu-id="f1a93-139">Recipient</span></span>|<span data-ttu-id="f1a93-140">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="f1a93-140">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="f1a93-141">body</span><span class="sxs-lookup"><span data-stu-id="f1a93-141">body</span></span>|<span data-ttu-id="f1a93-142">ItemBody</span><span class="sxs-lookup"><span data-stu-id="f1a93-142">ItemBody</span></span>|<span data-ttu-id="f1a93-p105">邮件的正文。仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p105">The body of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="f1a93-145">categories</span><span class="sxs-lookup"><span data-stu-id="f1a93-145">categories</span></span>|<span data-ttu-id="f1a93-146">String collection</span><span class="sxs-lookup"><span data-stu-id="f1a93-146">String collection</span></span>|<span data-ttu-id="f1a93-147">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="f1a93-147">The categories associated with the message.</span></span>|
|<span data-ttu-id="f1a93-148">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="f1a93-148">ccRecipients</span></span>|<span data-ttu-id="f1a93-149">收件人集合</span><span class="sxs-lookup"><span data-stu-id="f1a93-149">Recipient collection</span></span>|<span data-ttu-id="f1a93-150">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="f1a93-150">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="f1a93-151">flag</span><span class="sxs-lookup"><span data-stu-id="f1a93-151">flag</span></span>|[<span data-ttu-id="f1a93-152">followupFlag</span><span class="sxs-lookup"><span data-stu-id="f1a93-152">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="f1a93-153">指示邮件的状态、开始日期、截止日期或完成日期的标志值。</span><span class="sxs-lookup"><span data-stu-id="f1a93-153">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="f1a93-154">发件人</span><span class="sxs-lookup"><span data-stu-id="f1a93-154">from</span></span>|<span data-ttu-id="f1a93-155">收件人</span><span class="sxs-lookup"><span data-stu-id="f1a93-155">Recipient</span></span>|<span data-ttu-id="f1a93-156">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="f1a93-156">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="f1a93-157">必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="f1a93-157">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="f1a93-158">importance</span><span class="sxs-lookup"><span data-stu-id="f1a93-158">importance</span></span>|<span data-ttu-id="f1a93-159">String</span><span class="sxs-lookup"><span data-stu-id="f1a93-159">String</span></span>|<span data-ttu-id="f1a93-p107">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="f1a93-162">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="f1a93-162">inferenceClassification</span></span> | <span data-ttu-id="f1a93-163">String</span><span class="sxs-lookup"><span data-stu-id="f1a93-163">String</span></span> | <span data-ttu-id="f1a93-p108">根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="f1a93-166">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="f1a93-166">internetMessageId</span></span> |<span data-ttu-id="f1a93-167">String</span><span class="sxs-lookup"><span data-stu-id="f1a93-167">String</span></span> |<span data-ttu-id="f1a93-p109">由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p109">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="f1a93-170">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f1a93-170">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="f1a93-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1a93-171">Boolean</span></span>|<span data-ttu-id="f1a93-172">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="f1a93-172">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="f1a93-173">isRead</span><span class="sxs-lookup"><span data-stu-id="f1a93-173">isRead</span></span>|<span data-ttu-id="f1a93-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1a93-174">Boolean</span></span>|<span data-ttu-id="f1a93-175">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="f1a93-175">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="f1a93-176">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="f1a93-176">isReadReceiptRequested</span></span>|<span data-ttu-id="f1a93-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1a93-177">Boolean</span></span>|<span data-ttu-id="f1a93-178">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="f1a93-178">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="f1a93-179">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f1a93-179">multiValueExtendedProperties</span></span>|<span data-ttu-id="f1a93-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1a93-180">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f1a93-p110">为邮件定义的多值扩展属性的集合。只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p110">The collection of multi-value extended properties defined for the message. Nullable.</span></span>|
|<span data-ttu-id="f1a93-183">replyTo</span><span class="sxs-lookup"><span data-stu-id="f1a93-183">replyTo</span></span>|<span data-ttu-id="f1a93-184">收件人集合</span><span class="sxs-lookup"><span data-stu-id="f1a93-184">Recipient collection</span></span>|<span data-ttu-id="f1a93-p111">在答复时使用的电子邮件地址。仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p111">The email addresses to use when replying. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="f1a93-187">sender</span><span class="sxs-lookup"><span data-stu-id="f1a93-187">sender</span></span>|<span data-ttu-id="f1a93-188">收件人</span><span class="sxs-lookup"><span data-stu-id="f1a93-188">Recipient</span></span>|<span data-ttu-id="f1a93-189">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="f1a93-189">The account that is actually used to generate the message.</span></span> <span data-ttu-id="f1a93-190">从[共享邮箱](/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件或将邮件作为[委托](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送时可更新。</span><span class="sxs-lookup"><span data-stu-id="f1a93-190">Updatable when sending a message from a [shared mailbox](/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="f1a93-191">在任何情况下，此值必须对应于使用的实际邮箱。</span><span class="sxs-lookup"><span data-stu-id="f1a93-191">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="f1a93-192">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f1a93-192">singleValueExtendedProperties</span></span>|<span data-ttu-id="f1a93-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="f1a93-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f1a93-p113">为邮件定义的单值扩展属性的集合。可为空。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p113">The collection of single-value extended properties defined for the message. Nullable.</span></span>|
|<span data-ttu-id="f1a93-196">subject</span><span class="sxs-lookup"><span data-stu-id="f1a93-196">subject</span></span>|<span data-ttu-id="f1a93-197">String</span><span class="sxs-lookup"><span data-stu-id="f1a93-197">String</span></span>|<span data-ttu-id="f1a93-p114">邮件的主题。仅当 isDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p114">The subject of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="f1a93-200">toRecipients</span><span class="sxs-lookup"><span data-stu-id="f1a93-200">toRecipients</span></span>|<span data-ttu-id="f1a93-201">收件人集合</span><span class="sxs-lookup"><span data-stu-id="f1a93-201">Recipient collection</span></span>|<span data-ttu-id="f1a93-202">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="f1a93-202">The To recipients for the message.</span></span> |

<span data-ttu-id="f1a93-203">由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)，因此可以使用 `PATCH` 操作在现有 **邮件** 实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="f1a93-203">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="f1a93-204">响应</span><span class="sxs-lookup"><span data-stu-id="f1a93-204">Response</span></span>

<span data-ttu-id="f1a93-205">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1a93-205">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1a93-206">示例</span><span class="sxs-lookup"><span data-stu-id="f1a93-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1a93-207">请求</span><span class="sxs-lookup"><span data-stu-id="f1a93-207">Request</span></span>
<span data-ttu-id="f1a93-208">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1a93-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1a93-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a93-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f1a93-210">C#</span><span class="sxs-lookup"><span data-stu-id="f1a93-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1a93-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1a93-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1a93-212">Java</span><span class="sxs-lookup"><span data-stu-id="f1a93-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1a93-213">响应</span><span class="sxs-lookup"><span data-stu-id="f1a93-213">Response</span></span>
<span data-ttu-id="f1a93-p115">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f1a93-p115">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f1a93-216">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f1a93-216">See also</span></span>

- [<span data-ttu-id="f1a93-217">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f1a93-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f1a93-218">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="f1a93-218">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f1a93-219">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="f1a93-219">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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


