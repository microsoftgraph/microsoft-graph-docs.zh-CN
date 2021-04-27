---
title: 列出技能
description: 检索 skillProficiency 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 78f91c8e3ba8a60278c0188bb5990d2aadbd8fb1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037163"
---
# <a name="list-skills"></a><span data-ttu-id="06806-103">列出技能</span><span class="sxs-lookup"><span data-stu-id="06806-103">List skills</span></span>

<span data-ttu-id="06806-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06806-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06806-105">检索用户配置文件中的 [skillProficiency](../resources/skillproficiency.md) 对象 [列表](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="06806-105">Retrieve a list of [skillProficiency](../resources/skillproficiency.md) objects in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06806-106">权限</span><span class="sxs-lookup"><span data-stu-id="06806-106">Permissions</span></span>

<span data-ttu-id="06806-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06806-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06806-109">Permission type</span></span>                        | <span data-ttu-id="06806-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06806-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="06806-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06806-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06806-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06806-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="06806-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06806-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06806-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06806-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="06806-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06806-115">Application</span></span>                            | <span data-ttu-id="06806-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06806-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="06806-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06806-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills
GET /users/{id | userPrincipalName}/profile/skills
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06806-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="06806-118">Optional query parameters</span></span>

<span data-ttu-id="06806-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="06806-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="06806-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="06806-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="06806-121">名称</span><span class="sxs-lookup"><span data-stu-id="06806-121">Name</span></span>            |<span data-ttu-id="06806-122">值</span><span class="sxs-lookup"><span data-stu-id="06806-122">Value</span></span>    |<span data-ttu-id="06806-123">说明</span><span class="sxs-lookup"><span data-stu-id="06806-123">Description</span></span>                                                                                                                                                                      |
|:---------------|:--------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="06806-124">$filter</span><span class="sxs-lookup"><span data-stu-id="06806-124">$filter</span></span>         |<span data-ttu-id="06806-125">string</span><span class="sxs-lookup"><span data-stu-id="06806-125">string</span></span>   |<span data-ttu-id="06806-126">将响应限制到仅包含指定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="06806-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                                  |
|<span data-ttu-id="06806-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="06806-127">$orderby</span></span>        |<span data-ttu-id="06806-128">string</span><span class="sxs-lookup"><span data-stu-id="06806-128">string</span></span>   |<span data-ttu-id="06806-129">默认情况下，响应中的对象按查询中的 **createdDateTime** 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="06806-129">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="06806-130">可以使用 参数更改响应 `$orderby` 的顺序。</span><span class="sxs-lookup"><span data-stu-id="06806-130">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="06806-131">$select</span><span class="sxs-lookup"><span data-stu-id="06806-131">$select</span></span>         |<span data-ttu-id="06806-132">string</span><span class="sxs-lookup"><span data-stu-id="06806-132">string</span></span>   |<span data-ttu-id="06806-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="06806-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                             |
|<span data-ttu-id="06806-135">$skip</span><span class="sxs-lookup"><span data-stu-id="06806-135">$skip</span></span>           |<span data-ttu-id="06806-136">int</span><span class="sxs-lookup"><span data-stu-id="06806-136">int</span></span>      |<span data-ttu-id="06806-137">跳过前 n 个结果，可用于分页。</span><span class="sxs-lookup"><span data-stu-id="06806-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                     |
|<span data-ttu-id="06806-138">$top</span><span class="sxs-lookup"><span data-stu-id="06806-138">$top</span></span>            |<span data-ttu-id="06806-139">int</span><span class="sxs-lookup"><span data-stu-id="06806-139">int</span></span>      |<span data-ttu-id="06806-140">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="06806-140">Number of results to be returned.</span></span>                                                                                                                                                |

## <a name="request-headers"></a><span data-ttu-id="06806-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="06806-141">Request headers</span></span>

| <span data-ttu-id="06806-142">名称</span><span class="sxs-lookup"><span data-stu-id="06806-142">Name</span></span>           |<span data-ttu-id="06806-143">说明</span><span class="sxs-lookup"><span data-stu-id="06806-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="06806-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="06806-144">Authorization</span></span>  | <span data-ttu-id="06806-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06806-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="06806-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06806-147">Content-Type</span></span>   | <span data-ttu-id="06806-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="06806-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06806-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="06806-150">Request body</span></span>

<span data-ttu-id="06806-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06806-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06806-152">响应</span><span class="sxs-lookup"><span data-stu-id="06806-152">Response</span></span>

<span data-ttu-id="06806-153">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [skillProficiency](../resources/skillproficiency.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="06806-153">If successful, this method returns a `200 OK` response code and a collection of [skillProficiency](../resources/skillproficiency.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06806-154">示例</span><span class="sxs-lookup"><span data-stu-id="06806-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06806-155">请求</span><span class="sxs-lookup"><span data-stu-id="06806-155">Request</span></span>

<span data-ttu-id="06806-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="06806-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06806-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="06806-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_skills"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/skills
```
# <a name="c"></a>[<span data-ttu-id="06806-158">C#</span><span class="sxs-lookup"><span data-stu-id="06806-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-skills-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06806-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06806-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-skills-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06806-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06806-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-skills-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06806-161">Java</span><span class="sxs-lookup"><span data-stu-id="06806-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-skills-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06806-162">响应</span><span class="sxs-lookup"><span data-stu-id="06806-162">Response</span></span>

<span data-ttu-id="06806-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="06806-163">The following is an example of the response.</span></span>

> <span data-ttu-id="06806-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="06806-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "source": null,
      "categories": [
        "Professional"
      ],
      "displayName": "API Design",
      "proficiency": "advancedProfessional",
      "webUrl": null,
      "collaborationTags": [
        "ableToMentor"
      ]
    }
  ]
}
```


