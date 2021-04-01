---
title: 列出邮件
description: '获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。 '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 6ccbd844e9bb8ccae4e7dd607cc78c28eaef5dc0
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473687"
---
# <a name="list-messages"></a><span data-ttu-id="66013-103">列出邮件</span><span class="sxs-lookup"><span data-stu-id="66013-103">List messages</span></span>

<span data-ttu-id="66013-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66013-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66013-105">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="66013-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="66013-106">根据页面大小和邮箱数据，从邮箱中获取邮件可能会引发多个请求。</span><span class="sxs-lookup"><span data-stu-id="66013-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="66013-107">默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="66013-107">The default page size is 10 messages.</span></span> <span data-ttu-id="66013-108">使用 `$top` 以自定义页面大小（范围在 1 - 1000 之间）。</span><span class="sxs-lookup"><span data-stu-id="66013-108">Use `$top` to customize the page size, within the range of 1 and 1000.</span></span>

<span data-ttu-id="66013-109">若要改进操作响应时间，请使用 `$select` 指定所需的精确属性；请参阅下方 [示例 1](#example-1-list-all-messages)。</span><span class="sxs-lookup"><span data-stu-id="66013-109">To improve the operation response time, use `$select` to specify the exact properties you need; see [example 1](#example-1-list-all-messages) below.</span></span> <span data-ttu-id="66013-110">微调 `$select` 和 `$top` 的值，尤其在必须使用较大的页面大小时，因为返回带有数百条邮件（且每条邮件都有完整的响应有效负载） 的页面可能触发 [网关超时](/graph/errors#http-status-codes) (HTTP 504)。</span><span class="sxs-lookup"><span data-stu-id="66013-110">Fine-tune the values for `$select` and `$top`, especially when you must use a larger page size, as returning a page with hundreds of messages each with a full response payload may trigger the [gateway timeout](/graph/errors#http-status-codes) (HTTP 504).</span></span>

<span data-ttu-id="66013-111">若要获取下一页的邮件，只需将 `@odata.nextLink` 中返回的整个 URL 应用于下一个 get-messages 请求。</span><span class="sxs-lookup"><span data-stu-id="66013-111">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="66013-112">此 URL 包括可能已在初始请求中指定的任何查询参数。</span><span class="sxs-lookup"><span data-stu-id="66013-112">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="66013-113">不要尝试从 `@odata.nextLink` URL 中提取 `$skip` 值来操纵响应。</span><span class="sxs-lookup"><span data-stu-id="66013-113">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="66013-114">此 API 使用 `$skip` 值来保留其已在用户邮箱中遍历的所有项的计数，以返回 message-type 项的页面。</span><span class="sxs-lookup"><span data-stu-id="66013-114">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="66013-115">因此，甚至在初始响应中，`$skip` 值都会大于页面大小。</span><span class="sxs-lookup"><span data-stu-id="66013-115">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="66013-116">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="66013-116">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="66013-117">可以筛选邮件并仅获取包含已登录用户提及的邮件。 [](../resources/mention.md)</span><span class="sxs-lookup"><span data-stu-id="66013-117">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span> <span data-ttu-id="66013-118">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="66013-118">See an [example](#request-2) below.</span></span> <span data-ttu-id="66013-119">默认情况下， `GET /me/messages` 该操作不会返回 **mentions** 属性。</span><span class="sxs-lookup"><span data-stu-id="66013-119">By default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="66013-120">使用 `$expand` 查询参数 [查找邮件中每个提及的详细信息](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message)。</span><span class="sxs-lookup"><span data-stu-id="66013-120">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message).</span></span>

<span data-ttu-id="66013-121">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="66013-121">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="66013-122">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="66013-122">If the app has application permissions, or,</span></span>
* <span data-ttu-id="66013-123">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="66013-123">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="66013-124">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="66013-124">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="66013-125">**注意**：请注意 [已知问题](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams)，即此操作在自己的响应中包含 Microsoft Teams 聊天消息。</span><span class="sxs-lookup"><span data-stu-id="66013-125">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="66013-126">权限</span><span class="sxs-lookup"><span data-stu-id="66013-126">Permissions</span></span>
<span data-ttu-id="66013-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66013-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66013-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="66013-129">Permission type</span></span>      | <span data-ttu-id="66013-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66013-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66013-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66013-131">Delegated (work or school account)</span></span> | <span data-ttu-id="66013-132">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66013-132">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="66013-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66013-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66013-134">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66013-134">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="66013-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="66013-135">Application</span></span> | <span data-ttu-id="66013-136">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66013-136">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="66013-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66013-137">HTTP request</span></span>

<span data-ttu-id="66013-138">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="66013-138">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="66013-139">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="66013-139">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="66013-140">若要获取用户邮箱中包含用户提及的所有邮件： </span><span class="sxs-lookup"><span data-stu-id="66013-140">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66013-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="66013-141">Optional query parameters</span></span>
<span data-ttu-id="66013-142">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66013-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="66013-143">可以使用 `$filter` **mentionsPreview** 属性上的 query 参数获取提及已登录用户的邮件。</span><span class="sxs-lookup"><span data-stu-id="66013-143">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="66013-144">在同一查询中使用 filter 和 orderby</span><span class="sxs-lookup"><span data-stu-id="66013-144">Using filter and orderby in the same query</span></span>
<span data-ttu-id="66013-145">在同一查询中使用 `$filter` 和 `$orderby` 获取消息时，请确保按以下方式指定属性：</span><span class="sxs-lookup"><span data-stu-id="66013-145">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="66013-146">`$orderby` 中显示的属性也必须在 `$filter` 中显示。</span><span class="sxs-lookup"><span data-stu-id="66013-146">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="66013-147">`$orderby` 中显示的属性与 `$filter` 中属性的顺序相同。</span><span class="sxs-lookup"><span data-stu-id="66013-147">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="66013-148">`$orderby` 中存在的属性显示在 `$filter` 中不存在的任意属性之前。</span><span class="sxs-lookup"><span data-stu-id="66013-148">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="66013-149">无法进行此项操作时会导致下列错误：</span><span class="sxs-lookup"><span data-stu-id="66013-149">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="66013-150">错误代码：`InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="66013-150">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="66013-151">错误消息：`The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="66013-151">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="66013-152">请求标头</span><span class="sxs-lookup"><span data-stu-id="66013-152">Request headers</span></span>
| <span data-ttu-id="66013-153">名称</span><span class="sxs-lookup"><span data-stu-id="66013-153">Name</span></span>       | <span data-ttu-id="66013-154">类型</span><span class="sxs-lookup"><span data-stu-id="66013-154">Type</span></span> | <span data-ttu-id="66013-155">说明</span><span class="sxs-lookup"><span data-stu-id="66013-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66013-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="66013-156">Authorization</span></span>  | <span data-ttu-id="66013-157">string</span><span class="sxs-lookup"><span data-stu-id="66013-157">string</span></span>  | <span data-ttu-id="66013-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66013-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66013-160">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="66013-160">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="66013-161">string</span><span class="sxs-lookup"><span data-stu-id="66013-161">string</span></span> | <span data-ttu-id="66013-162">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="66013-162">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="66013-163">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="66013-163">Values can be "text" or "html".</span></span> <span data-ttu-id="66013-164">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="66013-164">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="66013-165">可选。</span><span class="sxs-lookup"><span data-stu-id="66013-165">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66013-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="66013-166">Request body</span></span>
<span data-ttu-id="66013-167">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66013-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66013-168">响应</span><span class="sxs-lookup"><span data-stu-id="66013-168">Response</span></span>

<span data-ttu-id="66013-169">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/message.md) 代码和 message 对象集合。</span><span class="sxs-lookup"><span data-stu-id="66013-169">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66013-170">示例</span><span class="sxs-lookup"><span data-stu-id="66013-170">Examples</span></span>
### <a name="example-1-list-all-messages"></a><span data-ttu-id="66013-171">示例 1：列出所有邮件</span><span class="sxs-lookup"><span data-stu-id="66013-171">Example 1: List all messages</span></span>
#### <a name="request"></a><span data-ttu-id="66013-172">请求</span><span class="sxs-lookup"><span data-stu-id="66013-172">Request</span></span>
<span data-ttu-id="66013-173">第一个示例获取登录用户邮箱中的默认前 10 个邮件。</span><span class="sxs-lookup"><span data-stu-id="66013-173">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="66013-174">它使用 `$select` 在响应中返回每封邮件的属性的子集。</span><span class="sxs-lookup"><span data-stu-id="66013-174">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="http"></a>[<span data-ttu-id="66013-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="66013-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="66013-176">C#</span><span class="sxs-lookup"><span data-stu-id="66013-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66013-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66013-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66013-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66013-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66013-179">Java</span><span class="sxs-lookup"><span data-stu-id="66013-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="66013-180">响应</span><span class="sxs-lookup"><span data-stu-id="66013-180">Response</span></span>
<span data-ttu-id="66013-181">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66013-181">Here is an example of the response.</span></span> <span data-ttu-id="66013-182">若要获取下一页邮件，请将 `@odata.nextLink` 中返回的 URL 应用 于后续 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="66013-182">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
  "value": [
    {
      "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAwR4Hg\"",
      "id": "AAMkAGUAAAwTW09AAA=",
      "subject": "You have late tasks!",
      "sender": {
        "emailAddress": {
          "name": "Microsoft Planner",
          "address": "noreply@Planner.Office365.com"
        }
      }
    }
  ]
}
```

### <a name="example-2-use-filter-to-get-all-messages-satisfying-a-specific-condition"></a><span data-ttu-id="66013-183">示例 2：$filter获取满足特定条件的所有邮件</span><span class="sxs-lookup"><span data-stu-id="66013-183">Example 2: Use $filter to get all messages satisfying a specific condition</span></span>
#### <a name="request"></a><span data-ttu-id="66013-184">请求</span><span class="sxs-lookup"><span data-stu-id="66013-184">Request</span></span>
<span data-ttu-id="66013-185">下一个示例将筛选已登录用户的邮箱中提及该用户的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="66013-185">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="66013-186">它还用于 `$select` 返回响应中每封邮件的一部分属性。</span><span class="sxs-lookup"><span data-stu-id="66013-186">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="66013-187">此示例还合并了查询参数字符串中空格字符的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="66013-187">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="http"></a>[<span data-ttu-id="66013-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="66013-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[<span data-ttu-id="66013-189">C#</span><span class="sxs-lookup"><span data-stu-id="66013-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66013-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66013-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66013-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66013-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66013-192">Java</span><span class="sxs-lookup"><span data-stu-id="66013-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="66013-193">响应</span><span class="sxs-lookup"><span data-stu-id="66013-193">Response</span></span>
<span data-ttu-id="66013-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66013-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

### <a name="example-3-use-prefer-header-to-get-the-message-body-and-uniquebody-is-text-format"></a><span data-ttu-id="66013-197">示例 3：使用 prefer 标头获取邮件正文，uniqueBody 为文本格式</span><span class="sxs-lookup"><span data-stu-id="66013-197">Example 3: Use prefer header to get the message body and uniqueBody is text format</span></span>
#### <a name="request"></a><span data-ttu-id="66013-198">请求</span><span class="sxs-lookup"><span data-stu-id="66013-198">Request</span></span>
<span data-ttu-id="66013-199">第三个示例演示如何使用标头获取文本格式的每封邮件的 body 和 `Prefer: outlook.body-content-type="text"` **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="66013-199">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="66013-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="66013-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="66013-201">C#</span><span class="sxs-lookup"><span data-stu-id="66013-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66013-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66013-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66013-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66013-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66013-204">Java</span><span class="sxs-lookup"><span data-stu-id="66013-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="66013-205">响应</span><span class="sxs-lookup"><span data-stu-id="66013-205">Response</span></span>
<span data-ttu-id="66013-206">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66013-206">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
  "value":[
    {
      "@odata.type":"#microsoft.graph.eventMessageRequest",
      "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
      "id":"AAMkAGIAAAoZCfIAAA=",
      "subject":"Orientation ",
      "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
      "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
      },
      "uniqueBody":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
