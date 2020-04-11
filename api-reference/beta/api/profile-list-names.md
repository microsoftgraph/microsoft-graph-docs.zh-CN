---
title: 列出名称
description: 从用户的配置文件中检索 Contact.personname 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 87688a8e8049370ebe6a0bd4929450f3de7a1301
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228658"
---
# <a name="list-names"></a><span data-ttu-id="17d48-103">列出名称</span><span class="sxs-lookup"><span data-stu-id="17d48-103">List names</span></span>

<span data-ttu-id="17d48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17d48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17d48-105">从用户的[配置文件](../resources/profile.md)中检索[contact.personname](../resources/personname.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="17d48-105">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="17d48-106">权限</span><span class="sxs-lookup"><span data-stu-id="17d48-106">Permissions</span></span>

<span data-ttu-id="17d48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17d48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17d48-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="17d48-109">Permission type</span></span>                        | <span data-ttu-id="17d48-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17d48-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="17d48-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17d48-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="17d48-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="17d48-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="17d48-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17d48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17d48-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="17d48-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="17d48-115">Application</span><span class="sxs-lookup"><span data-stu-id="17d48-115">Application</span></span>                            | <span data-ttu-id="17d48-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="17d48-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="17d48-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17d48-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17d48-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="17d48-118">Optional query parameters</span></span>

<span data-ttu-id="17d48-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="17d48-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="17d48-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="17d48-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="17d48-121">请求头</span><span class="sxs-lookup"><span data-stu-id="17d48-121">Request headers</span></span>

| <span data-ttu-id="17d48-122">名称</span><span class="sxs-lookup"><span data-stu-id="17d48-122">Name</span></span>           |<span data-ttu-id="17d48-123">说明</span><span class="sxs-lookup"><span data-stu-id="17d48-123">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="17d48-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="17d48-124">Authorization</span></span>  | <span data-ttu-id="17d48-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17d48-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="17d48-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17d48-127">Content-Type</span></span>   | <span data-ttu-id="17d48-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="17d48-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17d48-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="17d48-130">Request body</span></span>

<span data-ttu-id="17d48-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17d48-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17d48-132">响应</span><span class="sxs-lookup"><span data-stu-id="17d48-132">Response</span></span>

<span data-ttu-id="17d48-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[contact.personname](../resources/personname.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="17d48-133">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17d48-134">示例</span><span class="sxs-lookup"><span data-stu-id="17d48-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="17d48-135">请求</span><span class="sxs-lookup"><span data-stu-id="17d48-135">Request</span></span>

<span data-ttu-id="17d48-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17d48-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17d48-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="17d48-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names
```
# <a name="c"></a>[<span data-ttu-id="17d48-138">C#</span><span class="sxs-lookup"><span data-stu-id="17d48-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17d48-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17d48-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17d48-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17d48-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17d48-141">响应</span><span class="sxs-lookup"><span data-stu-id="17d48-141">Response</span></span>

<span data-ttu-id="17d48-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17d48-142">The following is an example of the response.</span></span>

> <span data-ttu-id="17d48-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="17d48-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "first": "first-value",
      "initials": "initials-value",
      "last": "last-value",
      "languageTag": "languageTag-value",
      "maiden": "maiden-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
