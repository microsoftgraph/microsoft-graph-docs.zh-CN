---
title: 'message: delta'
description: 获取指定文件夹中已添加、删除或更新的邮件集。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7b093d809ceb4df70b191ce9f38fb7cf594b4675
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449762"
---
# <a name="message-delta"></a><span data-ttu-id="c7608-103">message: delta</span><span class="sxs-lookup"><span data-stu-id="c7608-103">message: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7608-104">获取指定文件夹中已添加、删除或更新的邮件集。</span><span class="sxs-lookup"><span data-stu-id="c7608-104">Get a set of messages that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="c7608-p101">对文件夹中的邮件的 **delta** 函数调用与 GET 请求相似，除了前者可通过在对其的一次或多次调用中正确应用[状态令牌](/graph/delta-query-overview)来[查询该文件夹中的邮件的增量更改](/graph/delta-query-messages)。通过此功能，你可以维护和同步本地存储的用户邮件，而无需每次都从服务器中获取整组邮件。</span><span class="sxs-lookup"><span data-stu-id="c7608-p101">A **delta** function call for messages in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can [query for incremental changes in the messages in that folder](/graph/delta-query-messages). This allows you to maintain and synchronize a local store of a user's messages without having to fetch the entire set of messages from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c7608-107">权限</span><span class="sxs-lookup"><span data-stu-id="c7608-107">Permissions</span></span>
<span data-ttu-id="c7608-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7608-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7608-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7608-110">Permission type</span></span>      | <span data-ttu-id="c7608-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7608-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7608-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7608-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7608-113">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="c7608-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c7608-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7608-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7608-115">User.readbasic.all、邮件、读取、封写</span><span class="sxs-lookup"><span data-stu-id="c7608-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c7608-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7608-116">Application</span></span> | <span data-ttu-id="c7608-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7608-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7608-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7608-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/<id>/mailFolders/{id}/messages/delta
```

## <a name="query-parameters"></a><span data-ttu-id="c7608-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="c7608-119">Query parameters</span></span>

<span data-ttu-id="c7608-p103">跟踪邮件更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="c7608-p103">Tracking changes in messages incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="c7608-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="c7608-125">Query parameter</span></span>      | <span data-ttu-id="c7608-126">类型</span><span class="sxs-lookup"><span data-stu-id="c7608-126">Type</span></span>   |<span data-ttu-id="c7608-127">说明</span><span class="sxs-lookup"><span data-stu-id="c7608-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7608-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="c7608-128">$deltatoken</span></span> | <span data-ttu-id="c7608-129">string</span><span class="sxs-lookup"><span data-stu-id="c7608-129">string</span></span> | <span data-ttu-id="c7608-p104">对同一个邮件集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="c7608-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same message collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="c7608-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c7608-132">$skiptoken</span></span> | <span data-ttu-id="c7608-133">string</span><span class="sxs-lookup"><span data-stu-id="c7608-133">string</span></span> | <span data-ttu-id="c7608-134">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个邮件集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="c7608-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same message collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="c7608-135">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="c7608-135">OData query parameters</span></span>

- <span data-ttu-id="c7608-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="c7608-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 
- <span data-ttu-id="c7608-138">对于邮件，Delta 查询支持 `$select`、`$top` 和 `$expand`。</span><span class="sxs-lookup"><span data-stu-id="c7608-138">Delta query support `$select`, `$top`, and `$expand` for messages.</span></span> 
- <span data-ttu-id="c7608-139">提供对 `$filter` 和 `$orderby` 的有限支持：</span><span class="sxs-lookup"><span data-stu-id="c7608-139">There is limited support for `$filter` and `$orderby`:</span></span>
  * <span data-ttu-id="c7608-140">唯一支持的 `$filter` 表达式是 `$filter=receivedDateTime+ge+{value}` 或 `$filter=receivedDateTime+gt+{value}`。</span><span class="sxs-lookup"><span data-stu-id="c7608-140">The only supported `$filter` expresssions are `$filter=receivedDateTime+ge+{value}` or `$filter=receivedDateTime+gt+{value}`.</span></span>
  * <span data-ttu-id="c7608-p106">唯一支持的 `$orderby` 表达式是 `$orderby=receivedDateTime+desc`。如果不包含 `$orderby` 表达式，则不能保证返回顺序。</span><span class="sxs-lookup"><span data-stu-id="c7608-p106">The only supported `$orderby` expression is `$orderby=receivedDateTime+desc`. If you do not include an `$orderby` expression, the return order is not guaranteed.</span></span> 
- <span data-ttu-id="c7608-143">不支持 `$search`。</span><span class="sxs-lookup"><span data-stu-id="c7608-143">There is no support for `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7608-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7608-144">Request headers</span></span>
| <span data-ttu-id="c7608-145">名称</span><span class="sxs-lookup"><span data-stu-id="c7608-145">Name</span></span>       | <span data-ttu-id="c7608-146">类型</span><span class="sxs-lookup"><span data-stu-id="c7608-146">Type</span></span> | <span data-ttu-id="c7608-147">说明</span><span class="sxs-lookup"><span data-stu-id="c7608-147">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c7608-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7608-148">Authorization</span></span>  | <span data-ttu-id="c7608-149">string</span><span class="sxs-lookup"><span data-stu-id="c7608-149">string</span></span>  | <span data-ttu-id="c7608-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7608-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7608-152">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7608-152">Content-Type</span></span>  | <span data-ttu-id="c7608-153">string</span><span class="sxs-lookup"><span data-stu-id="c7608-153">string</span></span>  | <span data-ttu-id="c7608-p108">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c7608-p108">application/json. Required.</span></span> |
| <span data-ttu-id="c7608-156">Prefer</span><span class="sxs-lookup"><span data-stu-id="c7608-156">Prefer</span></span> | <span data-ttu-id="c7608-157">string</span><span class="sxs-lookup"><span data-stu-id="c7608-157">string</span></span>  | <span data-ttu-id="c7608-p109">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="c7608-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c7608-160">响应</span><span class="sxs-lookup"><span data-stu-id="c7608-160">Response</span></span>

