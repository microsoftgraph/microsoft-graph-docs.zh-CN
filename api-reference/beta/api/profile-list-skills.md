---
title: 列表技能
description: 检索 skillProficiency 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bfaa9d5eb967391627df730c913ec805217b48e6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937740"
---
# <a name="list-skills"></a><span data-ttu-id="ed5d1-103">列表技能</span><span class="sxs-lookup"><span data-stu-id="ed5d1-103">List skills</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed5d1-104">在用户的[配置文件](../resources/profile.md)中检索[skillProficiency](../resources/skillproficiency.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-104">Retrieve a list of [skillProficiency](../resources/skillproficiency.md) objects in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed5d1-105">权限</span><span class="sxs-lookup"><span data-stu-id="ed5d1-105">Permissions</span></span>

<span data-ttu-id="ed5d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed5d1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed5d1-108">Permission type</span></span>                        | <span data-ttu-id="ed5d1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed5d1-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ed5d1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5d1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed5d1-111">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="ed5d1-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ed5d1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed5d1-113">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="ed5d1-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ed5d1-114">Application</span><span class="sxs-lookup"><span data-stu-id="ed5d1-114">Application</span></span>                            | <span data-ttu-id="ed5d1-115">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="ed5d1-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="ed5d1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed5d1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed5d1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed5d1-117">Optional query parameters</span></span>

<span data-ttu-id="ed5d1-118">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="ed5d1-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="ed5d1-120">名称</span><span class="sxs-lookup"><span data-stu-id="ed5d1-120">Name</span></span>            |<span data-ttu-id="ed5d1-121">值</span><span class="sxs-lookup"><span data-stu-id="ed5d1-121">Value</span></span>    |<span data-ttu-id="ed5d1-122">说明</span><span class="sxs-lookup"><span data-stu-id="ed5d1-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="ed5d1-123">$filter</span><span class="sxs-lookup"><span data-stu-id="ed5d1-123">$filter</span></span>         |<span data-ttu-id="ed5d1-124">string</span><span class="sxs-lookup"><span data-stu-id="ed5d1-124">string</span></span>   |<span data-ttu-id="ed5d1-125">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="ed5d1-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="ed5d1-126">$orderby</span></span>        |<span data-ttu-id="ed5d1-127">string</span><span class="sxs-lookup"><span data-stu-id="ed5d1-127">string</span></span>   |<span data-ttu-id="ed5d1-128">默认情况下，响应中的对象按其在查询中的**createdDateTime**值进行排序。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-128">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="ed5d1-129">您可以使用`$orderby`参数更改响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="ed5d1-130">$select</span><span class="sxs-lookup"><span data-stu-id="ed5d1-130">$select</span></span>         |<span data-ttu-id="ed5d1-131">string</span><span class="sxs-lookup"><span data-stu-id="ed5d1-131">string</span></span>   |<span data-ttu-id="ed5d1-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="ed5d1-134">$skip</span><span class="sxs-lookup"><span data-stu-id="ed5d1-134">$skip</span></span>           |<span data-ttu-id="ed5d1-135">int</span><span class="sxs-lookup"><span data-stu-id="ed5d1-135">int</span></span>      |<span data-ttu-id="ed5d1-136">跳过前 n 个结果，对于分页非常有用。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="ed5d1-137">$top</span><span class="sxs-lookup"><span data-stu-id="ed5d1-137">$top</span></span>            |<span data-ttu-id="ed5d1-138">int</span><span class="sxs-lookup"><span data-stu-id="ed5d1-138">int</span></span>      |<span data-ttu-id="ed5d1-139">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="ed5d1-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed5d1-140">Request headers</span></span>

| <span data-ttu-id="ed5d1-141">名称</span><span class="sxs-lookup"><span data-stu-id="ed5d1-141">Name</span></span>           |<span data-ttu-id="ed5d1-142">说明</span><span class="sxs-lookup"><span data-stu-id="ed5d1-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ed5d1-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed5d1-143">Authorization</span></span>  | <span data-ttu-id="ed5d1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ed5d1-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed5d1-146">Content-Type</span></span>   | <span data-ttu-id="ed5d1-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ed5d1-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed5d1-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed5d1-149">Request body</span></span>

<span data-ttu-id="ed5d1-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed5d1-151">响应</span><span class="sxs-lookup"><span data-stu-id="ed5d1-151">Response</span></span>

<span data-ttu-id="ed5d1-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和[skillProficiency](../resources/skillproficiency.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-152">If successful, this method returns a `200 OK` response code and a collection of [skillProficiency](../resources/skillproficiency.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed5d1-153">示例</span><span class="sxs-lookup"><span data-stu-id="ed5d1-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed5d1-154">请求</span><span class="sxs-lookup"><span data-stu-id="ed5d1-154">Request</span></span>

<span data-ttu-id="ed5d1-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-155">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_skills"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/skills
```

### <a name="response"></a><span data-ttu-id="ed5d1-156">响应</span><span class="sxs-lookup"><span data-stu-id="ed5d1-156">Response</span></span>

<span data-ttu-id="ed5d1-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-157">The following is an example of the response.</span></span>

> <span data-ttu-id="ed5d1-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ed5d1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "categories": [
        "categories-value"
      ],
      "displayName": "displayName-value",
      "proficiency": "proficiency-value",
      "webUrl": "webUrl-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List skills",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
