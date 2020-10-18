---
title: List messages
description: 获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b4eac7cd0a00134e5b07fa404bc441b66a33f352
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582084"
---
# <a name="list-messages"></a><span data-ttu-id="5eaa4-103">列出邮件</span><span class="sxs-lookup"><span data-stu-id="5eaa4-103">List messages</span></span>

<span data-ttu-id="5eaa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eaa4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5eaa4-105">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-105">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="5eaa4-106">根据页面大小和邮箱数据，从邮箱中获取邮件可能会引发多个请求。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-106">Depending on the page size and mailbox data, getting messages from a mailbox can incur multiple requests.</span></span> <span data-ttu-id="5eaa4-107">默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-107">The default page size is 10 messages.</span></span> <span data-ttu-id="5eaa4-108">若要获取下一页的邮件，只需将 `@odata.nextLink` 中返回的整个 URL 应用于下一个 get-messages 请求。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-108">To get the next page of messages, simply apply the entire URL returned in `@odata.nextLink` to the next get-messages request.</span></span> <span data-ttu-id="5eaa4-109">此 URL 包括可能已在初始请求中指定的任何查询参数。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-109">This URL includes any query parameters you may have specified in the initial request.</span></span> 

<span data-ttu-id="5eaa4-110">不要尝试从 `@odata.nextLink` URL 中提取 `$skip` 值来操纵响应。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-110">Do not try to extract the `$skip` value from the `@odata.nextLink` URL to manipulate responses.</span></span> <span data-ttu-id="5eaa4-111">此 API 使用 `$skip` 值来保留其已在用户邮箱中遍历的所有项的计数，以返回 message-type 项的页面。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-111">This API uses the `$skip` value to keep count of all the items it has gone through in the user's mailbox to return a page of message-type items.</span></span> <span data-ttu-id="5eaa4-112">因此，甚至在初始响应中，`$skip` 值都会大于页面大小。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-112">It's therefore possible that even in the initial response, the `$skip` value is larger than the page size.</span></span> <span data-ttu-id="5eaa4-113">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-113">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="5eaa4-114">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-114">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="5eaa4-115">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="5eaa4-115">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="5eaa4-116">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="5eaa4-116">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5eaa4-117">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-117">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5eaa4-118">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-118">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

> <span data-ttu-id="5eaa4-119">**注意**：请注意[已知问题](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams)，即此操作在自己的响应中包含 Microsoft Teams 聊天消息。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-119">**Note** Be aware of the [known issue](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) that this operation includes Microsoft Teams chat messages in its response.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eaa4-120">权限</span><span class="sxs-lookup"><span data-stu-id="5eaa4-120">Permissions</span></span>
<span data-ttu-id="5eaa4-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eaa4-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="5eaa4-123">Permission type</span></span>      | <span data-ttu-id="5eaa4-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5eaa4-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eaa4-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5eaa4-125">Delegated (work or school account)</span></span> | <span data-ttu-id="5eaa4-126">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eaa4-126">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5eaa4-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5eaa4-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eaa4-128">Mail.ReadBasic、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eaa4-128">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5eaa4-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="5eaa4-129">Application</span></span> | <span data-ttu-id="5eaa4-130">Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eaa4-130">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eaa4-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5eaa4-131">HTTP request</span></span>

<span data-ttu-id="5eaa4-132">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="5eaa4-132">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="5eaa4-133">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="5eaa4-133">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5eaa4-134">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5eaa4-134">Optional query parameters</span></span>
<span data-ttu-id="5eaa4-135">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-135">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="using-filter-and-orderby-in-the-same-query"></a><span data-ttu-id="5eaa4-136">在同一查询中使用 filter 和 orderby</span><span class="sxs-lookup"><span data-stu-id="5eaa4-136">Using filter and orderby in the same query</span></span>
<span data-ttu-id="5eaa4-137">在同一查询中使用 `$filter` 和 `$orderby` 获取消息时，请确保按以下方式指定属性：</span><span class="sxs-lookup"><span data-stu-id="5eaa4-137">When using `$filter` and `$orderby` in the same query to get messages, make sure to specify properties in the following ways:</span></span>

