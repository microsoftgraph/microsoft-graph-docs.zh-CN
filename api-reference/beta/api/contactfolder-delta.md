---
title: 'contactFolder: delta'
description: 获取用户邮箱中已添加、删除或移除的联系人文件夹集。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7dcaee0575c99aaea06b060f767ecaee87bf7151
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327232"
---
# <a name="contactfolder-delta"></a><span data-ttu-id="8987f-103">contactFolder: delta</span><span class="sxs-lookup"><span data-stu-id="8987f-103">contactFolder: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8987f-104">获取用户邮箱中已添加、删除或移除的联系人文件夹集。</span><span class="sxs-lookup"><span data-stu-id="8987f-104">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="8987f-p101">对邮箱的联系人文件夹的 **delta** 函数调用与 GET 请求相似，但是可通过在对其的一次或多次调用中正确应用[状态令牌](/graph/delta-query-overview)来查询联系人文件夹中的增量更改这一点除外。通过此功能，你可以维护和同步本地存储的用户联系人文件夹，而无需每次都从服务器中获取该邮箱的所有联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="8987f-p101">A **delta** function call for contact folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contact folders. This allows you to maintain and synchronize a local store of a user's contact folders without having to fetch all the contact folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="8987f-107">权限</span><span class="sxs-lookup"><span data-stu-id="8987f-107">Permissions</span></span>
<span data-ttu-id="8987f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8987f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8987f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8987f-110">Permission type</span></span>      | <span data-ttu-id="8987f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8987f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8987f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8987f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8987f-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8987f-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8987f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8987f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8987f-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8987f-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8987f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8987f-116">Application</span></span> | <span data-ttu-id="8987f-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8987f-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8987f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8987f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/<id>/contactFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="8987f-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="8987f-119">Query parameters</span></span>

<span data-ttu-id="8987f-p103">跟踪联系人文件夹更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分（`skiptoken` 或 `$deltatoken`）。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="8987f-p103">Tracking changes in contact folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion (`skiptoken` or `$deltatoken`) of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="8987f-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="8987f-125">Query parameter</span></span>      | <span data-ttu-id="8987f-126">类型</span><span class="sxs-lookup"><span data-stu-id="8987f-126">Type</span></span>   |<span data-ttu-id="8987f-127">说明</span><span class="sxs-lookup"><span data-stu-id="8987f-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8987f-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="8987f-128">$deltatoken</span></span> | <span data-ttu-id="8987f-129">string</span><span class="sxs-lookup"><span data-stu-id="8987f-129">string</span></span> | <span data-ttu-id="8987f-p104">对同一个联系人文件夹集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="8987f-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="8987f-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="8987f-132">$skiptoken</span></span> | <span data-ttu-id="8987f-133">string</span><span class="sxs-lookup"><span data-stu-id="8987f-133">string</span></span> | <span data-ttu-id="8987f-134">之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个联系人文件夹集合中有进一步的更改需要追踪。</span><span class="sxs-lookup"><span data-stu-id="8987f-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="8987f-135">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="8987f-135">OData query parameters</span></span>

<span data-ttu-id="8987f-p105">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="8987f-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="8987f-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="8987f-138">Request headers</span></span>
| <span data-ttu-id="8987f-139">名称</span><span class="sxs-lookup"><span data-stu-id="8987f-139">Name</span></span>       | <span data-ttu-id="8987f-140">类型</span><span class="sxs-lookup"><span data-stu-id="8987f-140">Type</span></span> | <span data-ttu-id="8987f-141">说明</span><span class="sxs-lookup"><span data-stu-id="8987f-141">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="8987f-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="8987f-142">Authorization</span></span>  | <span data-ttu-id="8987f-143">string</span><span class="sxs-lookup"><span data-stu-id="8987f-143">string</span></span>  | <span data-ttu-id="8987f-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8987f-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8987f-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8987f-146">Content-Type</span></span>  | <span data-ttu-id="8987f-147">字符串</span><span class="sxs-lookup"><span data-stu-id="8987f-147">string</span></span>  | <span data-ttu-id="8987f-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8987f-p107">application/json. Required.</span></span> |
| <span data-ttu-id="8987f-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="8987f-150">Prefer</span></span> | <span data-ttu-id="8987f-151">string</span><span class="sxs-lookup"><span data-stu-id="8987f-151">string</span></span>  | <span data-ttu-id="8987f-p108">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="8987f-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8987f-154">响应</span><span class="sxs-lookup"><span data-stu-id="8987f-154">Response</span></span>

<span data-ttu-id="8987f-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contactFolder](../resources/contactfolder.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="8987f-155">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8987f-156">示例</span><span class="sxs-lookup"><span data-stu-id="8987f-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8987f-157">请求</span><span class="sxs-lookup"><span data-stu-id="8987f-157">Request</span></span>
<span data-ttu-id="8987f-158">以下示例演示了如何执行单次 **delta** 函数调用，并将响应正文中的联系人文件夹最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="8987f-158">The following example shows how to make a single **delta** function call, and limit the maximum number of contact folders in the response body to 2.</span></span>

<span data-ttu-id="8987f-159">若要跟踪邮箱的联系人文件夹的更改，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="8987f-159">To track changes in the contact folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="8987f-p109">演示如何使用状态令牌跟踪邮件文件夹中的邮件更改的示例与其相似：[获取文件夹中邮件的增量更改](/graph/delta-query-messages)。跟踪联系人文件夹和跟踪文件夹中的邮件之间的主要区别在于增量查询请求 URL 以及查询响应将返回 **contactFolder** 集合而非 **message** 集合。</span><span class="sxs-lookup"><span data-stu-id="8987f-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contact folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contactFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="8987f-162">响应</span><span class="sxs-lookup"><span data-stu-id="8987f-162">Response</span></span>

<span data-ttu-id="8987f-163">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="8987f-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="8987f-p110">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="8987f-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="8987f-166">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="8987f-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="8987f-p111">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8987f-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/contactfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
     "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="8987f-169">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8987f-169">See also</span></span>

- [<span data-ttu-id="8987f-170">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="8987f-170">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="8987f-171">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="8987f-171">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
