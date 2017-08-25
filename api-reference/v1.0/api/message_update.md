# <a name="update-message"></a><span data-ttu-id="e9397-101">更新邮件</span><span class="sxs-lookup"><span data-stu-id="e9397-101">Update message</span></span>

<span data-ttu-id="e9397-102">更新 message 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e9397-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9397-103">权限</span><span class="sxs-lookup"><span data-stu-id="e9397-103">Permissions</span></span>
<span data-ttu-id="e9397-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e9397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e9397-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9397-106">Permission type</span></span>      | <span data-ttu-id="e9397-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9397-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e9397-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9397-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e9397-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9397-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="e9397-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9397-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9397-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9397-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="e9397-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9397-112">Application</span></span> | <span data-ttu-id="e9397-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9397-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e9397-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9397-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e9397-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9397-115">Request headers</span></span>
| <span data-ttu-id="e9397-116">名称</span><span class="sxs-lookup"><span data-stu-id="e9397-116">Name</span></span>       | <span data-ttu-id="e9397-117">类型</span><span class="sxs-lookup"><span data-stu-id="e9397-117">Type</span></span> | <span data-ttu-id="e9397-118">说明</span><span class="sxs-lookup"><span data-stu-id="e9397-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e9397-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9397-119">Authorization</span></span>  | <span data-ttu-id="e9397-120">string</span><span class="sxs-lookup"><span data-stu-id="e9397-120">string</span></span>  | <span data-ttu-id="e9397-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9397-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9397-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9397-123">Content-Type</span></span> | <span data-ttu-id="e9397-124">string</span><span class="sxs-lookup"><span data-stu-id="e9397-124">string</span></span>  | <span data-ttu-id="e9397-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="e9397-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="e9397-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9397-127">Request body</span></span>
<span data-ttu-id="e9397-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性</span><span class="sxs-lookup"><span data-stu-id="e9397-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="e9397-132">属性</span><span class="sxs-lookup"><span data-stu-id="e9397-132">Property</span></span>     | <span data-ttu-id="e9397-133">类型</span><span class="sxs-lookup"><span data-stu-id="e9397-133">Type</span></span>   |<span data-ttu-id="e9397-134">说明</span><span class="sxs-lookup"><span data-stu-id="e9397-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9397-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="e9397-135">bccRecipients</span></span>|<span data-ttu-id="e9397-136">Recipient</span><span class="sxs-lookup"><span data-stu-id="e9397-136">Recipient</span></span>|<span data-ttu-id="e9397-p105">邮件的密件抄送收件人。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p105">The Bcc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-139">categories</span><span class="sxs-lookup"><span data-stu-id="e9397-139">categories</span></span>|<span data-ttu-id="e9397-140">String collection</span><span class="sxs-lookup"><span data-stu-id="e9397-140">String collection</span></span>|<span data-ttu-id="e9397-141">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="e9397-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="e9397-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="e9397-142">ccRecipients</span></span>|<span data-ttu-id="e9397-143">收件人集合</span><span class="sxs-lookup"><span data-stu-id="e9397-143">Recipient collection</span></span>|<span data-ttu-id="e9397-p106">邮件的抄送收件人。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p106">The Cc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-146">from</span><span class="sxs-lookup"><span data-stu-id="e9397-146">from</span></span>|<span data-ttu-id="e9397-147">Recipient</span><span class="sxs-lookup"><span data-stu-id="e9397-147">Recipient</span></span>|<span data-ttu-id="e9397-p107">邮箱所有者和邮件发件人。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p107">The mailbox owner and sender of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-150">importance</span><span class="sxs-lookup"><span data-stu-id="e9397-150">importance</span></span>|<span data-ttu-id="e9397-151">String</span><span class="sxs-lookup"><span data-stu-id="e9397-151">String</span></span>|<span data-ttu-id="e9397-p108">邮件的重要性。可能的值是：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="e9397-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="e9397-154">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="e9397-154">inferenceClassification</span></span> | <span data-ttu-id="e9397-155">String</span><span class="sxs-lookup"><span data-stu-id="e9397-155">String</span></span> | <span data-ttu-id="e9397-p109">根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="e9397-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="e9397-158">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="e9397-158">internetMessageId</span></span> |<span data-ttu-id="e9397-159">String</span><span class="sxs-lookup"><span data-stu-id="e9397-159">String</span></span> |<span data-ttu-id="e9397-p110">由 [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p110">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-162">isRead</span><span class="sxs-lookup"><span data-stu-id="e9397-162">isRead</span></span>|<span data-ttu-id="e9397-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9397-163">Boolean</span></span>|<span data-ttu-id="e9397-164">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="e9397-164">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="e9397-165">replyTo</span><span class="sxs-lookup"><span data-stu-id="e9397-165">replyTo</span></span>|<span data-ttu-id="e9397-166">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="e9397-166">Recipient collection</span></span>|<span data-ttu-id="e9397-p111">在答复时使用的电子邮件地址。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p111">The email addresses to use when replying. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-169">sender</span><span class="sxs-lookup"><span data-stu-id="e9397-169">sender</span></span>|<span data-ttu-id="e9397-170">Recipient</span><span class="sxs-lookup"><span data-stu-id="e9397-170">Recipient</span></span>|<span data-ttu-id="e9397-p112">实际用于生成邮件的帐户。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p112">The account that is actually used to generate the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-173">toRecipients</span><span class="sxs-lookup"><span data-stu-id="e9397-173">toRecipients</span></span>|<span data-ttu-id="e9397-174">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="e9397-174">Recipient collection</span></span>|<span data-ttu-id="e9397-p113">邮件的收件人。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p113">The To recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-177">正文</span><span class="sxs-lookup"><span data-stu-id="e9397-177">body</span></span>|<span data-ttu-id="e9397-178">ItemBody</span><span class="sxs-lookup"><span data-stu-id="e9397-178">ItemBody</span></span>|<span data-ttu-id="e9397-p114">邮件的正文。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p114">The body of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="e9397-181">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e9397-181">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="e9397-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9397-182">Boolean</span></span>|<span data-ttu-id="e9397-183">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="e9397-183">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="e9397-184">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="e9397-184">isReadReceiptRequested</span></span>|<span data-ttu-id="e9397-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9397-185">Boolean</span></span>|<span data-ttu-id="e9397-186">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="e9397-186">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="e9397-187">subject</span><span class="sxs-lookup"><span data-stu-id="e9397-187">subject</span></span>|<span data-ttu-id="e9397-188">String</span><span class="sxs-lookup"><span data-stu-id="e9397-188">String</span></span>|<span data-ttu-id="e9397-p115">邮件的主题。仅当 IsDraft = true 时可以更新。</span><span class="sxs-lookup"><span data-stu-id="e9397-p115">The subject of the message. Updatable only if IsDraft = true.</span></span>|

<span data-ttu-id="e9397-191">由于**邮件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。</span><span class="sxs-lookup"><span data-stu-id="e9397-191">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="e9397-192">响应</span><span class="sxs-lookup"><span data-stu-id="e9397-192">Response</span></span>

<span data-ttu-id="e9397-193">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9397-193">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9397-194">示例</span><span class="sxs-lookup"><span data-stu-id="e9397-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9397-195">请求</span><span class="sxs-lookup"><span data-stu-id="e9397-195">Request</span></span>
<span data-ttu-id="e9397-196">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9397-196">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e9397-197">响应</span><span class="sxs-lookup"><span data-stu-id="e9397-197">Response</span></span>
<span data-ttu-id="e9397-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9397-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e9397-201">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e9397-201">See also</span></span>

- [<span data-ttu-id="e9397-202">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e9397-202">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e9397-203">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="e9397-203">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
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
