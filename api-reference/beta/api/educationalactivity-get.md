---
title: 获取 educationalActivity
description: 检索 educationalactivity 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 980f7f246ec40a8822502c3c22497ee408f2fe8c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994779"
---
# <a name="get-educationalactivity"></a><span data-ttu-id="d78db-103">获取 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="d78db-103">Get educationalActivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d78db-104">从用户配置文件中检索[educationalActivity](../resources/educationalactivity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d78db-104">Retrieve the properties and relationships of an [educationalActivity](../resources/educationalactivity.md) object from a users profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="d78db-105">权限</span><span class="sxs-lookup"><span data-stu-id="d78db-105">Permissions</span></span>

<span data-ttu-id="d78db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d78db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d78db-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d78db-108">Permission type</span></span>                        | <span data-ttu-id="d78db-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d78db-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d78db-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d78db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d78db-111">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="d78db-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d78db-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d78db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d78db-113">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="d78db-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d78db-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d78db-114">Application</span></span>                            | <span data-ttu-id="d78db-115">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="d78db-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="d78db-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d78db-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/educationalActivities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d78db-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d78db-117">Optional query parameters</span></span>

<span data-ttu-id="d78db-118">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d78db-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="d78db-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d78db-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="d78db-120">名称</span><span class="sxs-lookup"><span data-stu-id="d78db-120">Name</span></span>            |<span data-ttu-id="d78db-121">值</span><span class="sxs-lookup"><span data-stu-id="d78db-121">Value</span></span>    |<span data-ttu-id="d78db-122">说明</span><span class="sxs-lookup"><span data-stu-id="d78db-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d78db-123">$filter</span><span class="sxs-lookup"><span data-stu-id="d78db-123">$filter</span></span>         |<span data-ttu-id="d78db-124">string</span><span class="sxs-lookup"><span data-stu-id="d78db-124">string</span></span>   |<span data-ttu-id="d78db-125">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="d78db-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="d78db-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="d78db-126">$orderby</span></span>        |<span data-ttu-id="d78db-127">string</span><span class="sxs-lookup"><span data-stu-id="d78db-127">string</span></span>   |<span data-ttu-id="d78db-128">默认情况下，响应中的对象按其在查询中的 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="d78db-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="d78db-129">您可以使用`$orderby`参数更改响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="d78db-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="d78db-130">$select</span><span class="sxs-lookup"><span data-stu-id="d78db-130">$select</span></span>         |<span data-ttu-id="d78db-131">string</span><span class="sxs-lookup"><span data-stu-id="d78db-131">string</span></span>   |<span data-ttu-id="d78db-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="d78db-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="d78db-134">$skip</span><span class="sxs-lookup"><span data-stu-id="d78db-134">$skip</span></span>           |<span data-ttu-id="d78db-135">int</span><span class="sxs-lookup"><span data-stu-id="d78db-135">int</span></span>      |<span data-ttu-id="d78db-136">跳过前 n 个结果，对于分页非常有用。</span><span class="sxs-lookup"><span data-stu-id="d78db-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="d78db-137">$top</span><span class="sxs-lookup"><span data-stu-id="d78db-137">$top</span></span>            |<span data-ttu-id="d78db-138">int</span><span class="sxs-lookup"><span data-stu-id="d78db-138">int</span></span>      |<span data-ttu-id="d78db-139">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="d78db-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="d78db-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="d78db-140">Request headers</span></span>

| <span data-ttu-id="d78db-141">名称</span><span class="sxs-lookup"><span data-stu-id="d78db-141">Name</span></span>           |<span data-ttu-id="d78db-142">说明</span><span class="sxs-lookup"><span data-stu-id="d78db-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d78db-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="d78db-143">Authorization</span></span>  | <span data-ttu-id="d78db-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d78db-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="d78db-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="d78db-146">Request body</span></span>

<span data-ttu-id="d78db-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d78db-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d78db-148">响应</span><span class="sxs-lookup"><span data-stu-id="d78db-148">Response</span></span>

<span data-ttu-id="d78db-149">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[educationalActivity](../resources/educationalactivity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d78db-149">If successful, this method returns a `200 OK` response code and the requested [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d78db-150">示例</span><span class="sxs-lookup"><span data-stu-id="d78db-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d78db-151">请求</span><span class="sxs-lookup"><span data-stu-id="d78db-151">Request</span></span>

<span data-ttu-id="d78db-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d78db-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d78db-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d78db-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationalactivity"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d78db-154">C#</span><span class="sxs-lookup"><span data-stu-id="d78db-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d78db-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d78db-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d78db-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d78db-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d78db-157">响应</span><span class="sxs-lookup"><span data-stu-id="d78db-157">Response</span></span>

<span data-ttu-id="d78db-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d78db-158">The following is an example of the response.</span></span>

> <span data-ttu-id="d78db-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d78db-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
