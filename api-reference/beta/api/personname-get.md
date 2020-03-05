---
title: 获取 Contact.personname
description: 检索 Contact.personname 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8258abf0b39163ecce62ac601f52f8cbcec42004
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455887"
---
# <a name="get-personname"></a><span data-ttu-id="62423-103">获取 Contact.personname</span><span class="sxs-lookup"><span data-stu-id="62423-103">Get personName</span></span>

<span data-ttu-id="62423-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="62423-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62423-105">在用户的[配置文件](../resources/profile.md)中检索[contact.personname](../resources/personname.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62423-105">Retrieve the properties and relationships of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62423-106">权限</span><span class="sxs-lookup"><span data-stu-id="62423-106">Permissions</span></span>

<span data-ttu-id="62423-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62423-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62423-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62423-109">Permission type</span></span>                        | <span data-ttu-id="62423-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62423-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="62423-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62423-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62423-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="62423-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="62423-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62423-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62423-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="62423-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="62423-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62423-115">Application</span></span>                            | <span data-ttu-id="62423-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="62423-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="62423-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62423-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62423-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="62423-118">Optional query parameters</span></span>

<span data-ttu-id="62423-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="62423-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="62423-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="62423-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="62423-121">Name</span><span class="sxs-lookup"><span data-stu-id="62423-121">Name</span></span>            |<span data-ttu-id="62423-122">值</span><span class="sxs-lookup"><span data-stu-id="62423-122">Value</span></span>    |<span data-ttu-id="62423-123">说明</span><span class="sxs-lookup"><span data-stu-id="62423-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="62423-124">$filter</span><span class="sxs-lookup"><span data-stu-id="62423-124">$filter</span></span>         |<span data-ttu-id="62423-125">string</span><span class="sxs-lookup"><span data-stu-id="62423-125">string</span></span>   |<span data-ttu-id="62423-126">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="62423-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="62423-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="62423-127">$orderby</span></span>        |<span data-ttu-id="62423-128">string</span><span class="sxs-lookup"><span data-stu-id="62423-128">string</span></span>   |<span data-ttu-id="62423-129">默认情况下，响应中的对象按其在查询中的 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="62423-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="62423-130">您可以使用 *$orderby*参数更改响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="62423-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="62423-131">$select</span><span class="sxs-lookup"><span data-stu-id="62423-131">$select</span></span>         |<span data-ttu-id="62423-132">string</span><span class="sxs-lookup"><span data-stu-id="62423-132">string</span></span>   |<span data-ttu-id="62423-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="62423-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="62423-135">$skip</span><span class="sxs-lookup"><span data-stu-id="62423-135">$skip</span></span>           |<span data-ttu-id="62423-136">int</span><span class="sxs-lookup"><span data-stu-id="62423-136">int</span></span>      |<span data-ttu-id="62423-137">跳过前 n 个结果，对于分页非常有用。</span><span class="sxs-lookup"><span data-stu-id="62423-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="62423-138">$top</span><span class="sxs-lookup"><span data-stu-id="62423-138">$top</span></span>            |<span data-ttu-id="62423-139">int</span><span class="sxs-lookup"><span data-stu-id="62423-139">int</span></span>      |<span data-ttu-id="62423-140">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="62423-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="62423-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="62423-141">Request headers</span></span>

| <span data-ttu-id="62423-142">名称</span><span class="sxs-lookup"><span data-stu-id="62423-142">Name</span></span>           |<span data-ttu-id="62423-143">说明</span><span class="sxs-lookup"><span data-stu-id="62423-143">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="62423-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="62423-144">Authorization</span></span>  | <span data-ttu-id="62423-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62423-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="62423-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="62423-147">Content-Type</span></span>   | <span data-ttu-id="62423-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="62423-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62423-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="62423-150">Request body</span></span>

<span data-ttu-id="62423-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62423-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62423-152">响应</span><span class="sxs-lookup"><span data-stu-id="62423-152">Response</span></span>

<span data-ttu-id="62423-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[contact.personname](../resources/personname.md)对象。</span><span class="sxs-lookup"><span data-stu-id="62423-153">If successful, this method returns a `200 OK` response code and the requested [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62423-154">示例</span><span class="sxs-lookup"><span data-stu-id="62423-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62423-155">请求</span><span class="sxs-lookup"><span data-stu-id="62423-155">Request</span></span>

<span data-ttu-id="62423-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62423-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62423-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="62423-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personname"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names/{id}
```
# <a name="c"></a>[<span data-ttu-id="62423-158">C#</span><span class="sxs-lookup"><span data-stu-id="62423-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62423-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62423-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62423-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62423-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62423-161">响应</span><span class="sxs-lookup"><span data-stu-id="62423-161">Response</span></span>

<span data-ttu-id="62423-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62423-162">The following is an example of the response.</span></span>

> <span data-ttu-id="62423-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62423-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
