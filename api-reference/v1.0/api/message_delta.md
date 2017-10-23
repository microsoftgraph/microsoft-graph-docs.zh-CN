# <a name="message-delta"></a><span data-ttu-id="1630e-101">message: delta</span><span class="sxs-lookup"><span data-stu-id="1630e-101">message: delta</span></span>

<span data-ttu-id="1630e-102">获取指定文件夹中已添加、删除或更新的邮件集。</span><span class="sxs-lookup"><span data-stu-id="1630e-102">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="1630e-p101">对文件夹中的邮件的 **delta** 函数调用与 GET 请求相似，除了前者可通过在对其的一次或多次调用中正确应用[状态令牌](../../../concepts/delta_query_overview.md)来[查询该文件夹中的邮件的增量更改](../../../concepts/delta_query_messages.md)。通过此功能，你可以维护和同步本地存储的用户邮件，而无需每次都从服务器中获取整组邮件。</span><span class="sxs-lookup"><span data-stu-id="1630e-p101">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can [query for incremental changes in the messages in that folder](../../../concepts/delta_query_messages.md). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="1630e-105">权限</span><span class="sxs-lookup"><span data-stu-id="1630e-105">Permissions</span></span>
<span data-ttu-id="1630e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1630e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1630e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1630e-108">Permission type</span></span>      | <span data-ttu-id="1630e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1630e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1630e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1630e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1630e-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1630e-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1630e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1630e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1630e-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1630e-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1630e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1630e-114">Application</span></span> | <span data-ttu-id="1630e-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1630e-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1630e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1630e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/<id>/mailFolders/{id}/messages/delta
```

### <a name="query-parameters"></a><span data-ttu-id="1630e-117">查询参数</span><span class="sxs-lookup"><span data-stu-id="1630e-117">Query parameters</span></span>

<span data-ttu-id="1630e-p103">跟踪邮件更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="1630e-p103">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="1630e-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="1630e-123">Query parameter</span></span>      | <span data-ttu-id="1630e-124">类型</span><span class="sxs-lookup"><span data-stu-id="1630e-124">Type</span></span>   |<span data-ttu-id="1630e-125">说明</span><span class="sxs-lookup"><span data-stu-id="1630e-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1630e-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="1630e-126">$deltatoken</span></span> | <span data-ttu-id="1630e-127">string</span><span class="sxs-lookup"><span data-stu-id="1630e-127">string</span></span> | <span data-ttu-id="1630e-p104">对同一个邮件集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="1630e-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="1630e-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="1630e-130">$skiptoken</span></span> | <span data-ttu-id="1630e-131">string</span><span class="sxs-lookup"><span data-stu-id="1630e-131">string</span></span> | <span data-ttu-id="1630e-132">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个邮件集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="1630e-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |

#### <a name="odata-query-parameters"></a><span data-ttu-id="1630e-133">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="1630e-133">OData query parameters</span></span>

- <span data-ttu-id="1630e-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="1630e-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="1630e-136">对于邮件，Delta 查询支持 `$select`、`$top` 和 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="1630e-136">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="1630e-137">提供对 `$filter` 和 `$orderby` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="1630e-137">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="1630e-138">唯一支持的 `$filter` 表达式是 `$filter=receivedDateTime+ge+{value}` 或 `$filter=receivedDateTime+gt+{value}`。</span><span class="sxs-lookup"><span data-stu-id="1630e-138">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="1630e-p106">唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。如果不包含 `$orderby` 表达式，则不能保证返回顺序。</span><span class="sxs-lookup"><span data-stu-id="1630e-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="1630e-141">不支持 `$search`。</span><span class="sxs-lookup"><span data-stu-id="1630e-141">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1630e-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="1630e-142">Request headers</span></span>
| <span data-ttu-id="1630e-143">名称</span><span class="sxs-lookup"><span data-stu-id="1630e-143">Name</span></span>       | <span data-ttu-id="1630e-144">类型</span><span class="sxs-lookup"><span data-stu-id="1630e-144">Type</span></span> | <span data-ttu-id="1630e-145">说明</span><span class="sxs-lookup"><span data-stu-id="1630e-145">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="1630e-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="1630e-146">Authorization</span></span>  | <span data-ttu-id="1630e-147">string</span><span class="sxs-lookup"><span data-stu-id="1630e-147">string</span></span>  | <span data-ttu-id="1630e-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1630e-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1630e-150">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1630e-150">Content-Type</span></span>  | <span data-ttu-id="1630e-151">string</span><span class="sxs-lookup"><span data-stu-id="1630e-151">string</span></span>  | <span data-ttu-id="1630e-p108">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1630e-p108">application/json. Required.</span></span> |
| <span data-ttu-id="1630e-154">Prefer</span><span class="sxs-lookup"><span data-stu-id="1630e-154">Prefer</span></span> | <span data-ttu-id="1630e-155">string</span><span class="sxs-lookup"><span data-stu-id="1630e-155">string</span></span>  | <span data-ttu-id="1630e-p109">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="1630e-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1630e-158">响应</span><span class="sxs-lookup"><span data-stu-id="1630e-158">Response</span></span>

<span data-ttu-id="1630e-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="1630e-159">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1630e-160">示例</span><span class="sxs-lookup"><span data-stu-id="1630e-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1630e-161">请求</span><span class="sxs-lookup"><span data-stu-id="1630e-161">Request</span></span>
<span data-ttu-id="1630e-162">以下示例演示了如何执行单次 **delta** 函数调用，并将响应正文中的邮件最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="1630e-162">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="1630e-p110">若要跟踪文件夹中的邮件更改，要执行一次或多次 **delta** 函数调用来获取上一次增量查询后的增量更改集。若要获取演示一组增量查询调用的示例，请参阅[获取文件夹中邮件的增量更改](../../../concepts/delta_query_messages.md)。</span><span class="sxs-lookup"><span data-stu-id="1630e-p110">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](../../../concepts/delta_query_messages.md).</span></span>
 
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="1630e-165">响应</span><span class="sxs-lookup"><span data-stu-id="1630e-165">Response</span></span>
<span data-ttu-id="1630e-166">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="1630e-166">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="1630e-p111">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="1630e-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="1630e-169">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="1630e-169">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="1630e-p112">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1630e-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders('{id}')/messages/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "internetMessageId": "internetMessageId-value",
      "subject": "subject-value",
      "body": {
        "contentType": "contentType-value",
        "content": "content-value"
      }
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="1630e-172">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1630e-172">See also</span></span>

- [<span data-ttu-id="1630e-173">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="1630e-173">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="1630e-174">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="1630e-174">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->