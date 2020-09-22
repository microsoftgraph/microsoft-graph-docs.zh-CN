---
title: List messages
description: '获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。 '
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: outlook
ms.openlocfilehash: cb9dc81ea7a0f0e4607ac7844a0e1c52aae5f9e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031891"
---
# <a name="list-messages"></a><span data-ttu-id="4b0f3-103">列出邮件</span><span class="sxs-lookup"><span data-stu-id="4b0f3-103">List messages</span></span>

<span data-ttu-id="4b0f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b0f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b0f3-105">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="4b0f3-106">根据页面大小和邮箱数据，从邮箱中获取邮件可能会引发多个请求。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="4b0f3-107">默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-107">The default page size is 10 messages.</span></span> <span data-ttu-id="4b0f3-108">若要获取下一页的邮件，只需将 `@odata.nextLink` 中返回的整个 URL 应用于下一个 get-messages 请求。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-108">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="4b0f3-109">此 URL 包括可能已在初始请求中指定的任何查询参数。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-109">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="4b0f3-110">不要尝试从 `@odata.nextLink` URL 中提取 `$skip` 值来操纵响应。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-110">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="4b0f3-111">此 API 使用 `$skip` 值来保留其已在用户邮箱中遍历的所有项的计数，以返回 message-type 项的页面。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-111">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="4b0f3-112">因此，甚至在初始响应中，`$skip` 值都会大于页面大小。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-112">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="4b0f3-113">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-113">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="4b0f3-114">您可以对邮件进行筛选，并只获取那些包含已登录 [用户的说明](../resources/mention.md) 。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-114">You can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span> <span data-ttu-id="4b0f3-115">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-115">See an [example](#request-2) below.</span></span> <span data-ttu-id="4b0f3-116">默认情况下，该 `GET /me/messages` 操作不会返回 **提及** 属性。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-116">By default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="4b0f3-117">使用 `$expand` 查询参数 [在邮件中查找每个提及的详细信息](../api/message-get.md#example-2)。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-117">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#example-2).</span></span>

<span data-ttu-id="4b0f3-118">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="4b0f3-118">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="4b0f3-119">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="4b0f3-119">If the app has application permissions, or,</span></span>
* <span data-ttu-id="4b0f3-120">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-120">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="4b0f3-121">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-121">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="4b0f3-122">**注意**：请注意[已知问题](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams)，即此操作在自己的响应中包含 Microsoft Teams 聊天消息。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-122">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="4b0f3-123">权限</span><span class="sxs-lookup"><span data-stu-id="4b0f3-123">Permissions</span></span>
<span data-ttu-id="4b0f3-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0f3-126">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b0f3-126">Permission type</span></span>      | <span data-ttu-id="4b0f3-127">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b0f3-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b0f3-128">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b0f3-128">Delegated (work or school account)</span></span> | <span data-ttu-id="4b0f3-129">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b0f3-129">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4b0f3-130">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b0f3-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b0f3-131">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b0f3-131">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4b0f3-132">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b0f3-132">Application</span></span> | <span data-ttu-id="4b0f3-133">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b0f3-133">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b0f3-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b0f3-134">HTTP request</span></span>

<span data-ttu-id="4b0f3-135">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4b0f3-135">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="4b0f3-136">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4b0f3-136">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="4b0f3-137">若要获取用户邮箱中包含用户 **提及** 的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4b0f3-137">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b0f3-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b0f3-138">Optional query parameters</span></span>
<span data-ttu-id="4b0f3-139">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-139">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4b0f3-140">您可以使用 `$filter` **mentionsPreview** 属性上的查询参数来获取那些提及已登录用户的消息。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-140">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="4b0f3-141">在同一查询中使用 filter 和 orderby</span><span class="sxs-lookup"><span data-stu-id="4b0f3-141">Using filter and orderby in the same query</span></span>
<span data-ttu-id="4b0f3-142">在同一查询中使用 `$filter` 和 `$orderby` 获取消息时，请确保按以下方式指定属性：</span><span class="sxs-lookup"><span data-stu-id="4b0f3-142">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="4b0f3-143">`$orderby` 中显示的属性也必须在 `$filter` 中显示。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-143">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="4b0f3-144">`$orderby` 中显示的属性与 `$filter` 中属性的顺序相同。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-144">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="4b0f3-145">`$orderby` 中存在的属性显示在 `$filter` 中不存在的任意属性之前。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-145">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="4b0f3-146">无法进行此项操作时会导致下列错误：</span><span class="sxs-lookup"><span data-stu-id="4b0f3-146">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="4b0f3-147">错误代码：`InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="4b0f3-147">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="4b0f3-148">错误消息：`The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="4b0f3-148">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b0f3-149">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b0f3-149">Request headers</span></span>
| <span data-ttu-id="4b0f3-150">名称</span><span class="sxs-lookup"><span data-stu-id="4b0f3-150">Name</span></span>       | <span data-ttu-id="4b0f3-151">类型</span><span class="sxs-lookup"><span data-stu-id="4b0f3-151">Type</span></span> | <span data-ttu-id="4b0f3-152">说明</span><span class="sxs-lookup"><span data-stu-id="4b0f3-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4b0f3-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b0f3-153">Authorization</span></span>  | <span data-ttu-id="4b0f3-154">string</span><span class="sxs-lookup"><span data-stu-id="4b0f3-154">string</span></span>  | <span data-ttu-id="4b0f3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b0f3-157">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="4b0f3-157">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="4b0f3-158">string</span><span class="sxs-lookup"><span data-stu-id="4b0f3-158">string</span></span> | <span data-ttu-id="4b0f3-159">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-159">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="4b0f3-160">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-160">Values can be "text" or "html".</span></span> <span data-ttu-id="4b0f3-161">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-161">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="4b0f3-162">可选。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-162">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b0f3-163">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b0f3-163">Request body</span></span>
<span data-ttu-id="4b0f3-164">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b0f3-165">响应</span><span class="sxs-lookup"><span data-stu-id="4b0f3-165">Response</span></span>

<span data-ttu-id="4b0f3-166">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [message](../resources/message.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-166">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b0f3-167">示例</span><span class="sxs-lookup"><span data-stu-id="4b0f3-167">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="4b0f3-168">请求 1</span><span class="sxs-lookup"><span data-stu-id="4b0f3-168">Request 1</span></span>
<span data-ttu-id="4b0f3-169">第一个示例获取已登录用户的邮箱中的默认前10封邮件。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-169">The first example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="4b0f3-170">它使用 `$select` 在响应中返回每封邮件的属性的子集。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-170">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

# <a name="http"></a>[<span data-ttu-id="4b0f3-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0f3-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="4b0f3-172">C#</span><span class="sxs-lookup"><span data-stu-id="4b0f3-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b0f3-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b0f3-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b0f3-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b0f3-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="4b0f3-175">响应 1</span><span class="sxs-lookup"><span data-stu-id="4b0f3-175">Response 1</span></span>
<span data-ttu-id="4b0f3-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-176">Here is an example of the response.</span></span> <span data-ttu-id="4b0f3-177">若要获取下一页邮件，请将 `@odata.nextLink` 中返回的 URL 应用 于后续 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-177">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/messages?$select=sender%2csubject&$skip=14",
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
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D1e\"",
            "id": "AAMkAGUAAAq5QKlAAA=",
            "subject": "You have late tasks!",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Planner",
                    "address": "noreply@Planner.Office365.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4D0v\"",
            "id": "AAMkAGUAAAq5QKkAAA=",
            "subject": "Your Azure AD Identity Protection Weekly Digest",
            "sender": {
                "emailAddress": {
                    "name": "Microsoft Azure",
                    "address": "azure-noreply@microsoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DsN\"",
            "id": "AAMkAGUAAAq5QKjAAA=",
            "subject": "Use attached file",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq9\"",
            "id": "AAMkAGUAAAq5QKiAAA=",
            "subject": "Original invitation",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dq1\"",
            "id": "AAMkAGUAAAq5QKhAAA=",
            "subject": "Koala image",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dqp\"",
            "id": "AAMkAGUAAAq5QKgAAA=",
            "subject": "Sales invoice template",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessageRequest",
            "@odata.etag": "W/\"CwAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dfa\"",
            "id": "AAMkAGUAAAq5T8tAAA=",
            "subject": "Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            }
        }
    ]
}
```


##### <a name="request-2"></a><span data-ttu-id="4b0f3-178">请求 2</span><span class="sxs-lookup"><span data-stu-id="4b0f3-178">Request 2</span></span>
<span data-ttu-id="4b0f3-179">下一个示例将对登录用户邮箱中的所有邮件进行筛选，以查找那些提及该用户的邮件。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-179">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="4b0f3-180">它还用于 `$select` 在响应中返回每个邮件的属性子集。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-180">It also uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="4b0f3-181">该示例还合并了查询参数字符串中的空格字符的 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-181">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b0f3-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0f3-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[<span data-ttu-id="4b0f3-183">C#</span><span class="sxs-lookup"><span data-stu-id="4b0f3-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b0f3-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b0f3-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b0f3-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b0f3-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="4b0f3-186">响应 2</span><span class="sxs-lookup"><span data-stu-id="4b0f3-186">Response 2</span></span>
<span data-ttu-id="4b0f3-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="4b0f3-190">请求 3</span><span class="sxs-lookup"><span data-stu-id="4b0f3-190">Request 3</span></span>
<span data-ttu-id="4b0f3-191">第三个示例演示如何使用 `Prefer: outlook.body-content-type="text"` 标头以文本格式获取每个邮件的 **Body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-191">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b0f3-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b0f3-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="4b0f3-193">C#</span><span class="sxs-lookup"><span data-stu-id="4b0f3-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b0f3-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b0f3-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b0f3-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b0f3-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-3"></a><span data-ttu-id="4b0f3-196">响应 3</span><span class="sxs-lookup"><span data-stu-id="4b0f3-196">Response 3</span></span>
<span data-ttu-id="4b0f3-197">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4b0f3-197">Here is an example of the response.</span></span> 

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
Content-length: 2704

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
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
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


