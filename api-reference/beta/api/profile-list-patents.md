---
title: 列出性
description: 从 patents 导航属性中获取项。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9a425f77d11d6a229c6397702ab2908ff1c6f576
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820135"
---
# <a name="list-patents"></a><span data-ttu-id="ed32f-103">列出性</span><span class="sxs-lookup"><span data-stu-id="ed32f-103">List patents</span></span>

<span data-ttu-id="ed32f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed32f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed32f-105">从用户的 [配置文件检索 itemPatent](../resources/itempatent.md) 对象 [列表](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="ed32f-105">Retrieve a list of [itemPatent](../resources/itempatent.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed32f-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed32f-106">Permissions</span></span>

<span data-ttu-id="ed32f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed32f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed32f-109">Permission type</span></span>                        | <span data-ttu-id="ed32f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed32f-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ed32f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed32f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed32f-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed32f-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ed32f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed32f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed32f-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed32f-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ed32f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed32f-115">Application</span></span>                            | <span data-ttu-id="ed32f-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed32f-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="ed32f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed32f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/patents
GET /users/{id | userPrincipalName}/profile/patents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed32f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed32f-118">Optional query parameters</span></span>

<span data-ttu-id="ed32f-119">此方法支持以下 OData 查询参数，这有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed32f-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="ed32f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ed32f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="ed32f-121">名称</span><span class="sxs-lookup"><span data-stu-id="ed32f-121">Name</span></span>            |<span data-ttu-id="ed32f-122">值</span><span class="sxs-lookup"><span data-stu-id="ed32f-122">Value</span></span>    |<span data-ttu-id="ed32f-123">说明</span><span class="sxs-lookup"><span data-stu-id="ed32f-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="ed32f-124">$filter</span><span class="sxs-lookup"><span data-stu-id="ed32f-124">$filter</span></span>         |<span data-ttu-id="ed32f-125">string</span><span class="sxs-lookup"><span data-stu-id="ed32f-125">string</span></span>   |<span data-ttu-id="ed32f-126">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="ed32f-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="ed32f-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="ed32f-127">$orderby</span></span>        |<span data-ttu-id="ed32f-128">string</span><span class="sxs-lookup"><span data-stu-id="ed32f-128">string</span></span>   |<span data-ttu-id="ed32f-129">默认情况下，响应中的对象在查询中按其 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="ed32f-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="ed32f-130">可以使用 $orderby 参数更改响应 *$orderby* 顺序。</span><span class="sxs-lookup"><span data-stu-id="ed32f-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="ed32f-131">$select</span><span class="sxs-lookup"><span data-stu-id="ed32f-131">$select</span></span>         |<span data-ttu-id="ed32f-132">string</span><span class="sxs-lookup"><span data-stu-id="ed32f-132">string</span></span>   |<span data-ttu-id="ed32f-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="ed32f-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="ed32f-135">$skip</span><span class="sxs-lookup"><span data-stu-id="ed32f-135">$skip</span></span>           |<span data-ttu-id="ed32f-136">int</span><span class="sxs-lookup"><span data-stu-id="ed32f-136">int</span></span>      |<span data-ttu-id="ed32f-137">跳过前 n 个结果，可用于分页。</span><span class="sxs-lookup"><span data-stu-id="ed32f-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="ed32f-138">$top</span><span class="sxs-lookup"><span data-stu-id="ed32f-138">$top</span></span>            |<span data-ttu-id="ed32f-139">int</span><span class="sxs-lookup"><span data-stu-id="ed32f-139">int</span></span>      |<span data-ttu-id="ed32f-140">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="ed32f-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="ed32f-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed32f-141">Request headers</span></span>
|<span data-ttu-id="ed32f-142">名称</span><span class="sxs-lookup"><span data-stu-id="ed32f-142">Name</span></span>|<span data-ttu-id="ed32f-143">说明</span><span class="sxs-lookup"><span data-stu-id="ed32f-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed32f-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed32f-144">Authorization</span></span>|<span data-ttu-id="ed32f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed32f-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed32f-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed32f-147">Request body</span></span>
<span data-ttu-id="ed32f-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed32f-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed32f-149">响应</span><span class="sxs-lookup"><span data-stu-id="ed32f-149">Response</span></span>

<span data-ttu-id="ed32f-150">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [itemPatent](../resources/itempatent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ed32f-150">If successful, this method returns a `200 OK` response code and a collection of [itemPatent](../resources/itempatent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed32f-151">示例</span><span class="sxs-lookup"><span data-stu-id="ed32f-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="ed32f-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed32f-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itempatents_from_profile"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/patents
```
# <a name="c"></a>[<span data-ttu-id="ed32f-153">C#</span><span class="sxs-lookup"><span data-stu-id="ed32f-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itempatents-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed32f-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed32f-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itempatents-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed32f-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed32f-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itempatents-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ed32f-156">响应</span><span class="sxs-lookup"><span data-stu-id="ed32f-156">Response</span></span>
<span data-ttu-id="ed32f-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed32f-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemPatent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
      "allowedAudiences": "me",
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
      "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
      "displayName": "Inferring User Intent through browsing behaviors",
      "isPending": true,
      "issuedDate": "Date",
      "issuingAuthority": null,
      "number": "USPTO-3954432633",
      "webUrl": "https://patents.gov/3954432633"
    }
  ]
}
```
