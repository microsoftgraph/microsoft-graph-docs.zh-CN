---
title: 列出人员
description: 检索按其与用户，这由用户的通信和协作模式和业务关系的相关性排序的 person 对象的列表。
author: simonhult
ms.openlocfilehash: 64d24111f295fd076024a889d050c8c48c104295
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347654"
---
# <a name="list-people"></a><span data-ttu-id="4ec04-103">列出人员</span><span class="sxs-lookup"><span data-stu-id="4ec04-103">List people</span></span>

> <span data-ttu-id="4ec04-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ec04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ec04-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ec04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ec04-106">检索按给[用户](../resources/user.md)，它由用户的通信和协作模式和业务关系其相关性排序的[person](../resources/person.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4ec04-106">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ec04-107">权限</span><span class="sxs-lookup"><span data-stu-id="4ec04-107">Permissions</span></span>

<span data-ttu-id="4ec04-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ec04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec04-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ec04-110">Permission type</span></span>      | <span data-ttu-id="4ec04-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ec04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ec04-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ec04-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="4ec04-113">People.Read</span></span>    |
|<span data-ttu-id="4ec04-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ec04-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="4ec04-115">People.Read</span></span>    |
|<span data-ttu-id="4ec04-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ec04-116">Application</span></span> | <span data-ttu-id="4ec04-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ec04-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ec04-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ec04-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ec04-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ec04-119">Optional query parameters</span></span>

<span data-ttu-id="4ec04-120">此方法支持以下 OData 查询参数，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ec04-120">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="4ec04-121">Name</span><span class="sxs-lookup"><span data-stu-id="4ec04-121">Name</span></span>|<span data-ttu-id="4ec04-122">值</span><span class="sxs-lookup"><span data-stu-id="4ec04-122">Value</span></span>|<span data-ttu-id="4ec04-123">说明</span><span class="sxs-lookup"><span data-stu-id="4ec04-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="4ec04-124">$filter</span><span class="sxs-lookup"><span data-stu-id="4ec04-124">$filter</span></span>|<span data-ttu-id="4ec04-125">string</span><span class="sxs-lookup"><span data-stu-id="4ec04-125">string</span></span>|<span data-ttu-id="4ec04-126">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="4ec04-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="4ec04-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="4ec04-127">$orderby</span></span>|<span data-ttu-id="4ec04-128">string</span><span class="sxs-lookup"><span data-stu-id="4ec04-128">string</span></span>|<span data-ttu-id="4ec04-129">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="4ec04-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="4ec04-130">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="4ec04-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="4ec04-131">$search</span><span class="sxs-lookup"><span data-stu-id="4ec04-131">$search</span></span>|<span data-ttu-id="4ec04-132">string</span><span class="sxs-lookup"><span data-stu-id="4ec04-132">string</span></span>|<span data-ttu-id="4ec04-133">按姓名或别名搜索人员。</span><span class="sxs-lookup"><span data-stu-id="4ec04-133">Search for people by name or alias.</span></span> <span data-ttu-id="4ec04-134">支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="4ec04-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="4ec04-135">参数仅适用于不搜索已登录的用户相关人员搜索相关的其他用户的人员。</span><span class="sxs-lookup"><span data-stu-id="4ec04-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="4ec04-136">此外支持`topic`要查找人员关键字基于提取与此人的电子邮件对话的主题。</span><span class="sxs-lookup"><span data-stu-id="4ec04-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="4ec04-137">请参阅*Perform 模糊搜索*节[获取有关人员的相关信息](/graph/people-example#perform-a-fuzzy-search)的信息和示例。</span><span class="sxs-lookup"><span data-stu-id="4ec04-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="4ec04-138">$select</span><span class="sxs-lookup"><span data-stu-id="4ec04-138">$select</span></span>|<span data-ttu-id="4ec04-139">string</span><span class="sxs-lookup"><span data-stu-id="4ec04-139">string</span></span>|<span data-ttu-id="4ec04-p105">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="4ec04-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="4ec04-142">$skip</span><span class="sxs-lookup"><span data-stu-id="4ec04-142">$skip</span></span>|<span data-ttu-id="4ec04-143">整数</span><span class="sxs-lookup"><span data-stu-id="4ec04-143">int</span></span>|<span data-ttu-id="4ec04-p106">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="4ec04-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="4ec04-146">$top</span><span class="sxs-lookup"><span data-stu-id="4ec04-146">$top</span></span>|<span data-ttu-id="4ec04-147">整数</span><span class="sxs-lookup"><span data-stu-id="4ec04-147">int</span></span>|<span data-ttu-id="4ec04-148">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="4ec04-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4ec04-149">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ec04-149">Request headers</span></span>

| <span data-ttu-id="4ec04-150">Name</span><span class="sxs-lookup"><span data-stu-id="4ec04-150">Name</span></span>      |<span data-ttu-id="4ec04-151">说明</span><span class="sxs-lookup"><span data-stu-id="4ec04-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ec04-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ec04-152">Authorization</span></span>  | <span data-ttu-id="4ec04-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ec04-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ec04-155">Accept</span><span class="sxs-lookup"><span data-stu-id="4ec04-155">Accept</span></span> | <span data-ttu-id="4ec04-156">application/json</span><span class="sxs-lookup"><span data-stu-id="4ec04-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ec04-157">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ec04-157">Request body</span></span>

<span data-ttu-id="4ec04-158">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ec04-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ec04-159">响应</span><span class="sxs-lookup"><span data-stu-id="4ec04-159">Response</span></span>

<span data-ttu-id="4ec04-160">如果成功，此方法返回`200 OK`响应代码和响应正文中的[联系人](../resources/person.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4ec04-160">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ec04-161">示例</span><span class="sxs-lookup"><span data-stu-id="4ec04-161">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="4ec04-162">浏览</span><span class="sxs-lookup"><span data-stu-id="4ec04-162">Browse</span></span>

<span data-ttu-id="4ec04-163">本节中的请求获得人员已登录的用户与最相关 (`/me`)、 基于通信、 协作和业务关系。</span><span class="sxs-lookup"><span data-stu-id="4ec04-163">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="4ec04-164">默认情况下，每个响应都会返回10条记录，但您可以 改变这点 使用 *$顶部* 参数。</span><span class="sxs-lookup"><span data-stu-id="4ec04-164">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="4ec04-165">这些请求需要 People.Read 的权限。</span><span class="sxs-lookup"><span data-stu-id="4ec04-165">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4ec04-166">请求</span><span class="sxs-lookup"><span data-stu-id="4ec04-166">Request</span></span>

<span data-ttu-id="4ec04-167">下面是请求的默认的示例。</span><span class="sxs-lookup"><span data-stu-id="4ec04-167">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="4ec04-168">响应</span><span class="sxs-lookup"><span data-stu-id="4ec04-168">Response</span></span>

<span data-ttu-id="4ec04-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ec04-169">The following is an example of the response.</span></span>
><span data-ttu-id="4ec04-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4ec04-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="4ec04-172">请求人员的后续页面。</span><span class="sxs-lookup"><span data-stu-id="4ec04-172">Requesting a subsequent page of people</span></span>

<span data-ttu-id="4ec04-p110">如果第一个响应未包含相关人员的完整列表，可以使用 *$top* 和 *$skip* 发出第二个请求，以请求其他信息页面。如果上一个请求包含其他信息，则下一个请求从服务器获取下一个人员页面。</span><span class="sxs-lookup"><span data-stu-id="4ec04-p110">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="4ec04-175">对响应进行排序</span><span class="sxs-lookup"><span data-stu-id="4ec04-175">Sort the response</span></span>

<span data-ttu-id="4ec04-176">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="4ec04-176">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="4ec04-177">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="4ec04-177">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="4ec04-178">此查询选择与您最相关的人员，按他们的显示名称对他们进行排序，然后返回排序列表中的前10个人。</span><span class="sxs-lookup"><span data-stu-id="4ec04-178">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="4ec04-179">更改返回的人数和返回的字段</span><span class="sxs-lookup"><span data-stu-id="4ec04-179">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="4ec04-180">可以通过设置 *$top* 参数更改响应中返回的人员数。</span><span class="sxs-lookup"><span data-stu-id="4ec04-180">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="4ec04-181">下面的示例请求与最相关的 1,000 人员`/me`。</span><span class="sxs-lookup"><span data-stu-id="4ec04-181">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="4ec04-182">此外将请求限制后从服务器发送的请求只有的人员的显示名称的数据量。</span><span class="sxs-lookup"><span data-stu-id="4ec04-182">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="4ec04-183">选择要返回的字段</span><span class="sxs-lookup"><span data-stu-id="4ec04-183">Selecting the fields to return</span></span>

<span data-ttu-id="4ec04-184">您可以限制从服务器返回通过使用 *$select*参数选择一个或多个字段的数据量。</span><span class="sxs-lookup"><span data-stu-id="4ec04-184">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="4ec04-185">该 *@ odata.id* 字段总会返回。</span><span class="sxs-lookup"><span data-stu-id="4ec04-185">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="4ec04-186">下面的示例限制对*DisplayName*和*电子邮件地址*的 10 个最相关人员的响应。</span><span class="sxs-lookup"><span data-stu-id="4ec04-186">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="4ec04-187">使用过滤来限制响应</span><span class="sxs-lookup"><span data-stu-id="4ec04-187">Using a filter to limit the response</span></span>

<span data-ttu-id="4ec04-188">可以使用 *$filter* 参数将响应限制为记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="4ec04-188">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="4ec04-189">下面的查询限制的响应人员与源"目录"。</span><span class="sxs-lookup"><span data-stu-id="4ec04-189">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="4ec04-190">选择要筛选的响应中返回的字段</span><span class="sxs-lookup"><span data-stu-id="4ec04-190">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="4ec04-191">可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。</span><span class="sxs-lookup"><span data-stu-id="4ec04-191">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="4ec04-192">下面的示例获取的*DisplayName*和其显示名称等于指定的名称的人员的*电子邮件地址*。</span><span class="sxs-lookup"><span data-stu-id="4ec04-192">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="4ec04-193">在本示例中，只返回显示名称等于“Nestor Kellum”的人。</span><span class="sxs-lookup"><span data-stu-id="4ec04-193">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="4ec04-194">搜索人员</span><span class="sxs-lookup"><span data-stu-id="4ec04-194">Search people</span></span>

<span data-ttu-id="4ec04-195">本节中的请求也会获得人员最相关的已登录的用户 (`/me`)。</span><span class="sxs-lookup"><span data-stu-id="4ec04-195">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="4ec04-196">搜索请求需要 People.Read 的权限。</span><span class="sxs-lookup"><span data-stu-id="4ec04-196">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="4ec04-197">使用搜索来选择的人员</span><span class="sxs-lookup"><span data-stu-id="4ec04-197">Using search to select people</span></span>

<span data-ttu-id="4ec04-198">使用 *$search* 参数选择符合某组特定条件的人员。</span><span class="sxs-lookup"><span data-stu-id="4ec04-198">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="4ec04-199">下面的搜索查询返回与相关人员`/me`其 GivenName 或姓字母开头"j"。</span><span class="sxs-lookup"><span data-stu-id="4ec04-199">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="4ec04-200">使用搜索来指定相关主题</span><span class="sxs-lookup"><span data-stu-id="4ec04-200">Using search to specify a relevant topic</span></span>

<span data-ttu-id="4ec04-201">以下请求返回与相关人员`/me`名称中包含"ma"和谁具有关联"规划的功能。"</span><span class="sxs-lookup"><span data-stu-id="4ec04-201">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="4ec04-202">执行模糊搜索</span><span class="sxs-lookup"><span data-stu-id="4ec04-202">Performing a fuzzy search</span></span>

<span data-ttu-id="4ec04-203">以下请求执行名为"Hermaini 大厅。"的人员搜索</span><span class="sxs-lookup"><span data-stu-id="4ec04-203">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="4ec04-204">因为没有名为"Herminia 轮廓"与已登录的用户相关的人员，则返回"Herminia 轮廓"的信息。</span><span class="sxs-lookup"><span data-stu-id="4ec04-204">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="4ec04-205">相关的人员</span><span class="sxs-lookup"><span data-stu-id="4ec04-205">Related people</span></span>

<span data-ttu-id="4ec04-206">以下请求用户的组织中获取人员最相关的其他人。</span><span class="sxs-lookup"><span data-stu-id="4ec04-206">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="4ec04-207">该请求需要 User.ReadBasic.All People.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="4ec04-207">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="4ec04-208">本示例中，显示 Nestor Kellum 相关人员。</span><span class="sxs-lookup"><span data-stu-id="4ec04-208">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
