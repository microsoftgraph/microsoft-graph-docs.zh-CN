---
title: 列表奖项
description: 从奖项导航属性中获取 personAwards 的集合。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a67a8819ead51647db8f598cbc027694c0f3a048
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812955"
---
# <a name="list-awards"></a><span data-ttu-id="8d29d-103">列表奖项</span><span class="sxs-lookup"><span data-stu-id="8d29d-103">List awards</span></span>

<span data-ttu-id="8d29d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d29d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d29d-105">从用户的[配置文件](../resources/profile.md)中检索[personAward](../resources/personaward.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8d29d-105">Retrieve a list of [personAward](../resources/personaward.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d29d-106">权限</span><span class="sxs-lookup"><span data-stu-id="8d29d-106">Permissions</span></span>

<span data-ttu-id="8d29d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d29d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d29d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d29d-109">Permission type</span></span>                        | <span data-ttu-id="8d29d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d29d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="8d29d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d29d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d29d-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="8d29d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8d29d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d29d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d29d-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="8d29d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8d29d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d29d-115">Application</span></span>                            | <span data-ttu-id="8d29d-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="8d29d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="8d29d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d29d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/awards
GET /users/{id | userPrincipalName}/profile/awards
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d29d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d29d-118">Optional query parameters</span></span>

<span data-ttu-id="8d29d-119">此方法支持以下 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8d29d-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="8d29d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8d29d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="8d29d-121">名称</span><span class="sxs-lookup"><span data-stu-id="8d29d-121">Name</span></span>            |<span data-ttu-id="8d29d-122">值</span><span class="sxs-lookup"><span data-stu-id="8d29d-122">Value</span></span>    |<span data-ttu-id="8d29d-123">说明</span><span class="sxs-lookup"><span data-stu-id="8d29d-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="8d29d-124">$filter</span><span class="sxs-lookup"><span data-stu-id="8d29d-124">$filter</span></span>         |<span data-ttu-id="8d29d-125">string</span><span class="sxs-lookup"><span data-stu-id="8d29d-125">string</span></span>   |<span data-ttu-id="8d29d-126">将响应限制为仅包含指定条件的那些对象。</span><span class="sxs-lookup"><span data-stu-id="8d29d-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="8d29d-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="8d29d-127">$orderby</span></span>        |<span data-ttu-id="8d29d-128">string</span><span class="sxs-lookup"><span data-stu-id="8d29d-128">string</span></span>   |<span data-ttu-id="8d29d-129">默认情况下，响应中的对象按其在查询中的 createdDateTime 值进行排序。</span><span class="sxs-lookup"><span data-stu-id="8d29d-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="8d29d-130">您可以使用 *$orderby* 参数更改响应的顺序。</span><span class="sxs-lookup"><span data-stu-id="8d29d-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="8d29d-131">$select</span><span class="sxs-lookup"><span data-stu-id="8d29d-131">$select</span></span>         |<span data-ttu-id="8d29d-132">string</span><span class="sxs-lookup"><span data-stu-id="8d29d-132">string</span></span>   |<span data-ttu-id="8d29d-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="8d29d-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="8d29d-135">$skip</span><span class="sxs-lookup"><span data-stu-id="8d29d-135">$skip</span></span>           |<span data-ttu-id="8d29d-136">int</span><span class="sxs-lookup"><span data-stu-id="8d29d-136">int</span></span>      |<span data-ttu-id="8d29d-137">跳过前 n 个结果，对于分页非常有用。</span><span class="sxs-lookup"><span data-stu-id="8d29d-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="8d29d-138">$top</span><span class="sxs-lookup"><span data-stu-id="8d29d-138">$top</span></span>            |<span data-ttu-id="8d29d-139">int</span><span class="sxs-lookup"><span data-stu-id="8d29d-139">int</span></span>      |<span data-ttu-id="8d29d-140">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="8d29d-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="8d29d-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d29d-141">Request headers</span></span>
|<span data-ttu-id="8d29d-142">名称</span><span class="sxs-lookup"><span data-stu-id="8d29d-142">Name</span></span>|<span data-ttu-id="8d29d-143">说明</span><span class="sxs-lookup"><span data-stu-id="8d29d-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d29d-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d29d-144">Authorization</span></span>|<span data-ttu-id="8d29d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d29d-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d29d-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d29d-147">Request body</span></span>
<span data-ttu-id="8d29d-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d29d-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d29d-149">响应</span><span class="sxs-lookup"><span data-stu-id="8d29d-149">Response</span></span>

<span data-ttu-id="8d29d-150">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [personAward](../resources/personaward.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d29d-150">If successful, this method returns a `200 OK` response code and a collection of [personAward](../resources/personaward.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d29d-151">示例</span><span class="sxs-lookup"><span data-stu-id="8d29d-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="8d29d-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d29d-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemawards_from_profile"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/awards
```
# <a name="c"></a>[<span data-ttu-id="8d29d-153">C#</span><span class="sxs-lookup"><span data-stu-id="8d29d-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d29d-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d29d-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d29d-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d29d-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8d29d-156">响应</span><span class="sxs-lookup"><span data-stu-id="8d29d-156">Response</span></span>
<span data-ttu-id="8d29d-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8d29d-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personAward)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
      "description": "Lifetime Achievement award from the International Association of Branding Managers",
      "displayName": "Lifetime Achievement Award For Excellence in Branding",
      "issuedDate": "Date",
      "issuingAuthority": "International Association of Branding Management",
      "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
      "webUrl": "https://www.iabm.io"
    }
  ]
}
```
