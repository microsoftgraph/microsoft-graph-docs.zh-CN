---
title: 获取 personInterest
description: 检索 personInterest 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9d26dd248a10ba809e7c5a82c0abba9c57c7a1a2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819631"
---
# <a name="get-personinterest"></a><span data-ttu-id="18baf-103">获取 personInterest</span><span class="sxs-lookup"><span data-stu-id="18baf-103">Get personInterest</span></span>

<span data-ttu-id="18baf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18baf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18baf-105">在用户的配置文件中检索 [personInterest](../resources/personinterest.md) 对象的属性和 [关系](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="18baf-105">Retrieve the properties and relationships of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18baf-106">权限</span><span class="sxs-lookup"><span data-stu-id="18baf-106">Permissions</span></span>

<span data-ttu-id="18baf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18baf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18baf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18baf-109">Permission type</span></span>                        | <span data-ttu-id="18baf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18baf-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="18baf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18baf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18baf-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18baf-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="18baf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18baf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18baf-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18baf-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="18baf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18baf-115">Application</span></span>                            | <span data-ttu-id="18baf-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18baf-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="18baf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18baf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests/{id}
GET /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18baf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="18baf-118">Optional query parameters</span></span>

<span data-ttu-id="18baf-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="18baf-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="18baf-120">指定要在响应中包含的属性列表，并用逗号将它们分开。</span><span class="sxs-lookup"><span data-stu-id="18baf-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="18baf-121">为了获得最佳性能，请仅选择需要的属性子集。</span><span class="sxs-lookup"><span data-stu-id="18baf-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18baf-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="18baf-122">Request headers</span></span>

| <span data-ttu-id="18baf-123">名称</span><span class="sxs-lookup"><span data-stu-id="18baf-123">Name</span></span>           |<span data-ttu-id="18baf-124">说明</span><span class="sxs-lookup"><span data-stu-id="18baf-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="18baf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18baf-125">Authorization</span></span>  | <span data-ttu-id="18baf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18baf-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="18baf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="18baf-128">Request body</span></span>

<span data-ttu-id="18baf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18baf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18baf-130">响应</span><span class="sxs-lookup"><span data-stu-id="18baf-130">Response</span></span>

<span data-ttu-id="18baf-131">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [请求的 personInterest](../resources/personinterest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18baf-131">If successful, this method returns a `200 OK` response code and the requested [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18baf-132">示例</span><span class="sxs-lookup"><span data-stu-id="18baf-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18baf-133">请求</span><span class="sxs-lookup"><span data-stu-id="18baf-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="18baf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="18baf-134">HTTP</span></span>](#tab/http)

<span data-ttu-id="18baf-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="18baf-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_personinterest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="18baf-136">C#</span><span class="sxs-lookup"><span data-stu-id="18baf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18baf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18baf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18baf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18baf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="18baf-139">响应</span><span class="sxs-lookup"><span data-stu-id="18baf-139">Response</span></span>

<span data-ttu-id="18baf-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="18baf-140">The following is an example of the response.</span></span>

> <span data-ttu-id="18baf-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18baf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
