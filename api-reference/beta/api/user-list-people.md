---
title: 列出人员
description: 检索按其与用户的相关性排序的人员对象列表, 该列表由用户的通信和协作模式以及业务关系决定。
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: ed6c7a6c05cd678dc2107f00c42211a186fa61fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329892"
---
# <a name="list-people"></a><span data-ttu-id="ccc86-103">列出人员</span><span class="sxs-lookup"><span data-stu-id="ccc86-103">List people</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccc86-104">检索按其与[用户](../resources/user.md)的相关性排序的[人员](../resources/person.md)对象列表, 该列表由用户的通信和协作模式以及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="ccc86-104">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc86-105">权限</span><span class="sxs-lookup"><span data-stu-id="ccc86-105">Permissions</span></span>

<span data-ttu-id="ccc86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccc86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccc86-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccc86-108">Permission type</span></span>      | <span data-ttu-id="ccc86-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccc86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccc86-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ccc86-111">People.Read</span><span class="sxs-lookup"><span data-stu-id="ccc86-111">People.Read</span></span>    |
|<span data-ttu-id="ccc86-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccc86-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="ccc86-113">People.Read</span></span>    |
|<span data-ttu-id="ccc86-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccc86-114">Application</span></span> | <span data-ttu-id="ccc86-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc86-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccc86-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccc86-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccc86-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ccc86-117">Optional query parameters</span></span>

<span data-ttu-id="ccc86-118">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ccc86-118">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="ccc86-119">名称</span><span class="sxs-lookup"><span data-stu-id="ccc86-119">Name</span></span>|<span data-ttu-id="ccc86-120">值</span><span class="sxs-lookup"><span data-stu-id="ccc86-120">Value</span></span>|<span data-ttu-id="ccc86-121">说明</span><span class="sxs-lookup"><span data-stu-id="ccc86-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="ccc86-122">$filter</span><span class="sxs-lookup"><span data-stu-id="ccc86-122">$filter</span></span>|<span data-ttu-id="ccc86-123">string</span><span class="sxs-lookup"><span data-stu-id="ccc86-123">string</span></span>|<span data-ttu-id="ccc86-124">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="ccc86-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="ccc86-125">$orderby</span></span>|<span data-ttu-id="ccc86-126">string</span><span class="sxs-lookup"><span data-stu-id="ccc86-126">string</span></span>|<span data-ttu-id="ccc86-127">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="ccc86-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="ccc86-128">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="ccc86-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="ccc86-129">$search</span><span class="sxs-lookup"><span data-stu-id="ccc86-129">$search</span></span>|<span data-ttu-id="ccc86-130">string</span><span class="sxs-lookup"><span data-stu-id="ccc86-130">string</span></span>|<span data-ttu-id="ccc86-131">按姓名或别名搜索人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-131">Search for people by name or alias.</span></span> <span data-ttu-id="ccc86-132">支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="ccc86-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="ccc86-133">参数仅适用于搜索登录用户的相关人员, 而不是用于搜索与其他用户相关的人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="ccc86-134">还支持`topic`关键字, 以根据从与该人员的电子邮件对话中提取的主题查找人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="ccc86-135">有关信息和示例, 请参阅 "*执行模糊搜索*" 部分,[获取有关人员的相关信息](/graph/people-example#perform-a-fuzzy-search)和示例。</span><span class="sxs-lookup"><span data-stu-id="ccc86-135">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="ccc86-136">$select</span><span class="sxs-lookup"><span data-stu-id="ccc86-136">$select</span></span>|<span data-ttu-id="ccc86-137">string</span><span class="sxs-lookup"><span data-stu-id="ccc86-137">string</span></span>|<span data-ttu-id="ccc86-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="ccc86-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="ccc86-140">$skip</span><span class="sxs-lookup"><span data-stu-id="ccc86-140">$skip</span></span>|<span data-ttu-id="ccc86-141">int</span><span class="sxs-lookup"><span data-stu-id="ccc86-141">int</span></span>|<span data-ttu-id="ccc86-p105">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="ccc86-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="ccc86-144">$top</span><span class="sxs-lookup"><span data-stu-id="ccc86-144">$top</span></span>|<span data-ttu-id="ccc86-145">int</span><span class="sxs-lookup"><span data-stu-id="ccc86-145">int</span></span>|<span data-ttu-id="ccc86-146">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="ccc86-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ccc86-147">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccc86-147">Request headers</span></span>

