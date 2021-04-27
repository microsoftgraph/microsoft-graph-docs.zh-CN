---
title: 列出人员
description: 检索 person 对象列表，这些对象按与 user 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。
author: dkershaw10
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8df99c32c43e947863c4a7713c984b99fbd4bb73
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053354"
---
# <a name="list-people"></a><span data-ttu-id="6bb38-103">列出人员</span><span class="sxs-lookup"><span data-stu-id="6bb38-103">List people</span></span>

<span data-ttu-id="6bb38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bb38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bb38-105">检索[人员对象列表](../resources/person.md)，这些对象按与用户的相关性排序，这[](../resources/user.md)由用户的通信和协作模式以及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="6bb38-105">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bb38-106">权限</span><span class="sxs-lookup"><span data-stu-id="6bb38-106">Permissions</span></span>

<span data-ttu-id="6bb38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6bb38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bb38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6bb38-109">Permission type</span></span>      | <span data-ttu-id="6bb38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6bb38-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bb38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6bb38-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6bb38-112">People.Read</span><span class="sxs-lookup"><span data-stu-id="6bb38-112">People.Read</span></span>    |
|<span data-ttu-id="6bb38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6bb38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bb38-114">People.Read</span><span class="sxs-lookup"><span data-stu-id="6bb38-114">People.Read</span></span>    |
|<span data-ttu-id="6bb38-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6bb38-115">Application</span></span> | <span data-ttu-id="6bb38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bb38-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bb38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bb38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6bb38-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6bb38-118">Optional query parameters</span></span>

