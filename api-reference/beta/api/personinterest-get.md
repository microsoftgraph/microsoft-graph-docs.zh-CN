---
title: 获取 personInterest
description: 检索 personInterest 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 405b6068d85349d8f17bb2491e4aace8fa3b2d08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986285"
---
# <a name="get-personinterest"></a><span data-ttu-id="148ff-103">获取 personInterest</span><span class="sxs-lookup"><span data-stu-id="148ff-103">Get personInterest</span></span>

<span data-ttu-id="148ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="148ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="148ff-105">在用户的[配置文件](../resources/profile.md)中检索[personInterest](../resources/personinterest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="148ff-105">Retrieve the properties and relationships of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="148ff-106">权限</span><span class="sxs-lookup"><span data-stu-id="148ff-106">Permissions</span></span>

<span data-ttu-id="148ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="148ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="148ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="148ff-109">Permission type</span></span>                        | <span data-ttu-id="148ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="148ff-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="148ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="148ff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="148ff-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="148ff-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="148ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="148ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="148ff-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="148ff-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="148ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="148ff-115">Application</span></span>                            | <span data-ttu-id="148ff-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="148ff-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="148ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="148ff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests/{id}
GET /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="148ff-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="148ff-118">Optional query parameters</span></span>

<span data-ttu-id="148ff-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="148ff-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="148ff-120">指定要包含在响应中的属性的列表，并以逗号分隔。</span><span class="sxs-lookup"><span data-stu-id="148ff-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="148ff-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="148ff-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="148ff-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="148ff-122">Request headers</span></span>

| <span data-ttu-id="148ff-123">名称</span><span class="sxs-lookup"><span data-stu-id="148ff-123">Name</span></span>           |<span data-ttu-id="148ff-124">说明</span><span class="sxs-lookup"><span data-stu-id="148ff-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="148ff-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="148ff-125">Authorization</span></span>  | <span data-ttu-id="148ff-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="148ff-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="148ff-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="148ff-128">Request body</span></span>

<span data-ttu-id="148ff-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="148ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="148ff-130">响应</span><span class="sxs-lookup"><span data-stu-id="148ff-130">Response</span></span>

<span data-ttu-id="148ff-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [personInterest](../resources/personinterest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="148ff-131">If successful, this method returns a `200 OK` response code and the requested [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="148ff-132">示例</span><span class="sxs-lookup"><span data-stu-id="148ff-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="148ff-133">请求</span><span class="sxs-lookup"><span data-stu-id="148ff-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="148ff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="148ff-134">HTTP</span></span>](#tab/http)

<span data-ttu-id="148ff-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="148ff-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_personinterest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="148ff-136">C#</span><span class="sxs-lookup"><span data-stu-id="148ff-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="148ff-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="148ff-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="148ff-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="148ff-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="148ff-139">响应</span><span class="sxs-lookup"><span data-stu-id="148ff-139">Response</span></span>

<span data-ttu-id="148ff-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="148ff-140">The following is an example of the response.</span></span>

> <span data-ttu-id="148ff-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="148ff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