<span data-ttu-id="c7608-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c7608-161">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7608-162">示例</span><span class="sxs-lookup"><span data-stu-id="c7608-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7608-163">请求</span><span class="sxs-lookup"><span data-stu-id="c7608-163">Request</span></span>
<span data-ttu-id="c7608-164">以下示例演示了如何执行单次 **delta** 函数调用，并将响应正文中的邮件最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="c7608-164">The following example shows how to make a single **delta** function call, and limit the maximum number of messages in the response body to 2.</span></span>

<span data-ttu-id="c7608-p110">若要跟踪文件夹中的邮件更改，要执行一次或多次 **delta** 函数调用来获取上一次增量查询后的增量更改集。若要获取演示一组增量查询调用的示例，请参阅[获取文件夹中邮件的增量更改](/graph/delta-query-messages)。</span><span class="sxs-lookup"><span data-stu-id="c7608-p110">To track changes in the messages in a folder, you would make one or more **delta** function calls to get the set of incremental changes since the last delta query. For an example that shows a round of delta query calls, see [Get incremental changes to messages in a folder](/graph/delta-query-messages).</span></span>
 

# <a name="httptabhttp"></a>[<span data-ttu-id="c7608-167">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c7608-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/{id}/messages/delta

Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7608-168">C#</span><span class="sxs-lookup"><span data-stu-id="c7608-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7608-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7608-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c7608-170">响应</span><span class="sxs-lookup"><span data-stu-id="c7608-170">Response</span></span>
<span data-ttu-id="c7608-171">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="c7608-171">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="c7608-p111">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="c7608-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="c7608-174">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="c7608-174">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="c7608-p112">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7608-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders('{id}')/messages/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="c7608-177">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c7608-177">See also</span></span>

- [<span data-ttu-id="c7608-178">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="c7608-178">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="c7608-179">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="c7608-179">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
