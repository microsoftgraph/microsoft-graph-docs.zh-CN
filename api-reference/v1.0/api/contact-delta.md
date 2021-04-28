---
title: 'contact: delta'
description: 获取指定文件夹中已添加、删除或更新的联系人集。
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1956d285daebfd4a5d7916b33ade459d7869319a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051541"
---
# <a name="contact-delta"></a><span data-ttu-id="004ad-103">contact: delta</span><span class="sxs-lookup"><span data-stu-id="004ad-103">contact: delta</span></span>

<span data-ttu-id="004ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="004ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="004ad-105">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="004ad-105">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="004ad-p101">对文件夹中的联系人的 **delta** 函数调用与 GET 请求相似，但是可通过在对其的一次或多次调用中正确应用 [状态令牌](/graph/delta-query-overview)来查询该文件夹中的联系人的增量更改这一点除外。通过此功能，你可以维护和同步本地存储的用户联系人，而无需每次都从服务器中获取整组联系人。</span><span class="sxs-lookup"><span data-stu-id="004ad-p101">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="004ad-108">权限</span><span class="sxs-lookup"><span data-stu-id="004ad-108">Permissions</span></span>
<span data-ttu-id="004ad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="004ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="004ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="004ad-111">Permission type</span></span>      | <span data-ttu-id="004ad-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="004ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="004ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="004ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="004ad-114">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="004ad-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="004ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="004ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="004ad-116">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="004ad-116">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="004ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="004ad-117">Application</span></span> | <span data-ttu-id="004ad-118">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="004ad-118">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="004ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="004ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/{id}/contactFolders/{id}/contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="004ad-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="004ad-120">Query parameters</span></span>

<span data-ttu-id="004ad-p103">跟踪联系人更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="004ad-p103">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="004ad-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="004ad-126">Query parameter</span></span>      | <span data-ttu-id="004ad-127">类型</span><span class="sxs-lookup"><span data-stu-id="004ad-127">Type</span></span>   |<span data-ttu-id="004ad-128">说明</span><span class="sxs-lookup"><span data-stu-id="004ad-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="004ad-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="004ad-129">$deltatoken</span></span> | <span data-ttu-id="004ad-130">string</span><span class="sxs-lookup"><span data-stu-id="004ad-130">string</span></span> | <span data-ttu-id="004ad-p104">对同一个联系人集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="004ad-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="004ad-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="004ad-133">$skiptoken</span></span> | <span data-ttu-id="004ad-134">string</span><span class="sxs-lookup"><span data-stu-id="004ad-134">string</span></span> | <span data-ttu-id="004ad-135">之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个联系人集合中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="004ad-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="004ad-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="004ad-136">OData query parameters</span></span>

- <span data-ttu-id="004ad-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="004ad-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="004ad-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="004ad-139">Request headers</span></span>
| <span data-ttu-id="004ad-140">名称</span><span class="sxs-lookup"><span data-stu-id="004ad-140">Name</span></span>       | <span data-ttu-id="004ad-141">类型</span><span class="sxs-lookup"><span data-stu-id="004ad-141">Type</span></span> | <span data-ttu-id="004ad-142">说明</span><span class="sxs-lookup"><span data-stu-id="004ad-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="004ad-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="004ad-143">Authorization</span></span>  | <span data-ttu-id="004ad-144">string</span><span class="sxs-lookup"><span data-stu-id="004ad-144">string</span></span>  | <span data-ttu-id="004ad-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="004ad-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="004ad-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="004ad-147">Content-Type</span></span>  | <span data-ttu-id="004ad-148">string</span><span class="sxs-lookup"><span data-stu-id="004ad-148">string</span></span>  | <span data-ttu-id="004ad-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="004ad-p107">application/json. Required.</span></span> |
| <span data-ttu-id="004ad-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="004ad-151">Prefer</span></span> | <span data-ttu-id="004ad-152">string</span><span class="sxs-lookup"><span data-stu-id="004ad-152">string</span></span>  | <span data-ttu-id="004ad-p108">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="004ad-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="004ad-155">响应</span><span class="sxs-lookup"><span data-stu-id="004ad-155">Response</span></span>

<span data-ttu-id="004ad-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="004ad-156">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="004ad-157">示例</span><span class="sxs-lookup"><span data-stu-id="004ad-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="004ad-158">请求</span><span class="sxs-lookup"><span data-stu-id="004ad-158">Request</span></span>
<span data-ttu-id="004ad-159">下面的示例演示了如何调用单个 **delta** 函数，使用 `$select` 参数仅获取每个联系人的 **displayName** 属性并将响应正文中的联系人的最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="004ad-159">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="004ad-160">若要跟踪文件夹中联系人的更改，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="004ad-160">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="004ad-p109">演示如何使用状态令牌跟踪邮件文件夹中的邮件更改的示例与其相似：[获取文件夹中邮件的增量更改](/graph/delta-query-messages)。跟踪联系人和跟踪文件夹中的邮件之间的主要区别在于增量查询请求 URL 以及查询响应将返回 **mailFolder** 集合而非 **message** 集合。</span><span class="sxs-lookup"><span data-stu-id="004ad-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="004ad-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="004ad-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts/delta?$select=displayName
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="004ad-164">C#</span><span class="sxs-lookup"><span data-stu-id="004ad-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="004ad-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="004ad-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="004ad-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="004ad-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="004ad-167">Java</span><span class="sxs-lookup"><span data-stu-id="004ad-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="004ad-168">响应</span><span class="sxs-lookup"><span data-stu-id="004ad-168">Response</span></span>
<span data-ttu-id="004ad-169">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="004ad-169">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="004ad-p110">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="004ad-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="004ad-172">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="004ad-172">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="004ad-173">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="004ad-173">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/contactfolders/{id}/contacts/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="004ad-174">另请参阅</span><span class="sxs-lookup"><span data-stu-id="004ad-174">See also</span></span>

- [<span data-ttu-id="004ad-175">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="004ad-175">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="004ad-176">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="004ad-176">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

