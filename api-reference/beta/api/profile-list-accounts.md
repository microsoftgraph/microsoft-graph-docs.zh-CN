---
title: 列出帐户
description: 检索 userAccountInformation 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 97d8209e6badb9917768513e1db31d7ccaa2d30a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441088"
---
# <a name="list-accounts"></a><span data-ttu-id="fd99b-103">列出帐户</span><span class="sxs-lookup"><span data-stu-id="fd99b-103">List accounts</span></span>

<span data-ttu-id="fd99b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd99b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd99b-105">从配置文件中检索与用户帐户相关的 [属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="fd99b-105">Retrieves properties related to the user's accounts from the [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd99b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fd99b-106">Permissions</span></span>

<span data-ttu-id="fd99b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd99b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd99b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd99b-109">Permission type</span></span>                        | <span data-ttu-id="fd99b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd99b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="fd99b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd99b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd99b-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd99b-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fd99b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd99b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd99b-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd99b-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fd99b-115">Application</span><span class="sxs-lookup"><span data-stu-id="fd99b-115">Application</span></span>                            | <span data-ttu-id="fd99b-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd99b-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="fd99b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd99b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
GET /users/{id | userPrincipalName}/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd99b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fd99b-118">Optional query parameters</span></span>

<span data-ttu-id="fd99b-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fd99b-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="fd99b-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="fd99b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="fd99b-121">名称</span><span class="sxs-lookup"><span data-stu-id="fd99b-121">Name</span></span>            |<span data-ttu-id="fd99b-122">值</span><span class="sxs-lookup"><span data-stu-id="fd99b-122">Value</span></span>    |<span data-ttu-id="fd99b-123">说明</span><span class="sxs-lookup"><span data-stu-id="fd99b-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="fd99b-124">$filter</span><span class="sxs-lookup"><span data-stu-id="fd99b-124">$filter</span></span>         |<span data-ttu-id="fd99b-125">string</span><span class="sxs-lookup"><span data-stu-id="fd99b-125">string</span></span>   |<span data-ttu-id="fd99b-126">将响应限制到仅包含指定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="fd99b-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="fd99b-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="fd99b-127">$orderby</span></span>        |<span data-ttu-id="fd99b-128">string</span><span class="sxs-lookup"><span data-stu-id="fd99b-128">string</span></span>   |<span data-ttu-id="fd99b-129">默认情况下，响应中的对象按查询中的 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="fd99b-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="fd99b-130">可以使用 $orderby 参数更改 *响应* 的顺序。</span><span class="sxs-lookup"><span data-stu-id="fd99b-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="fd99b-131">$select</span><span class="sxs-lookup"><span data-stu-id="fd99b-131">$select</span></span>         |<span data-ttu-id="fd99b-132">string</span><span class="sxs-lookup"><span data-stu-id="fd99b-132">string</span></span>   |<span data-ttu-id="fd99b-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="fd99b-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="fd99b-135">$skip</span><span class="sxs-lookup"><span data-stu-id="fd99b-135">$skip</span></span>           |<span data-ttu-id="fd99b-136">int</span><span class="sxs-lookup"><span data-stu-id="fd99b-136">int</span></span>      |<span data-ttu-id="fd99b-137">跳过前 n 个结果，对分页很有用。</span><span class="sxs-lookup"><span data-stu-id="fd99b-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="fd99b-138">$top</span><span class="sxs-lookup"><span data-stu-id="fd99b-138">$top</span></span>            |<span data-ttu-id="fd99b-139">int</span><span class="sxs-lookup"><span data-stu-id="fd99b-139">int</span></span>      |<span data-ttu-id="fd99b-140">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="fd99b-140">Number of results to be returned.</span></span>                                                                                                                                           |


## <a name="request-headers"></a><span data-ttu-id="fd99b-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd99b-141">Request headers</span></span>

| <span data-ttu-id="fd99b-142">名称</span><span class="sxs-lookup"><span data-stu-id="fd99b-142">Name</span></span>           |<span data-ttu-id="fd99b-143">说明</span><span class="sxs-lookup"><span data-stu-id="fd99b-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="fd99b-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd99b-144">Authorization</span></span>  | <span data-ttu-id="fd99b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd99b-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="fd99b-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd99b-147">Content-Type</span></span>   | <span data-ttu-id="fd99b-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fd99b-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd99b-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd99b-150">Request body</span></span>

<span data-ttu-id="fd99b-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fd99b-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd99b-152">响应</span><span class="sxs-lookup"><span data-stu-id="fd99b-152">Response</span></span>

<span data-ttu-id="fd99b-153">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userAccountInformation](../resources/useraccountinformation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fd99b-153">If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd99b-154">示例</span><span class="sxs-lookup"><span data-stu-id="fd99b-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd99b-155">请求</span><span class="sxs-lookup"><span data-stu-id="fd99b-155">Request</span></span>

<span data-ttu-id="fd99b-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fd99b-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fd99b-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd99b-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account
```
# <a name="c"></a>[<span data-ttu-id="fd99b-158">C#</span><span class="sxs-lookup"><span data-stu-id="fd99b-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-account-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd99b-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd99b-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-account-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd99b-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd99b-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-account-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd99b-161">Java</span><span class="sxs-lookup"><span data-stu-id="fd99b-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-account-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fd99b-162">响应</span><span class="sxs-lookup"><span data-stu-id="fd99b-162">Response</span></span>

<span data-ttu-id="fd99b-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fd99b-163">The following is an example of the response.</span></span>

> <span data-ttu-id="fd99b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fd99b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation",
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
      "ageGroup": "adult",
      "countryCode": "NO",
      "preferredLanguageTag": null,
      "userPrincipalName": "innocenty.popov@adventureworks.com"
    }
  ]
}
```


