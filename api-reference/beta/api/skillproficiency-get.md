---
title: 获取 skillProficiency
description: 检索 skillproficiency 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 053aad37ae5387fdd2b5ee427f5e38b0a5cb658b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938356"
---
# <a name="get-skillproficiency"></a><span data-ttu-id="e38c5-103">获取 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="e38c5-103">Get skillProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e38c5-104">在用户的[配置文件](../resources/profile.md)中检索[skillproficiency](../resources/skillproficiency.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e38c5-104">Retrieve the properties and relationships of a [skillproficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e38c5-105">权限</span><span class="sxs-lookup"><span data-stu-id="e38c5-105">Permissions</span></span>

<span data-ttu-id="e38c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e38c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e38c5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e38c5-108">Permission type</span></span>                        | <span data-ttu-id="e38c5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e38c5-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e38c5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e38c5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e38c5-111">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="e38c5-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e38c5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e38c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e38c5-113">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="e38c5-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e38c5-114">Application</span><span class="sxs-lookup"><span data-stu-id="e38c5-114">Application</span></span>                            | <span data-ttu-id="e38c5-115">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="e38c5-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e38c5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e38c5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e38c5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e38c5-117">Optional query parameters</span></span>

<span data-ttu-id="e38c5-118">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e38c5-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="e38c5-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e38c5-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="e38c5-120">名称</span><span class="sxs-lookup"><span data-stu-id="e38c5-120">Name</span></span>            |<span data-ttu-id="e38c5-121">值</span><span class="sxs-lookup"><span data-stu-id="e38c5-121">Value</span></span>    |<span data-ttu-id="e38c5-122">说明</span><span class="sxs-lookup"><span data-stu-id="e38c5-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e38c5-123">$filter</span><span class="sxs-lookup"><span data-stu-id="e38c5-123">$filter</span></span>         |<span data-ttu-id="e38c5-124">string</span><span class="sxs-lookup"><span data-stu-id="e38c5-124">string</span></span>   |<span data-ttu-id="e38c5-125">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="e38c5-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="e38c5-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="e38c5-126">$orderby</span></span>        |<span data-ttu-id="e38c5-127">string</span><span class="sxs-lookup"><span data-stu-id="e38c5-127">string</span></span>   |<span data-ttu-id="e38c5-128">默认情况下，响应中的对象按其在查询中的 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="e38c5-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="e38c5-129">您可以使用 *$orderby*参数更改响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="e38c5-129">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="e38c5-130">$select</span><span class="sxs-lookup"><span data-stu-id="e38c5-130">$select</span></span>         |<span data-ttu-id="e38c5-131">string</span><span class="sxs-lookup"><span data-stu-id="e38c5-131">string</span></span>   |<span data-ttu-id="e38c5-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="e38c5-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="e38c5-134">$skip</span><span class="sxs-lookup"><span data-stu-id="e38c5-134">$skip</span></span>           |<span data-ttu-id="e38c5-135">int</span><span class="sxs-lookup"><span data-stu-id="e38c5-135">int</span></span>      |<span data-ttu-id="e38c5-136">跳过前 n 个结果，对于分页非常有用。</span><span class="sxs-lookup"><span data-stu-id="e38c5-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="e38c5-137">$top</span><span class="sxs-lookup"><span data-stu-id="e38c5-137">$top</span></span>            |<span data-ttu-id="e38c5-138">int</span><span class="sxs-lookup"><span data-stu-id="e38c5-138">int</span></span>      |<span data-ttu-id="e38c5-139">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="e38c5-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="e38c5-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="e38c5-140">Request headers</span></span>

| <span data-ttu-id="e38c5-141">名称</span><span class="sxs-lookup"><span data-stu-id="e38c5-141">Name</span></span>           |<span data-ttu-id="e38c5-142">说明</span><span class="sxs-lookup"><span data-stu-id="e38c5-142">Description</span></span>                   |
|:---------------|:-----------------------------|
| <span data-ttu-id="e38c5-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="e38c5-143">Authorization</span></span>  | <span data-ttu-id="e38c5-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e38c5-p105">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="e38c5-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e38c5-146">Content-Type</span></span>   | <span data-ttu-id="e38c5-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e38c5-p106">application/json. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="e38c5-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="e38c5-149">Request body</span></span>

<span data-ttu-id="e38c5-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e38c5-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e38c5-151">响应</span><span class="sxs-lookup"><span data-stu-id="e38c5-151">Response</span></span>

<span data-ttu-id="e38c5-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[skillProficiency](../resources/skillproficiency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e38c5-152">If successful, this method returns a `200 OK` response code and the requested [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e38c5-153">示例</span><span class="sxs-lookup"><span data-stu-id="e38c5-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e38c5-154">请求</span><span class="sxs-lookup"><span data-stu-id="e38c5-154">Request</span></span>

<span data-ttu-id="e38c5-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e38c5-155">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_skillproficiency"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/skills/{id}
```

### <a name="response"></a><span data-ttu-id="e38c5-156">响应</span><span class="sxs-lookup"><span data-stu-id="e38c5-156">Response</span></span>

<span data-ttu-id="e38c5-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e38c5-157">The following is an example of the response.</span></span>

> <span data-ttu-id="e38c5-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e38c5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "displayName": "displayName-value",
  "proficiency": "proficiency-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get skillProficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->