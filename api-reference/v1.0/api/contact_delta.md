# <a name="contact-delta"></a><span data-ttu-id="714c3-101">contact: delta</span><span class="sxs-lookup"><span data-stu-id="714c3-101">contact: delta</span></span>

<span data-ttu-id="714c3-102">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="714c3-102">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="714c3-p101">对文件夹中的联系人的 **delta** 函数调用与 GET 请求相似，但是可通过在对其的一次或多次调用中正确应用[状态令牌](../../../concepts/delta_query_overview.md)来查询该文件夹中的联系人的增量更改这一点除外。通过此功能，你可以维护和同步本地存储的用户联系人，而无需每次都从服务器中获取整组联系人。</span><span class="sxs-lookup"><span data-stu-id="714c3-p101">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="714c3-105">权限</span><span class="sxs-lookup"><span data-stu-id="714c3-105">Permissions</span></span>
<span data-ttu-id="714c3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="714c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="714c3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="714c3-108">Permission type</span></span>      | <span data-ttu-id="714c3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="714c3-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="714c3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="714c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="714c3-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="714c3-111">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="714c3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="714c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="714c3-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="714c3-113">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="714c3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="714c3-114">Application</span></span> | <span data-ttu-id="714c3-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="714c3-115">Contacts.Read, Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="714c3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="714c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/<id>/contactFolders/{id}/contacts/delta
```

### <a name="query-parameters"></a><span data-ttu-id="714c3-117">查询参数</span><span class="sxs-lookup"><span data-stu-id="714c3-117">Query parameters</span></span>

<span data-ttu-id="714c3-p103">跟踪联系人更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="714c3-p103">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="714c3-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="714c3-123">Query parameter</span></span>      | <span data-ttu-id="714c3-124">类型</span><span class="sxs-lookup"><span data-stu-id="714c3-124">Type</span></span>   |<span data-ttu-id="714c3-125">说明</span><span class="sxs-lookup"><span data-stu-id="714c3-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="714c3-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="714c3-126">$deltatoken</span></span> | <span data-ttu-id="714c3-127">字符串</span><span class="sxs-lookup"><span data-stu-id="714c3-127">string</span></span> | <span data-ttu-id="714c3-p104">对同一个联系人集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="714c3-p104">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="714c3-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="714c3-130">$skiptoken</span></span> | <span data-ttu-id="714c3-131">string</span><span class="sxs-lookup"><span data-stu-id="714c3-131">string</span></span> | <span data-ttu-id="714c3-132">之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个联系人集合中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="714c3-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |


#### <a name="odata-query-parameters"></a><span data-ttu-id="714c3-133">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="714c3-133">OData query parameters</span></span>

- <span data-ttu-id="714c3-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="714c3-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="714c3-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="714c3-136">Request headers</span></span>
| <span data-ttu-id="714c3-137">名称</span><span class="sxs-lookup"><span data-stu-id="714c3-137">Name</span></span>       | <span data-ttu-id="714c3-138">类型</span><span class="sxs-lookup"><span data-stu-id="714c3-138">Type</span></span> | <span data-ttu-id="714c3-139">说明</span><span class="sxs-lookup"><span data-stu-id="714c3-139">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="714c3-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="714c3-140">Authorization</span></span>  | <span data-ttu-id="714c3-141">string</span><span class="sxs-lookup"><span data-stu-id="714c3-141">string</span></span>  | <span data-ttu-id="714c3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="714c3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="714c3-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="714c3-144">Content-Type</span></span>  | <span data-ttu-id="714c3-145">string</span><span class="sxs-lookup"><span data-stu-id="714c3-145">string</span></span>  | <span data-ttu-id="714c3-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="714c3-p107">application/json. Required.</span></span> |
| <span data-ttu-id="714c3-148">Prefer</span><span class="sxs-lookup"><span data-stu-id="714c3-148">Prefer</span></span> | <span data-ttu-id="714c3-149">string</span><span class="sxs-lookup"><span data-stu-id="714c3-149">string</span></span>  | <span data-ttu-id="714c3-p108">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="714c3-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="714c3-152">响应</span><span class="sxs-lookup"><span data-stu-id="714c3-152">Response</span></span>

<span data-ttu-id="714c3-153">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [contact](../resources/contact.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="714c3-153">If successful, this method returns a `200, OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="714c3-154">示例</span><span class="sxs-lookup"><span data-stu-id="714c3-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="714c3-155">请求</span><span class="sxs-lookup"><span data-stu-id="714c3-155">Request</span></span>
<span data-ttu-id="714c3-156">下面的示例演示了如何调用单个 **delta** 函数，使用 `$select` 参数仅获取每个联系人的 **displayName** 属性并将响应正文中的联系人的最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="714c3-156">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="714c3-157">若要跟踪文件夹中联系人的更改，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="714c3-157">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="714c3-p109">演示如何使用状态令牌跟踪邮件文件夹中的邮件更改的示例与其相似：[获取文件夹中邮件的增量更改](../../../concepts/delta_query_messages.md)。跟踪联系人和跟踪文件夹中的邮件之间的主要区别在于增量查询请求 URL 以及查询响应将返回 **mailFolder** 集合而非 **message** 集合。</span><span class="sxs-lookup"><span data-stu-id="714c3-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](../../../concepts/delta_query_messages.md). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts/delta?$select=displayName

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="714c3-160">响应</span><span class="sxs-lookup"><span data-stu-id="714c3-160">Response</span></span>
<span data-ttu-id="714c3-161">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="714c3-161">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="714c3-p110">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="714c3-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="714c3-164">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="714c3-164">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="714c3-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="714c3-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders('{id}')/contacts/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="714c3-167">另请参阅</span><span class="sxs-lookup"><span data-stu-id="714c3-167">See also</span></span>

- [<span data-ttu-id="714c3-168">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="714c3-168">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="714c3-169">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="714c3-169">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->