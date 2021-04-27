---
title: 列出 educationalActivities
description: 检索 educationalActivity 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ab8a9800bd6c8517fd4d3fc84b1485549c4ed4ba
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037275"
---
# <a name="list-educationalactivities"></a><span data-ttu-id="4dcf1-103">列出 educationalActivities</span><span class="sxs-lookup"><span data-stu-id="4dcf1-103">List educationalActivities</span></span>

<span data-ttu-id="4dcf1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dcf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dcf1-105">从用户配置文件中检索 [educationalActivity](../resources/educationalactivity.md) 对象 [的列表](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-105">Retrieve a list of [educationalActivity](../resources/educationalactivity.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4dcf1-106">权限</span><span class="sxs-lookup"><span data-stu-id="4dcf1-106">Permissions</span></span>

<span data-ttu-id="4dcf1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4dcf1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dcf1-109">Permission type</span></span>                        | <span data-ttu-id="4dcf1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4dcf1-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="4dcf1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dcf1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4dcf1-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dcf1-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4dcf1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dcf1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dcf1-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dcf1-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4dcf1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dcf1-115">Application</span></span>                            | <span data-ttu-id="4dcf1-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dcf1-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="4dcf1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dcf1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities
GET /users/{id | userPrincipalName}/profile/educationalActivities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4dcf1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4dcf1-118">Optional query parameters</span></span>

<span data-ttu-id="4dcf1-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="4dcf1-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="4dcf1-121">名称</span><span class="sxs-lookup"><span data-stu-id="4dcf1-121">Name</span></span>            |<span data-ttu-id="4dcf1-122">值</span><span class="sxs-lookup"><span data-stu-id="4dcf1-122">Value</span></span>    |<span data-ttu-id="4dcf1-123">说明</span><span class="sxs-lookup"><span data-stu-id="4dcf1-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4dcf1-124">$filter</span><span class="sxs-lookup"><span data-stu-id="4dcf1-124">$filter</span></span>         |<span data-ttu-id="4dcf1-125">string</span><span class="sxs-lookup"><span data-stu-id="4dcf1-125">string</span></span>   |<span data-ttu-id="4dcf1-126">将响应限制到仅包含指定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="4dcf1-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="4dcf1-127">$orderby</span></span>        |<span data-ttu-id="4dcf1-128">string</span><span class="sxs-lookup"><span data-stu-id="4dcf1-128">string</span></span>   |<span data-ttu-id="4dcf1-129">默认情况下，响应中的对象按查询中的 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="4dcf1-130">可以使用 $orderby 参数 *更改响应* 的顺序。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="4dcf1-131">$select</span><span class="sxs-lookup"><span data-stu-id="4dcf1-131">$select</span></span>         |<span data-ttu-id="4dcf1-132">string</span><span class="sxs-lookup"><span data-stu-id="4dcf1-132">string</span></span>   |<span data-ttu-id="4dcf1-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="4dcf1-135">$skip</span><span class="sxs-lookup"><span data-stu-id="4dcf1-135">$skip</span></span>           |<span data-ttu-id="4dcf1-136">int</span><span class="sxs-lookup"><span data-stu-id="4dcf1-136">int</span></span>      |<span data-ttu-id="4dcf1-137">跳过前 n 个结果，可用于分页。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="4dcf1-138">$top</span><span class="sxs-lookup"><span data-stu-id="4dcf1-138">$top</span></span>            |<span data-ttu-id="4dcf1-139">int</span><span class="sxs-lookup"><span data-stu-id="4dcf1-139">int</span></span>      |<span data-ttu-id="4dcf1-140">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="4dcf1-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dcf1-141">Request headers</span></span>

| <span data-ttu-id="4dcf1-142">名称</span><span class="sxs-lookup"><span data-stu-id="4dcf1-142">Name</span></span>           |<span data-ttu-id="4dcf1-143">说明</span><span class="sxs-lookup"><span data-stu-id="4dcf1-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4dcf1-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dcf1-144">Authorization</span></span>  | <span data-ttu-id="4dcf1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="4dcf1-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dcf1-147">Request body</span></span>

<span data-ttu-id="4dcf1-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dcf1-149">响应</span><span class="sxs-lookup"><span data-stu-id="4dcf1-149">Response</span></span>

<span data-ttu-id="4dcf1-150">如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码和 educationalActivity](../resources/educationalactivity.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-150">If successful, this method returns a `200 OK` response code and a collection of [educationalActivity](../resources/educationalactivity.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4dcf1-151">示例</span><span class="sxs-lookup"><span data-stu-id="4dcf1-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4dcf1-152">请求</span><span class="sxs-lookup"><span data-stu-id="4dcf1-152">Request</span></span>

<span data-ttu-id="4dcf1-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4dcf1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dcf1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationalactivities"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities
```
# <a name="c"></a>[<span data-ttu-id="4dcf1-155">C#</span><span class="sxs-lookup"><span data-stu-id="4dcf1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4dcf1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dcf1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4dcf1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4dcf1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4dcf1-158">Java</span><span class="sxs-lookup"><span data-stu-id="4dcf1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationalactivities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4dcf1-159">响应</span><span class="sxs-lookup"><span data-stu-id="4dcf1-159">Response</span></span>

<span data-ttu-id="4dcf1-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-160">The following is an example of the response.</span></span>

> <span data-ttu-id="4dcf1-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4dcf1-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity",
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
      "completionMonthYear": "Date",
      "endMonthYear": "Date",
      "institution": {
        "description": null,
        "displayName": "Colorado State University",
        "location": {
          "type": "business",
          "postOfficeBox": null,
          "street": "12000 E Prospect Rd",
          "city": "Fort Collins",
          "state": "Colorado",
          "countryOrRegion": "USA",
          "postalCode": "80525"
        },
        "webUrl": "https://www.colostate.edu"
      },
      "program": {
        "abbreviation": "MBA",
        "activities": null,
        "awards": null,
        "description": "Master of Business Administration with a major in Entreprenuership and Finance.",
        "displayName": "Master of Business Administration",
        "fieldsOfStudy": null,
        "grade": "3.9",
        "notes": null,
        "webUrl": "https://biz.colostate.edu"
      },
      "startMonthYear": "Date"
    }
  ]
}
```