| <span data-ttu-id="ccc86-148">名称</span><span class="sxs-lookup"><span data-stu-id="ccc86-148">Name</span></span>      |<span data-ttu-id="ccc86-149">说明</span><span class="sxs-lookup"><span data-stu-id="ccc86-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ccc86-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc86-150">Authorization</span></span>  | <span data-ttu-id="ccc86-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccc86-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccc86-153">接受</span><span class="sxs-lookup"><span data-stu-id="ccc86-153">Accept</span></span> | <span data-ttu-id="ccc86-154">application/json</span><span class="sxs-lookup"><span data-stu-id="ccc86-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccc86-155">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccc86-155">Request body</span></span>

<span data-ttu-id="ccc86-156">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccc86-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccc86-157">响应</span><span class="sxs-lookup"><span data-stu-id="ccc86-157">Response</span></span>

<span data-ttu-id="ccc86-158">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[person](../resources/person.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ccc86-158">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccc86-159">示例</span><span class="sxs-lookup"><span data-stu-id="ccc86-159">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="ccc86-160">定位</span><span class="sxs-lookup"><span data-stu-id="ccc86-160">Browse</span></span>

<span data-ttu-id="ccc86-161">本节中的请求将根据通信、协作和业务关系获取与登录用户最`/me`相关的人员 ()。</span><span class="sxs-lookup"><span data-stu-id="ccc86-161">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="ccc86-162">默认情况下，每个响应都会返回10条记录，但您可以 改变这点 使用 *$顶部* 参数。</span><span class="sxs-lookup"><span data-stu-id="ccc86-162">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="ccc86-163">这些请求需要人员读取权限。</span><span class="sxs-lookup"><span data-stu-id="ccc86-163">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="ccc86-164">请求</span><span class="sxs-lookup"><span data-stu-id="ccc86-164">Request</span></span>

<span data-ttu-id="ccc86-165">以下是默认请求的示例。</span><span class="sxs-lookup"><span data-stu-id="ccc86-165">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="ccc86-166">响应</span><span class="sxs-lookup"><span data-stu-id="ccc86-166">Response</span></span>

<span data-ttu-id="ccc86-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ccc86-167">The following is an example of the response.</span></span>
><span data-ttu-id="ccc86-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ccc86-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="ccc86-170">请求人员的后续页面。</span><span class="sxs-lookup"><span data-stu-id="ccc86-170">Requesting a subsequent page of people</span></span>

<span data-ttu-id="ccc86-p109">如果第一个响应未包含相关人员的完整列表，可以使用 *$top* 和 *$skip* 发出第二个请求，以请求其他信息页面。如果上一个请求包含其他信息，则下一个请求从服务器获取下一个人员页面。</span><span class="sxs-lookup"><span data-stu-id="ccc86-p109">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="ccc86-173">对响应进行排序</span><span class="sxs-lookup"><span data-stu-id="ccc86-173">Sort the response</span></span>

<span data-ttu-id="ccc86-174">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="ccc86-174">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="ccc86-175">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="ccc86-175">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="ccc86-176">此查询选择与您最相关的人员，按他们的显示名称对他们进行排序，然后返回排序列表中的前10个人。</span><span class="sxs-lookup"><span data-stu-id="ccc86-176">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="ccc86-177">更改返回的人数和返回的字段</span><span class="sxs-lookup"><span data-stu-id="ccc86-177">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="ccc86-178">可以通过设置 *$top* 参数更改响应中返回的人员数。</span><span class="sxs-lookup"><span data-stu-id="ccc86-178">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="ccc86-179">下面的示例请求与最相关的1000人`/me`。</span><span class="sxs-lookup"><span data-stu-id="ccc86-179">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="ccc86-180">请求还通过仅请求用户的显示名称来限制从服务器发送回的数据量。</span><span class="sxs-lookup"><span data-stu-id="ccc86-180">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="ccc86-181">选择要返回的字段</span><span class="sxs-lookup"><span data-stu-id="ccc86-181">Selecting the fields to return</span></span>

<span data-ttu-id="ccc86-182">您可以通过使用 *$select*参数选择一个或多个字段来限制从服务器返回的数据量。</span><span class="sxs-lookup"><span data-stu-id="ccc86-182">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="ccc86-183">该 *@ odata.id* 字段总会返回。</span><span class="sxs-lookup"><span data-stu-id="ccc86-183">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="ccc86-184">下面的示例将响应限制为10个最相关人员的*DisplayName*和*EmailAddress* 。</span><span class="sxs-lookup"><span data-stu-id="ccc86-184">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="ccc86-185">使用过滤来限制响应</span><span class="sxs-lookup"><span data-stu-id="ccc86-185">Using a filter to limit the response</span></span>

<span data-ttu-id="ccc86-186">可以使用 *$filter* 参数将响应限制为记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-186">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="ccc86-187">以下查询将响应限制为对源 "Directory" 的人员的响应。</span><span class="sxs-lookup"><span data-stu-id="ccc86-187">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="ccc86-188">在筛选的响应中选择要返回的字段</span><span class="sxs-lookup"><span data-stu-id="ccc86-188">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="ccc86-189">可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。</span><span class="sxs-lookup"><span data-stu-id="ccc86-189">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="ccc86-190">下面的示例获取其显示名称等于指定名称的用户的*DisplayName*和*EmailAddress* 。</span><span class="sxs-lookup"><span data-stu-id="ccc86-190">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="ccc86-191">在本示例中，只返回显示名称等于“Nestor Kellum”的人。</span><span class="sxs-lookup"><span data-stu-id="ccc86-191">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="ccc86-192">搜索人员</span><span class="sxs-lookup"><span data-stu-id="ccc86-192">Search people</span></span>

<span data-ttu-id="ccc86-193">此部分中的请求还可以获取与登录用户最相关的人员 (`/me`)。</span><span class="sxs-lookup"><span data-stu-id="ccc86-193">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="ccc86-194">搜索请求需要人员读取权限。</span><span class="sxs-lookup"><span data-stu-id="ccc86-194">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="ccc86-195">使用 "搜索" 选择人员</span><span class="sxs-lookup"><span data-stu-id="ccc86-195">Using search to select people</span></span>

<span data-ttu-id="ccc86-196">使用 *$search* 参数选择符合某组特定条件的人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-196">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="ccc86-197">下面的搜索查询返回与`/me`其 GivenName 或姓以字母 "j" 开头的人员相关的人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-197">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="ccc86-198">使用搜索来指定相关主题</span><span class="sxs-lookup"><span data-stu-id="ccc86-198">Using search to specify a relevant topic</span></span>

<span data-ttu-id="ccc86-199">以下请求返回相关人员, `/me`其名称包含 "ma", 以及与 "功能计划" 有关联的人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-199">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="ccc86-200">执行模糊搜索</span><span class="sxs-lookup"><span data-stu-id="ccc86-200">Performing a fuzzy search</span></span>

<span data-ttu-id="ccc86-201">下面的请求搜索名为 "Hermaini 厅" 的人。</span><span class="sxs-lookup"><span data-stu-id="ccc86-201">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="ccc86-202">由于存在与登录用户相关的名为 "所以凸" 的人员, 因此返回 "所以凸" 的信息。</span><span class="sxs-lookup"><span data-stu-id="ccc86-202">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="ccc86-203">相关人员</span><span class="sxs-lookup"><span data-stu-id="ccc86-203">Related people</span></span>

<span data-ttu-id="ccc86-204">以下请求获取与用户组织中的其他人最相关的人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-204">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="ccc86-205">此请求需要 user.readbasic.all 的所有人。读取。 all 权限。</span><span class="sxs-lookup"><span data-stu-id="ccc86-205">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="ccc86-206">在此示例中, 将显示 Nestor Kellum 的相关人员。</span><span class="sxs-lookup"><span data-stu-id="ccc86-206">In this example, Nestor Kellum's relevant people are displayed.</span></span>

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
  "suppressions": []
}
-->
