---
title: 列出人员
description: 检索一组 person 对象，这些对象按与 user 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。
author: dkershaw10
localization_priority: Priority
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 1acc5a963939381ad132defdc3942db9e7d7a920
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509036"
---
# <a name="list-people"></a><span data-ttu-id="39b45-103">列出人员</span><span class="sxs-lookup"><span data-stu-id="39b45-103">List people</span></span>

<span data-ttu-id="39b45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39b45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39b45-105">检索一组 [person](../resources/person.md) 对象，这些对象按与 [user](../resources/user.md) 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="39b45-105">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="39b45-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](/graph/people-example)一文。</span><span class="sxs-lookup"><span data-stu-id="39b45-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="39b45-108">权限</span><span class="sxs-lookup"><span data-stu-id="39b45-108">Permissions</span></span>

<span data-ttu-id="39b45-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39b45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39b45-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39b45-111">Permission type</span></span>      | <span data-ttu-id="39b45-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39b45-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39b45-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39b45-113">Delegated (work or school account)</span></span> | <span data-ttu-id="39b45-114">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="39b45-114">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="39b45-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39b45-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39b45-116">People.Read</span><span class="sxs-lookup"><span data-stu-id="39b45-116">People.Read</span></span>    |
|<span data-ttu-id="39b45-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39b45-117">Application</span></span> | <span data-ttu-id="39b45-118">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="39b45-118">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39b45-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39b45-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39b45-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39b45-120">Optional query parameters</span></span>

<span data-ttu-id="39b45-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)自定义响应，如[获取人员的相关信息](/graph/people-example)一文中的示例所示。</span><span class="sxs-lookup"><span data-stu-id="39b45-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="39b45-122">名称</span><span class="sxs-lookup"><span data-stu-id="39b45-122">Name</span></span>|<span data-ttu-id="39b45-123">值</span><span class="sxs-lookup"><span data-stu-id="39b45-123">Value</span></span>|<span data-ttu-id="39b45-124">说明</span><span class="sxs-lookup"><span data-stu-id="39b45-124">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="39b45-125">$filter</span><span class="sxs-lookup"><span data-stu-id="39b45-125">$filter</span></span>|<span data-ttu-id="39b45-126">string</span><span class="sxs-lookup"><span data-stu-id="39b45-126">string</span></span>|<span data-ttu-id="39b45-127">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="39b45-127">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="39b45-128">$orderby</span><span class="sxs-lookup"><span data-stu-id="39b45-128">$orderby</span></span>|<span data-ttu-id="39b45-129">string</span><span class="sxs-lookup"><span data-stu-id="39b45-129">string</span></span>|<span data-ttu-id="39b45-130">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="39b45-130">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="39b45-131">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="39b45-131">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="39b45-132">$search</span><span class="sxs-lookup"><span data-stu-id="39b45-132">$search</span></span>|<span data-ttu-id="39b45-133">string</span><span class="sxs-lookup"><span data-stu-id="39b45-133">string</span></span>|<span data-ttu-id="39b45-134">按姓名或别名搜索人员。</span><span class="sxs-lookup"><span data-stu-id="39b45-134">Search for people by name or alias.</span></span> <span data-ttu-id="39b45-135">支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="39b45-135">Supports Fuzzy matching.</span></span> <span data-ttu-id="39b45-136">参数仅适用于搜索已登录用户的相关人员，而不适用于搜索与其他用户相关的人员。</span><span class="sxs-lookup"><span data-stu-id="39b45-136">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="39b45-137">此外还支持 `topic` 关键字，以根据从与此人的电子邮件对话中提取的主题查找人员。</span><span class="sxs-lookup"><span data-stu-id="39b45-137">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="39b45-138">有关信息和示例，请参阅“[获取相关人员的信息](/graph/people-example#perform-a-fuzzy-search)”的“*执行模糊搜索*”部分。</span><span class="sxs-lookup"><span data-stu-id="39b45-138">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="39b45-139">$select</span><span class="sxs-lookup"><span data-stu-id="39b45-139">$select</span></span>|<span data-ttu-id="39b45-140">string</span><span class="sxs-lookup"><span data-stu-id="39b45-140">string</span></span>|<span data-ttu-id="39b45-p105">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="39b45-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="39b45-143">$skip</span><span class="sxs-lookup"><span data-stu-id="39b45-143">$skip</span></span>|<span data-ttu-id="39b45-144">int</span><span class="sxs-lookup"><span data-stu-id="39b45-144">int</span></span>|<span data-ttu-id="39b45-p106">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="39b45-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="39b45-147">$top</span><span class="sxs-lookup"><span data-stu-id="39b45-147">$top</span></span>|<span data-ttu-id="39b45-148">int</span><span class="sxs-lookup"><span data-stu-id="39b45-148">int</span></span>|<span data-ttu-id="39b45-149">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="39b45-149">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="39b45-150">请求标头</span><span class="sxs-lookup"><span data-stu-id="39b45-150">Request headers</span></span>

| <span data-ttu-id="39b45-151">名称</span><span class="sxs-lookup"><span data-stu-id="39b45-151">Name</span></span>      |<span data-ttu-id="39b45-152">说明</span><span class="sxs-lookup"><span data-stu-id="39b45-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39b45-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="39b45-153">Authorization</span></span>  | <span data-ttu-id="39b45-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39b45-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39b45-156">接受</span><span class="sxs-lookup"><span data-stu-id="39b45-156">Accept</span></span> | <span data-ttu-id="39b45-157">application/json</span><span class="sxs-lookup"><span data-stu-id="39b45-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="39b45-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="39b45-158">Request body</span></span>

<span data-ttu-id="39b45-159">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39b45-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39b45-160">响应</span><span class="sxs-lookup"><span data-stu-id="39b45-160">Response</span></span>

<span data-ttu-id="39b45-p108">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象集合。响应可以包含一个人员对象或一个人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="39b45-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="39b45-163">示例</span><span class="sxs-lookup"><span data-stu-id="39b45-163">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="39b45-164">请求</span><span class="sxs-lookup"><span data-stu-id="39b45-164">Request</span></span>

<span data-ttu-id="39b45-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="39b45-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="39b45-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="39b45-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/people
```
# <a name="c"></a>[<span data-ttu-id="39b45-167">C#</span><span class="sxs-lookup"><span data-stu-id="39b45-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39b45-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39b45-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39b45-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39b45-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39b45-170">Java</span><span class="sxs-lookup"><span data-stu-id="39b45-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39b45-171">响应</span><span class="sxs-lookup"><span data-stu-id="39b45-171">Response</span></span>

<span data-ttu-id="39b45-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="39b45-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="39b45-173">有关更多示例，请参阅[获取人员的相关信息](/graph/people-example)一文。</span><span class="sxs-lookup"><span data-stu-id="39b45-173">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

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