1. <span data-ttu-id="5eaa4-138">`$orderby` 中显示的属性也必须在 `$filter` 中显示。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-138">Properties that appear in `$orderby` must also appear in `$filter`.</span></span> 
2. <span data-ttu-id="5eaa4-139">`$orderby` 中显示的属性与 `$filter` 中属性的顺序相同。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-139">Properties that appear in `$orderby` are in the same order as in `$filter`.</span></span>
3. <span data-ttu-id="5eaa4-140">`$orderby` 中存在的属性显示在 `$filter` 中不存在的任意属性之前。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-140">Properties that are present in `$orderby` appear in `$filter` before any properties that aren't.</span></span>

<span data-ttu-id="5eaa4-141">无法进行此项操作时会导致下列错误：</span><span class="sxs-lookup"><span data-stu-id="5eaa4-141">Failing to do this results in the following error:</span></span>

- <span data-ttu-id="5eaa4-142">错误代码：`InefficientFilter`</span><span class="sxs-lookup"><span data-stu-id="5eaa4-142">Error code: `InefficientFilter`</span></span>
- <span data-ttu-id="5eaa4-143">错误消息：`The restriction or sort order is too complex for this operation.`</span><span class="sxs-lookup"><span data-stu-id="5eaa4-143">Error message: `The restriction or sort order is too complex for this operation.`</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eaa4-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="5eaa4-144">Request headers</span></span>
| <span data-ttu-id="5eaa4-145">名称</span><span class="sxs-lookup"><span data-stu-id="5eaa4-145">Name</span></span>       | <span data-ttu-id="5eaa4-146">类型</span><span class="sxs-lookup"><span data-stu-id="5eaa4-146">Type</span></span> | <span data-ttu-id="5eaa4-147">说明</span><span class="sxs-lookup"><span data-stu-id="5eaa4-147">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5eaa4-148">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eaa4-148">Authorization</span></span>  | <span data-ttu-id="5eaa4-149">string</span><span class="sxs-lookup"><span data-stu-id="5eaa4-149">string</span></span>  | <span data-ttu-id="5eaa4-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5eaa4-152">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5eaa4-152">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5eaa4-153">string</span><span class="sxs-lookup"><span data-stu-id="5eaa4-153">string</span></span> | <span data-ttu-id="5eaa4-154">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-154">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="5eaa4-155">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-155">Values can be "text" or "html".</span></span> <span data-ttu-id="5eaa4-156">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-156">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="5eaa4-157">可选。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-157">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5eaa4-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="5eaa4-158">Request body</span></span>
<span data-ttu-id="5eaa4-159">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eaa4-160">响应</span><span class="sxs-lookup"><span data-stu-id="5eaa4-160">Response</span></span>

<span data-ttu-id="5eaa4-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Message](../resources/message.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-161">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eaa4-162">示例</span><span class="sxs-lookup"><span data-stu-id="5eaa4-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5eaa4-163">请求</span><span class="sxs-lookup"><span data-stu-id="5eaa4-163">Request</span></span>
<span data-ttu-id="5eaa4-164">此示例获取已登录用户的邮箱中的默认前 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-164">This example gets the default, top 10 messages in the signed-in user's mailbox.</span></span> <span data-ttu-id="5eaa4-165">它使用 `$select` 在响应中返回每封邮件的属性的子集。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-165">It uses `$select` to return a subset of the properties of each message in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="5eaa4-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eaa4-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=sender,subject
```
# <a name="c"></a>[<span data-ttu-id="5eaa4-167">C#</span><span class="sxs-lookup"><span data-stu-id="5eaa4-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5eaa4-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eaa4-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5eaa4-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eaa4-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5eaa4-170">Java</span><span class="sxs-lookup"><span data-stu-id="5eaa4-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5eaa4-171">响应</span><span class="sxs-lookup"><span data-stu-id="5eaa4-171">Response</span></span>
<span data-ttu-id="5eaa4-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-172">Here is an example of the response.</span></span> <span data-ttu-id="5eaa4-173">若要获取下一页邮件，请将 `@odata.nextLink` 中返回的 URL 应用 于后续 GET 请求。</span><span class="sxs-lookup"><span data-stu-id="5eaa4-173">To get the next page of messages, apply the URL returned in `@odata.nextLink` to a subsequent GET request.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$select=sender%2csubject&$skip=14",
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
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4Dft\"",
            "id": "AAMkAGUAAAq5UMVAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
            "@odata.etag": "W/\"DAAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAq4DfF\"",
            "id": "AAMkAGUAAAq5UMUAAA=",
            "subject": "Accepted: Review strategy for Q3",
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "/O=EXCHANGELABS/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=A17A02BCF30C4937A87B14273385667C-ADELEV"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.eventMessage",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->