<span data-ttu-id="6bb38-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6bb38-119">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="6bb38-120">名称</span><span class="sxs-lookup"><span data-stu-id="6bb38-120">Name</span></span>|<span data-ttu-id="6bb38-121">值</span><span class="sxs-lookup"><span data-stu-id="6bb38-121">Value</span></span>|<span data-ttu-id="6bb38-122">说明</span><span class="sxs-lookup"><span data-stu-id="6bb38-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="6bb38-123">$filter</span><span class="sxs-lookup"><span data-stu-id="6bb38-123">$filter</span></span>|<span data-ttu-id="6bb38-124">string</span><span class="sxs-lookup"><span data-stu-id="6bb38-124">string</span></span>|<span data-ttu-id="6bb38-125">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-125">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="6bb38-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="6bb38-126">$orderby</span></span>|<span data-ttu-id="6bb38-127">string</span><span class="sxs-lookup"><span data-stu-id="6bb38-127">string</span></span>|<span data-ttu-id="6bb38-128">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="6bb38-128">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="6bb38-129">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="6bb38-129">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="6bb38-130">$search</span><span class="sxs-lookup"><span data-stu-id="6bb38-130">$search</span></span>|<span data-ttu-id="6bb38-131">string</span><span class="sxs-lookup"><span data-stu-id="6bb38-131">string</span></span>|<span data-ttu-id="6bb38-132">按姓名或别名搜索人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-132">Search for people by name or alias.</span></span> <span data-ttu-id="6bb38-133">支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="6bb38-133">Supports Fuzzy matching.</span></span> <span data-ttu-id="6bb38-134">参数仅适用于搜索已登录用户的相关人员，而不适用于搜索与其他用户相关的人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-134">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="6bb38-135">此外还支持 `topic` 关键字，以根据从与此人的电子邮件对话中提取的主题查找人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-135">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="6bb38-136">有关信息和示例，请参阅“[获取相关人员的信息](/graph/people-example#perform-a-fuzzy-search)”的“*执行模糊搜索*”部分。</span><span class="sxs-lookup"><span data-stu-id="6bb38-136">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="6bb38-137">$select</span><span class="sxs-lookup"><span data-stu-id="6bb38-137">$select</span></span>|<span data-ttu-id="6bb38-138">string</span><span class="sxs-lookup"><span data-stu-id="6bb38-138">string</span></span>|<span data-ttu-id="6bb38-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="6bb38-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="6bb38-141">$skip</span><span class="sxs-lookup"><span data-stu-id="6bb38-141">$skip</span></span>|<span data-ttu-id="6bb38-142">int</span><span class="sxs-lookup"><span data-stu-id="6bb38-142">int</span></span>|<span data-ttu-id="6bb38-p105">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="6bb38-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="6bb38-145">$top</span><span class="sxs-lookup"><span data-stu-id="6bb38-145">$top</span></span>|<span data-ttu-id="6bb38-146">int</span><span class="sxs-lookup"><span data-stu-id="6bb38-146">int</span></span>|<span data-ttu-id="6bb38-147">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="6bb38-147">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6bb38-148">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bb38-148">Request headers</span></span>

| <span data-ttu-id="6bb38-149">名称</span><span class="sxs-lookup"><span data-stu-id="6bb38-149">Name</span></span>      |<span data-ttu-id="6bb38-150">说明</span><span class="sxs-lookup"><span data-stu-id="6bb38-150">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6bb38-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bb38-151">Authorization</span></span>  | <span data-ttu-id="6bb38-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6bb38-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6bb38-154">接受</span><span class="sxs-lookup"><span data-stu-id="6bb38-154">Accept</span></span> | <span data-ttu-id="6bb38-155">application/json</span><span class="sxs-lookup"><span data-stu-id="6bb38-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bb38-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bb38-156">Request body</span></span>

<span data-ttu-id="6bb38-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6bb38-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bb38-158">响应</span><span class="sxs-lookup"><span data-stu-id="6bb38-158">Response</span></span>

<span data-ttu-id="6bb38-159">如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和 [person](../resources/person.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6bb38-159">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6bb38-160">示例</span><span class="sxs-lookup"><span data-stu-id="6bb38-160">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="6bb38-161">浏览</span><span class="sxs-lookup"><span data-stu-id="6bb38-161">Browse</span></span>

<span data-ttu-id="6bb38-162">本节中的请求根据通信、协作和业务关系，获取与登录 () `/me` 相关最多的人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-162">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="6bb38-163">默认情况下，每个响应都会返回10条记录，但您可以 改变这点 使用 *$顶部* 参数。</span><span class="sxs-lookup"><span data-stu-id="6bb38-163">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="6bb38-164">这些请求需要 People.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="6bb38-164">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="6bb38-165">请求</span><span class="sxs-lookup"><span data-stu-id="6bb38-165">Request</span></span>

<span data-ttu-id="6bb38-166">以下是默认请求的一个示例。</span><span class="sxs-lookup"><span data-stu-id="6bb38-166">The following is an example of the default request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6bb38-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb38-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/people
```
# <a name="c"></a>[<span data-ttu-id="6bb38-168">C#</span><span class="sxs-lookup"><span data-stu-id="6bb38-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bb38-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bb38-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bb38-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bb38-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bb38-171">Java</span><span class="sxs-lookup"><span data-stu-id="6bb38-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6bb38-172">响应</span><span class="sxs-lookup"><span data-stu-id="6bb38-172">Response</span></span>

<span data-ttu-id="6bb38-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6bb38-173">The following is an example of the response.</span></span>
><span data-ttu-id="6bb38-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6bb38-174">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="6bb38-175">请求人员的后续页面。</span><span class="sxs-lookup"><span data-stu-id="6bb38-175">Requesting a subsequent page of people</span></span>

<span data-ttu-id="6bb38-p108">如果第一个响应未包含相关人员的完整列表，可以使用 *$top* 和 *$skip* 发出第二个请求，以请求其他信息页面。如果上一个请求包含其他信息，则下一个请求从服务器获取下一个人员页面。</span><span class="sxs-lookup"><span data-stu-id="6bb38-p108">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="6bb38-178">对响应进行排序</span><span class="sxs-lookup"><span data-stu-id="6bb38-178">Sort the response</span></span>

<span data-ttu-id="6bb38-179">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="6bb38-179">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="6bb38-180">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="6bb38-180">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="6bb38-181">此查询选择与您最相关的人员，按他们的显示名称对他们进行排序，然后返回排序列表中的前10个人。</span><span class="sxs-lookup"><span data-stu-id="6bb38-181">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="6bb38-182">更改返回的人数和返回的字段</span><span class="sxs-lookup"><span data-stu-id="6bb38-182">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="6bb38-183">可以通过设置 *$top* 参数更改响应中返回的人员数。</span><span class="sxs-lookup"><span data-stu-id="6bb38-183">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="6bb38-184">以下示例请求与 最相关的 1，000 个人 `/me` 。</span><span class="sxs-lookup"><span data-stu-id="6bb38-184">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="6bb38-185">请求还通过仅请求用户的请求来限制从服务器显示名称的数量。</span><span class="sxs-lookup"><span data-stu-id="6bb38-185">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="6bb38-186">选择要返回的字段</span><span class="sxs-lookup"><span data-stu-id="6bb38-186">Selecting the fields to return</span></span>

<span data-ttu-id="6bb38-187">可以使用 $select 参数选择一个或多个字段 *，* 以限制从服务器返回的数据量。</span><span class="sxs-lookup"><span data-stu-id="6bb38-187">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="6bb38-188">该 *@ odata.id* 字段总会返回。</span><span class="sxs-lookup"><span data-stu-id="6bb38-188">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="6bb38-189">以下示例将响应限制为 10 个最相关的人的 *DisplayName* 和 *EmailAddress。*</span><span class="sxs-lookup"><span data-stu-id="6bb38-189">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="6bb38-190">使用过滤来限制响应</span><span class="sxs-lookup"><span data-stu-id="6bb38-190">Using a filter to limit the response</span></span>

<span data-ttu-id="6bb38-191">可以使用 *$filter* 参数将响应限制为记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-191">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="6bb38-192">以下查询将响应限制为源为"Directory"的人。</span><span class="sxs-lookup"><span data-stu-id="6bb38-192">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="6bb38-193">选择要在筛选的响应中返回的字段</span><span class="sxs-lookup"><span data-stu-id="6bb38-193">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="6bb38-194">可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。</span><span class="sxs-lookup"><span data-stu-id="6bb38-194">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="6bb38-195">以下示例获取其名称等于指定名称显示名称的 *DisplayName* 和 *EmailAddress。*</span><span class="sxs-lookup"><span data-stu-id="6bb38-195">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="6bb38-196">在本示例中，只返回显示名称等于“Nestor Kellum”的人。</span><span class="sxs-lookup"><span data-stu-id="6bb38-196">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="6bb38-197">搜索人员</span><span class="sxs-lookup"><span data-stu-id="6bb38-197">Search people</span></span>

<span data-ttu-id="6bb38-198">本节中的请求还获取与登录用户相关 `/me` () 。</span><span class="sxs-lookup"><span data-stu-id="6bb38-198">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="6bb38-199">搜索请求需要 People.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="6bb38-199">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="6bb38-200">使用搜索选择人员</span><span class="sxs-lookup"><span data-stu-id="6bb38-200">Using search to select people</span></span>

<span data-ttu-id="6bb38-201">使用 *$search* 参数选择符合某组特定条件的人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-201">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="6bb38-202">下面的搜索查询返回与其 GivenName 或 Surname 以字母 `/me` "j"开头的人相关。</span><span class="sxs-lookup"><span data-stu-id="6bb38-202">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="6bb38-203">使用搜索来指定相关主题</span><span class="sxs-lookup"><span data-stu-id="6bb38-203">Using search to specify a relevant topic</span></span>

<span data-ttu-id="6bb38-204">以下请求返回与姓名包含"ma"且与"功能规划" `/me` 有关联的人。</span><span class="sxs-lookup"><span data-stu-id="6bb38-204">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="6bb38-205">执行模糊搜索</span><span class="sxs-lookup"><span data-stu-id="6bb38-205">Performing a fuzzy search</span></span>

<span data-ttu-id="6bb38-206">以下请求将搜索名为"Hermaini Hall"的人。</span><span class="sxs-lookup"><span data-stu-id="6bb38-206">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="6bb38-207">由于有一个名为"Herminia Hull"的人与登录用户相关，因此将返回"Herminia Hull"的信息。</span><span class="sxs-lookup"><span data-stu-id="6bb38-207">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="6bb38-208">相关人员</span><span class="sxs-lookup"><span data-stu-id="6bb38-208">Related people</span></span>

<span data-ttu-id="6bb38-209">以下请求获取与用户组织中其他人最相关的人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-209">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="6bb38-210">此请求需要具有 People.Read.All 权限的 User.ReadBasic.All。</span><span class="sxs-lookup"><span data-stu-id="6bb38-210">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="6bb38-211">本示例显示 Nestor Kellum 的的相关人员。</span><span class="sxs-lookup"><span data-stu-id="6bb38-211">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


