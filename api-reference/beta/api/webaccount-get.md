---
title: 获取 webAccount
description: 检索 webAccount 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 86b0307de43db9cf8cb97c50691bf656b1c1c9a8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937600"
---
# <a name="get-webaccount"></a><span data-ttu-id="1069f-103">获取 webAccount</span><span class="sxs-lookup"><span data-stu-id="1069f-103">Get webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1069f-104">从用户的[配置文件](../resources/profile.md)中检索[webAccount](../resources/webaccount.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1069f-104">Retrieve the properties and relationships of a [webAccount](../resources/webaccount.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1069f-105">权限</span><span class="sxs-lookup"><span data-stu-id="1069f-105">Permissions</span></span>

<span data-ttu-id="1069f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1069f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1069f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1069f-108">Permission type</span></span>                        | <span data-ttu-id="1069f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1069f-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="1069f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1069f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1069f-111">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="1069f-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1069f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1069f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1069f-113">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="1069f-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1069f-114">Application</span><span class="sxs-lookup"><span data-stu-id="1069f-114">Application</span></span>                            | <span data-ttu-id="1069f-115">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="1069f-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="1069f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1069f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/webAccounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1069f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1069f-117">Optional query parameters</span></span>

<span data-ttu-id="1069f-118">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1069f-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="1069f-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1069f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="1069f-120">名称</span><span class="sxs-lookup"><span data-stu-id="1069f-120">Name</span></span>            |<span data-ttu-id="1069f-121">值</span><span class="sxs-lookup"><span data-stu-id="1069f-121">Value</span></span>    |<span data-ttu-id="1069f-122">说明</span><span class="sxs-lookup"><span data-stu-id="1069f-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="1069f-123">$filter</span><span class="sxs-lookup"><span data-stu-id="1069f-123">$filter</span></span>         |<span data-ttu-id="1069f-124">string</span><span class="sxs-lookup"><span data-stu-id="1069f-124">string</span></span>   |<span data-ttu-id="1069f-125">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="1069f-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="1069f-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="1069f-126">$orderby</span></span>        |<span data-ttu-id="1069f-127">string</span><span class="sxs-lookup"><span data-stu-id="1069f-127">string</span></span>   |<span data-ttu-id="1069f-128">默认情况下，响应中的对象按其在查询中的**createdDateTime**值进行排序。</span><span class="sxs-lookup"><span data-stu-id="1069f-128">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="1069f-129">您可以使用`$orderby`参数更改响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="1069f-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="1069f-130">$select</span><span class="sxs-lookup"><span data-stu-id="1069f-130">$select</span></span>         |<span data-ttu-id="1069f-131">string</span><span class="sxs-lookup"><span data-stu-id="1069f-131">string</span></span>   |<span data-ttu-id="1069f-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="1069f-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="1069f-134">$skip</span><span class="sxs-lookup"><span data-stu-id="1069f-134">$skip</span></span>           |<span data-ttu-id="1069f-135">int</span><span class="sxs-lookup"><span data-stu-id="1069f-135">int</span></span>      |<span data-ttu-id="1069f-136">跳过前 n 个结果，对于分页非常有用。</span><span class="sxs-lookup"><span data-stu-id="1069f-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="1069f-137">$top</span><span class="sxs-lookup"><span data-stu-id="1069f-137">$top</span></span>            |<span data-ttu-id="1069f-138">int</span><span class="sxs-lookup"><span data-stu-id="1069f-138">int</span></span>      |<span data-ttu-id="1069f-139">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="1069f-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="1069f-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="1069f-140">Request headers</span></span>

| <span data-ttu-id="1069f-141">名称</span><span class="sxs-lookup"><span data-stu-id="1069f-141">Name</span></span>           |<span data-ttu-id="1069f-142">说明</span><span class="sxs-lookup"><span data-stu-id="1069f-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1069f-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="1069f-143">Authorization</span></span>  | <span data-ttu-id="1069f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1069f-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="1069f-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="1069f-146">Request body</span></span>

<span data-ttu-id="1069f-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1069f-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1069f-148">响应</span><span class="sxs-lookup"><span data-stu-id="1069f-148">Response</span></span>

<span data-ttu-id="1069f-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[webAccount](../resources/webaccount.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1069f-149">If successful, this method returns a `200 OK` response code and the requested [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1069f-150">示例</span><span class="sxs-lookup"><span data-stu-id="1069f-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1069f-151">请求</span><span class="sxs-lookup"><span data-stu-id="1069f-151">Request</span></span>

<span data-ttu-id="1069f-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1069f-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_webaccount"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
```

### <a name="response"></a><span data-ttu-id="1069f-153">响应</span><span class="sxs-lookup"><span data-stu-id="1069f-153">Response</span></span>

<span data-ttu-id="1069f-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1069f-154">The following is an example of the response.</span></span>

> <span data-ttu-id="1069f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1069f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
