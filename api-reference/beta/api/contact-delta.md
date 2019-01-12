---
title: 'contact: delta'
description: 获取指定文件夹中已添加、删除或更新的联系人集。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 500895404d92c1eb74b06bc80dd380b9f7c224e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916220"
---
# <a name="contact-delta"></a><span data-ttu-id="42c43-103">contact: delta</span><span class="sxs-lookup"><span data-stu-id="42c43-103">contact: delta</span></span>

> <span data-ttu-id="42c43-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42c43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42c43-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42c43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42c43-106">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="42c43-106">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>

<span data-ttu-id="42c43-p102">对文件夹中的联系人的 **delta** 函数调用与 GET 请求相似，但是可通过在对其的一次或多次调用中正确应用[状态令牌](/graph/delta-query-overview)来查询该文件夹中的联系人的增量更改这一点除外。通过此功能，你可以维护和同步本地存储的用户联系人，而无需每次都从服务器中获取整组联系人。</span><span class="sxs-lookup"><span data-stu-id="42c43-p102">A **delta** function call for contacts in a folder is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contacts in that folder. This allows you to maintain and synchronize a local store of a user's contacts without having to fetch the entire set of contacts from the server every time.</span></span>  

## <a name="permissions"></a><span data-ttu-id="42c43-109">权限</span><span class="sxs-lookup"><span data-stu-id="42c43-109">Permissions</span></span>
<span data-ttu-id="42c43-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42c43-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42c43-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="42c43-112">Permission type</span></span>      | <span data-ttu-id="42c43-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42c43-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42c43-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42c43-114">Delegated (work or school account)</span></span> | <span data-ttu-id="42c43-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42c43-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="42c43-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42c43-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42c43-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42c43-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="42c43-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="42c43-118">Application</span></span> | <span data-ttu-id="42c43-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42c43-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="42c43-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42c43-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/contacts/delta
GET /users/<id>/contactFolders/{id}/contacts/delta
```

## <a name="query-parameters"></a><span data-ttu-id="42c43-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="42c43-121">Query parameters</span></span>

<span data-ttu-id="42c43-p104">跟踪联系人更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="42c43-p104">Tracking changes in contacts incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="42c43-127">查询参数</span><span class="sxs-lookup"><span data-stu-id="42c43-127">Query parameter</span></span>      | <span data-ttu-id="42c43-128">类型</span><span class="sxs-lookup"><span data-stu-id="42c43-128">Type</span></span>   |<span data-ttu-id="42c43-129">说明</span><span class="sxs-lookup"><span data-stu-id="42c43-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42c43-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="42c43-130">$deltatoken</span></span> | <span data-ttu-id="42c43-131">字符串</span><span class="sxs-lookup"><span data-stu-id="42c43-131">string</span></span> | <span data-ttu-id="42c43-p105">对同一个联系人集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="42c43-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="42c43-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="42c43-134">$skiptoken</span></span> | <span data-ttu-id="42c43-135">string</span><span class="sxs-lookup"><span data-stu-id="42c43-135">string</span></span> | <span data-ttu-id="42c43-136">之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个联系人集合中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="42c43-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="42c43-137">OData 查询参数</span><span class="sxs-lookup"><span data-stu-id="42c43-137">OData query parameters</span></span>

- <span data-ttu-id="42c43-p106">像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 _id_ 属性。</span><span class="sxs-lookup"><span data-stu-id="42c43-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="42c43-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="42c43-140">Request headers</span></span>
| <span data-ttu-id="42c43-141">名称</span><span class="sxs-lookup"><span data-stu-id="42c43-141">Name</span></span>       | <span data-ttu-id="42c43-142">类型</span><span class="sxs-lookup"><span data-stu-id="42c43-142">Type</span></span> | <span data-ttu-id="42c43-143">说明</span><span class="sxs-lookup"><span data-stu-id="42c43-143">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="42c43-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="42c43-144">Authorization</span></span>  | <span data-ttu-id="42c43-145">string</span><span class="sxs-lookup"><span data-stu-id="42c43-145">string</span></span>  | <span data-ttu-id="42c43-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42c43-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42c43-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42c43-148">Content-Type</span></span>  | <span data-ttu-id="42c43-149">string</span><span class="sxs-lookup"><span data-stu-id="42c43-149">string</span></span>  | <span data-ttu-id="42c43-p108">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="42c43-p108">application/json. Required.</span></span> |
| <span data-ttu-id="42c43-152">Prefer</span><span class="sxs-lookup"><span data-stu-id="42c43-152">Prefer</span></span> | <span data-ttu-id="42c43-153">string</span><span class="sxs-lookup"><span data-stu-id="42c43-153">string</span></span>  | <span data-ttu-id="42c43-p109">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="42c43-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="42c43-156">响应</span><span class="sxs-lookup"><span data-stu-id="42c43-156">Response</span></span>

<span data-ttu-id="42c43-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [contact](../resources/contact.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="42c43-157">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42c43-158">示例</span><span class="sxs-lookup"><span data-stu-id="42c43-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42c43-159">请求</span><span class="sxs-lookup"><span data-stu-id="42c43-159">Request</span></span>
<span data-ttu-id="42c43-160">下面的示例演示了如何调用单个 **delta** 函数，使用 `$select` 参数仅获取每个联系人的 **displayName** 属性并将响应正文中的联系人的最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="42c43-160">The following example shows how to make a single **delta** function call, use the `$select` parameter to get only each contact's **displayName** property, and limit the maximum number of contacts in the response body to 2.</span></span>

<span data-ttu-id="42c43-161">若要跟踪文件夹中联系人的更改，要使用正确的状态令牌执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="42c43-161">To track changes in the contacts in a folder, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="42c43-p110">演示如何使用状态令牌跟踪邮件文件夹中的邮件更改的示例与其相似：[获取文件夹中邮件的增量更改](/graph/delta-query-messages)。跟踪联系人和跟踪文件夹中的邮件之间的主要区别在于增量查询请求 URL 以及查询响应将返回 **mailFolder** 集合而非 **message** 集合。</span><span class="sxs-lookup"><span data-stu-id="42c43-p110">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contacts and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contact** rather than **message** collections.</span></span>
 
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts/delta?$select=displayName

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="42c43-164">响应</span><span class="sxs-lookup"><span data-stu-id="42c43-164">Response</span></span>
<span data-ttu-id="42c43-165">如果请求成功，响应将包含一个状态令牌，其为 _skipToken_</span><span class="sxs-lookup"><span data-stu-id="42c43-165">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="42c43-p111">（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="42c43-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="42c43-168">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="42c43-168">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="42c43-p112">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42c43-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/contactfolders('{id}')/contacts/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="42c43-171">另请参阅</span><span class="sxs-lookup"><span data-stu-id="42c43-171">See also</span></span>

- [<span data-ttu-id="42c43-172">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="42c43-172">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="42c43-173">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="42c43-173">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
