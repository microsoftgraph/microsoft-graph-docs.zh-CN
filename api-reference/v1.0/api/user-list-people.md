---
title: 列出人员
description: 检索一组 person 对象，这些对象按与 user 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。
author: dkershaw10
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 9ae83dbea4176ca818f9539f3676ff1febade3cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460201"
---
# <a name="list-people"></a><span data-ttu-id="e158c-103">列出人员</span><span class="sxs-lookup"><span data-stu-id="e158c-103">List people</span></span>

<span data-ttu-id="e158c-104">检索一组 [person](../resources/person.md) 对象，这些对象按与 [user](../resources/user.md) 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="e158c-104">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="e158c-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](/graph/people-example)一文。</span><span class="sxs-lookup"><span data-stu-id="e158c-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="e158c-107">权限</span><span class="sxs-lookup"><span data-stu-id="e158c-107">Permissions</span></span>

<span data-ttu-id="e158c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e158c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e158c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e158c-110">Permission type</span></span>      | <span data-ttu-id="e158c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e158c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e158c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e158c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e158c-113">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="e158c-113">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="e158c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e158c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e158c-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="e158c-115">People.Read</span></span>    |
|<span data-ttu-id="e158c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e158c-116">Application</span></span> | <span data-ttu-id="e158c-117">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="e158c-117">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e158c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e158c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e158c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e158c-119">Optional query parameters</span></span>

<span data-ttu-id="e158c-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)自定义响应，如[获取人员的相关信息](/graph/people-example)一文中的示例所示。</span><span class="sxs-lookup"><span data-stu-id="e158c-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="e158c-121">名称</span><span class="sxs-lookup"><span data-stu-id="e158c-121">Name</span></span>|<span data-ttu-id="e158c-122">值</span><span class="sxs-lookup"><span data-stu-id="e158c-122">Value</span></span>|<span data-ttu-id="e158c-123">说明</span><span class="sxs-lookup"><span data-stu-id="e158c-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="e158c-124">$filter</span><span class="sxs-lookup"><span data-stu-id="e158c-124">$filter</span></span>|<span data-ttu-id="e158c-125">string</span><span class="sxs-lookup"><span data-stu-id="e158c-125">string</span></span>|<span data-ttu-id="e158c-126">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="e158c-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="e158c-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="e158c-127">$orderby</span></span>|<span data-ttu-id="e158c-128">string</span><span class="sxs-lookup"><span data-stu-id="e158c-128">string</span></span>|<span data-ttu-id="e158c-129">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="e158c-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="e158c-130">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="e158c-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="e158c-131">$search</span><span class="sxs-lookup"><span data-stu-id="e158c-131">$search</span></span>|<span data-ttu-id="e158c-132">string</span><span class="sxs-lookup"><span data-stu-id="e158c-132">string</span></span>|<span data-ttu-id="e158c-133">按姓名或别名搜索人员。</span><span class="sxs-lookup"><span data-stu-id="e158c-133">Search for people by name or alias.</span></span> <span data-ttu-id="e158c-134">支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="e158c-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="e158c-135">参数仅适用于搜索已登录用户的相关人员，而不适用于搜索与其他用户相关的人员。</span><span class="sxs-lookup"><span data-stu-id="e158c-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="e158c-136">此外还支持 `topic` 关键字，以根据从与此人的电子邮件对话中提取的主题查找人员。</span><span class="sxs-lookup"><span data-stu-id="e158c-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="e158c-137">有关信息和示例，请参阅“[获取相关人员的信息](/graph/people-example#perform-a-fuzzy-search)”的“*执行模糊搜索*”部分。</span><span class="sxs-lookup"><span data-stu-id="e158c-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="e158c-138">$select</span><span class="sxs-lookup"><span data-stu-id="e158c-138">$select</span></span>|<span data-ttu-id="e158c-139">string</span><span class="sxs-lookup"><span data-stu-id="e158c-139">string</span></span>|<span data-ttu-id="e158c-p105">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="e158c-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="e158c-142">$skip</span><span class="sxs-lookup"><span data-stu-id="e158c-142">$skip</span></span>|<span data-ttu-id="e158c-143">int</span><span class="sxs-lookup"><span data-stu-id="e158c-143">int</span></span>|<span data-ttu-id="e158c-p106">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="e158c-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="e158c-146">$top</span><span class="sxs-lookup"><span data-stu-id="e158c-146">$top</span></span>|<span data-ttu-id="e158c-147">int</span><span class="sxs-lookup"><span data-stu-id="e158c-147">int</span></span>|<span data-ttu-id="e158c-148">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="e158c-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e158c-149">请求标头</span><span class="sxs-lookup"><span data-stu-id="e158c-149">Request headers</span></span>

| <span data-ttu-id="e158c-150">名称</span><span class="sxs-lookup"><span data-stu-id="e158c-150">Name</span></span>      |<span data-ttu-id="e158c-151">说明</span><span class="sxs-lookup"><span data-stu-id="e158c-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e158c-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="e158c-152">Authorization</span></span>  | <span data-ttu-id="e158c-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e158c-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e158c-155">接受</span><span class="sxs-lookup"><span data-stu-id="e158c-155">Accept</span></span> | <span data-ttu-id="e158c-156">application/json</span><span class="sxs-lookup"><span data-stu-id="e158c-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e158c-157">请求正文</span><span class="sxs-lookup"><span data-stu-id="e158c-157">Request body</span></span>

<span data-ttu-id="e158c-158">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e158c-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e158c-159">响应</span><span class="sxs-lookup"><span data-stu-id="e158c-159">Response</span></span>

<span data-ttu-id="e158c-p108">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象集合。响应可以包含一个人员对象或一个人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="e158c-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="e158c-162">示例</span><span class="sxs-lookup"><span data-stu-id="e158c-162">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="e158c-163">请求</span><span class="sxs-lookup"><span data-stu-id="e158c-163">Request</span></span>

<span data-ttu-id="e158c-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e158c-164">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e158c-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="e158c-165">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e158c-166">C#</span><span class="sxs-lookup"><span data-stu-id="e158c-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e158c-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="e158c-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e158c-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e158c-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e158c-169">响应</span><span class="sxs-lookup"><span data-stu-id="e158c-169">Response</span></span>

<span data-ttu-id="e158c-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e158c-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1370

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
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```

<span data-ttu-id="e158c-171">有关更多示例，请参阅[获取人员的相关信息](/graph/people-example)一文。</span><span class="sxs-lookup"><span data-stu-id="e158c-171">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
