---
title: 列出 webAccounts
description: 检索 webAccounts 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 49b617693fea47f266d95cf62ccc5b067969e934
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034629"
---
# <a name="list-webaccounts"></a><span data-ttu-id="817ce-103">列出 webAccounts</span><span class="sxs-lookup"><span data-stu-id="817ce-103">List webAccounts</span></span>

<span data-ttu-id="817ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="817ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="817ce-105">从用户的[配置文件](../resources/profile.md)中检索[webAccounts](../resources/webaccount.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="817ce-105">Retrieve a list of [webAccounts](../resources/webaccount.md) objects from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="817ce-106">权限</span><span class="sxs-lookup"><span data-stu-id="817ce-106">Permissions</span></span>

<span data-ttu-id="817ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="817ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="817ce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="817ce-109">Permission type</span></span>                        | <span data-ttu-id="817ce-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="817ce-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="817ce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="817ce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="817ce-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="817ce-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="817ce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="817ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="817ce-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="817ce-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="817ce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="817ce-115">Application</span></span>                            | <span data-ttu-id="817ce-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="817ce-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="817ce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="817ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/webAccounts
GET /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="817ce-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="817ce-118">Optional query parameters</span></span>

<span data-ttu-id="817ce-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="817ce-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="817ce-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="817ce-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="817ce-121">名称</span><span class="sxs-lookup"><span data-stu-id="817ce-121">Name</span></span>            |<span data-ttu-id="817ce-122">值</span><span class="sxs-lookup"><span data-stu-id="817ce-122">Value</span></span>    |<span data-ttu-id="817ce-123">说明</span><span class="sxs-lookup"><span data-stu-id="817ce-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="817ce-124">$filter</span><span class="sxs-lookup"><span data-stu-id="817ce-124">$filter</span></span>         |<span data-ttu-id="817ce-125">string</span><span class="sxs-lookup"><span data-stu-id="817ce-125">string</span></span>   |<span data-ttu-id="817ce-126">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="817ce-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="817ce-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="817ce-127">$orderby</span></span>        |<span data-ttu-id="817ce-128">string</span><span class="sxs-lookup"><span data-stu-id="817ce-128">string</span></span>   |<span data-ttu-id="817ce-129">默认情况下，响应中的对象按其在查询中的 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="817ce-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="817ce-130">您可以使用 *$orderby* 参数更改响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="817ce-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="817ce-131">$select</span><span class="sxs-lookup"><span data-stu-id="817ce-131">$select</span></span>         |<span data-ttu-id="817ce-132">string</span><span class="sxs-lookup"><span data-stu-id="817ce-132">string</span></span>   |<span data-ttu-id="817ce-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="817ce-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="817ce-135">$skip</span><span class="sxs-lookup"><span data-stu-id="817ce-135">$skip</span></span>           |<span data-ttu-id="817ce-136">int</span><span class="sxs-lookup"><span data-stu-id="817ce-136">int</span></span>      |<span data-ttu-id="817ce-137">跳过前 n 个结果，对于分页非常有用。</span><span class="sxs-lookup"><span data-stu-id="817ce-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="817ce-138">$top</span><span class="sxs-lookup"><span data-stu-id="817ce-138">$top</span></span>            |<span data-ttu-id="817ce-139">int</span><span class="sxs-lookup"><span data-stu-id="817ce-139">int</span></span>      |<span data-ttu-id="817ce-140">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="817ce-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="817ce-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="817ce-141">Request headers</span></span>

| <span data-ttu-id="817ce-142">名称</span><span class="sxs-lookup"><span data-stu-id="817ce-142">Name</span></span>           |<span data-ttu-id="817ce-143">说明</span><span class="sxs-lookup"><span data-stu-id="817ce-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="817ce-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="817ce-144">Authorization</span></span>  | <span data-ttu-id="817ce-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="817ce-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="817ce-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="817ce-147">Request body</span></span>

<span data-ttu-id="817ce-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="817ce-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="817ce-149">响应</span><span class="sxs-lookup"><span data-stu-id="817ce-149">Response</span></span>

<span data-ttu-id="817ce-150">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [webAccount](../resources/webaccount.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="817ce-150">If successful, this method returns a `200 OK` response code and a collection of [webAccount](../resources/webaccount.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="817ce-151">示例</span><span class="sxs-lookup"><span data-stu-id="817ce-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="817ce-152">请求</span><span class="sxs-lookup"><span data-stu-id="817ce-152">Request</span></span>

<span data-ttu-id="817ce-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="817ce-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="817ce-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="817ce-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_webaccounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/webAccounts
```
# <a name="c"></a>[<span data-ttu-id="817ce-155">C#</span><span class="sxs-lookup"><span data-stu-id="817ce-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-webaccounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="817ce-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="817ce-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-webaccounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="817ce-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="817ce-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-webaccounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="817ce-158">响应</span><span class="sxs-lookup"><span data-stu-id="817ce-158">Response</span></span>

<span data-ttu-id="817ce-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="817ce-159">The following is an example of the response.</span></span>

> <span data-ttu-id="817ce-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="817ce-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount",
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
      "description": "My Github contributions!",
      "userId": "innocenty.popov",
      "service": {
        "name": "GitHub",
        "webUrl": "https://github.com"
      },
      "statusMessage": null,
      "webUrl": "https://github.com/innocenty.popov"
    }
  ]
}
```


