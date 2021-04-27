---
title: 'mailFolder: delta'
description: 获取用户邮箱中已添加、删除或移除的邮件文件夹集。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7bd7dc88530476efecad48c5ba81d8bfa531df4f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049287"
---
# <a name="mailfolder-delta"></a><span data-ttu-id="768c3-103">mailFolder: delta</span><span class="sxs-lookup"><span data-stu-id="768c3-103">mailFolder: delta</span></span>

<span data-ttu-id="768c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="768c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="768c3-105">获取用户邮箱中已添加、删除或移除的邮件文件夹集。</span><span class="sxs-lookup"><span data-stu-id="768c3-105">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="768c3-p101">对邮箱的邮件文件夹的 **delta** 函数调用与 GET 请求相似，除了前者可通过在对其的一次或多次调用中正确应用 [状态令牌](/graph/delta-query-overview)来查询邮件文件夹中的增量更改。通过此功能，你可以维护和同步本地存储的用户邮件文件夹，而无需每次都从服务器中获取该邮箱的所有邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="768c3-p101">A **delta** function call for mail folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the mail folders. This allows you to maintain and synchronize a local store of a user's mail folders without having to fetch all the mail folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="768c3-108">权限</span><span class="sxs-lookup"><span data-stu-id="768c3-108">Permissions</span></span>
<span data-ttu-id="768c3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="768c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="768c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="768c3-111">Permission type</span></span>      | <span data-ttu-id="768c3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="768c3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="768c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="768c3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="768c3-114">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="768c3-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="768c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="768c3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="768c3-116">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="768c3-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="768c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="768c3-117">Application</span></span> | <span data-ttu-id="768c3-118">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="768c3-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="768c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="768c3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/{id}/mailFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="768c3-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="768c3-120">Query parameters</span></span>

<span data-ttu-id="768c3-p103">跟踪邮件文件夹更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="768c3-p103">Tracking changes in mail folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="768c3-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="768c3-126">Query parameter</span></span>      | <span data-ttu-id="768c3-127">类型</span><span class="sxs-lookup"><span data-stu-id="768c3-127">Type</span></span>   |<span data-ttu-id="768c3-128">说明</span><span class="sxs-lookup"><span data-stu-id="768c3-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="768c3-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="768c3-129">$deltatoken</span></span> | <span data-ttu-id="768c3-130">string</span><span class="sxs-lookup"><span data-stu-id="768c3-130">string</span></span> | <span data-ttu-id="768c3-p104">对同一个邮件文件夹集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，其指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="768c3-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same mail folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="768c3-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="768c3-133">$skiptoken</span></span> | <span data-ttu-id="768c3-134">string</span><span class="sxs-lookup"><span data-stu-id="768c3-134">string</span></span> | <span data-ttu-id="768c3-135">对之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个邮件文件夹集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="768c3-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same mail folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="768c3-136">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="768c3-136">OData query parameters</span></span>

<span data-ttu-id="768c3-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="768c3-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="768c3-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="768c3-139">Request headers</span></span>
| <span data-ttu-id="768c3-140">名称</span><span class="sxs-lookup"><span data-stu-id="768c3-140">Name</span></span>       | <span data-ttu-id="768c3-141">类型</span><span class="sxs-lookup"><span data-stu-id="768c3-141">Type</span></span> | <span data-ttu-id="768c3-142">说明</span><span class="sxs-lookup"><span data-stu-id="768c3-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="768c3-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="768c3-143">Authorization</span></span>  | <span data-ttu-id="768c3-144">string</span><span class="sxs-lookup"><span data-stu-id="768c3-144">string</span></span>  | <span data-ttu-id="768c3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="768c3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="768c3-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="768c3-147">Content-Type</span></span>  | <span data-ttu-id="768c3-148">string</span><span class="sxs-lookup"><span data-stu-id="768c3-148">string</span></span>  | <span data-ttu-id="768c3-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="768c3-p107">application/json. Required.</span></span> |
| <span data-ttu-id="768c3-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="768c3-151">Prefer</span></span> | <span data-ttu-id="768c3-152">string</span><span class="sxs-lookup"><span data-stu-id="768c3-152">string</span></span>  | <span data-ttu-id="768c3-p108">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="768c3-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="768c3-155">响应</span><span class="sxs-lookup"><span data-stu-id="768c3-155">Response</span></span>

<span data-ttu-id="768c3-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [MailFolder](../resources/mailfolder.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="768c3-156">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="768c3-157">示例</span><span class="sxs-lookup"><span data-stu-id="768c3-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="768c3-158">请求</span><span class="sxs-lookup"><span data-stu-id="768c3-158">Request</span></span>
<span data-ttu-id="768c3-159">以下示例演示了如何执行单次 **delta** 函数调用，并将响应正文中的邮件文件夹最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="768c3-159">The following example shows how to make a single **delta** function call, and limit the maximum number of mail folders in the response body to 2.</span></span>

<span data-ttu-id="768c3-160">若要跟踪邮箱的邮件文件夹的更改，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上一次增量查询后的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="768c3-160">To track changes in the mail folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="768c3-p109">你可以找到一个类似的示例，演示如何使用状态令牌跟踪邮件文件夹中的邮件更改：[获取文件夹中邮件的增量更改](/graph/delta-query-messages)。跟踪邮件文件夹和跟踪文件夹中的邮件之间的主要区别在于，增量查询请求 URL 以及查询响应将返回 **mailFolder** 集合而非 **message** 集合。</span><span class="sxs-lookup"><span data-stu-id="768c3-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking mail folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **mailFolder** rather than **message** collections.</span></span>


# <a name="http"></a>[<span data-ttu-id="768c3-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="768c3-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="768c3-164">C#</span><span class="sxs-lookup"><span data-stu-id="768c3-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="768c3-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="768c3-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="768c3-166">Java</span><span class="sxs-lookup"><span data-stu-id="768c3-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="768c3-167">响应</span><span class="sxs-lookup"><span data-stu-id="768c3-167">Response</span></span>

<span data-ttu-id="768c3-168">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="768c3-168">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="768c3-p110">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="768c3-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="768c3-171">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="768c3-171">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="768c3-172">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="768c3-172">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="768c3-173">另请参阅</span><span class="sxs-lookup"><span data-stu-id="768c3-173">See also</span></span>

- [<span data-ttu-id="768c3-174">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="768c3-174">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="768c3-175">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="768c3-175">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


