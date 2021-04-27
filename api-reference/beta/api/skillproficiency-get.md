---
title: 获取 skillProficiency
description: 检索技能属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c6447e613b73555fa183c1be8a11701ca33a87b3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048993"
---
# <a name="get-skillproficiency"></a><span data-ttu-id="6d27d-103">获取 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="6d27d-103">Get skillProficiency</span></span>

<span data-ttu-id="6d27d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d27d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d27d-105">检索用户配置文件中的 [技能属性](../resources/skillproficiency.md) 和 [关系](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="6d27d-105">Retrieve the properties and relationships of a [skillproficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d27d-106">权限</span><span class="sxs-lookup"><span data-stu-id="6d27d-106">Permissions</span></span>

<span data-ttu-id="6d27d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d27d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d27d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d27d-109">Permission type</span></span>                        | <span data-ttu-id="6d27d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d27d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6d27d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d27d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d27d-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d27d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6d27d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d27d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d27d-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d27d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6d27d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d27d-115">Application</span></span>                            | <span data-ttu-id="6d27d-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d27d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="6d27d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d27d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills/{id}
GET /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d27d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d27d-118">Optional query parameters</span></span>

<span data-ttu-id="6d27d-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="6d27d-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="6d27d-120">指定要包括在响应中的属性列表，用逗号分隔它们。</span><span class="sxs-lookup"><span data-stu-id="6d27d-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="6d27d-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="6d27d-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d27d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d27d-122">Request headers</span></span>

| <span data-ttu-id="6d27d-123">名称</span><span class="sxs-lookup"><span data-stu-id="6d27d-123">Name</span></span>           | <span data-ttu-id="6d27d-124">说明</span><span class="sxs-lookup"><span data-stu-id="6d27d-124">Description</span></span>                  |
|:---------------|:-----------------------------|
| <span data-ttu-id="6d27d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d27d-125">Authorization</span></span>  | <span data-ttu-id="6d27d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d27d-p103">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="6d27d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d27d-128">Content-Type</span></span>   | <span data-ttu-id="6d27d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6d27d-p104">application/json. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="6d27d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d27d-131">Request body</span></span>

<span data-ttu-id="6d27d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d27d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d27d-133">响应</span><span class="sxs-lookup"><span data-stu-id="6d27d-133">Response</span></span>

<span data-ttu-id="6d27d-134">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [skillProficiency](../resources/skillproficiency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d27d-134">If successful, this method returns a `200 OK` response code and the requested [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d27d-135">示例</span><span class="sxs-lookup"><span data-stu-id="6d27d-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d27d-136">请求</span><span class="sxs-lookup"><span data-stu-id="6d27d-136">Request</span></span>

<span data-ttu-id="6d27d-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6d27d-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d27d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d27d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_skillproficiency"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/skills/{id}
```
# <a name="c"></a>[<span data-ttu-id="6d27d-139">C#</span><span class="sxs-lookup"><span data-stu-id="6d27d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d27d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d27d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d27d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d27d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d27d-142">Java</span><span class="sxs-lookup"><span data-stu-id="6d27d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-skillproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d27d-143">响应</span><span class="sxs-lookup"><span data-stu-id="6d27d-143">Response</span></span>

<span data-ttu-id="6d27d-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6d27d-144">The following is an example of the response.</span></span>

> <span data-ttu-id="6d27d-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6d27d-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
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
  "source": null,
  "categories": [
    "Professional"
  ],
  "displayName": "API Design",
  "proficiency": "advancedProfessional",
  "webUrl": null,
  "collaborationTags": [
    "ableToMentor"
  ]
}
```


