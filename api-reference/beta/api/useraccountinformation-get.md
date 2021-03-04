---
title: 获取 userAccountInformation
description: 检索 userAccountInformation 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: ec6b24daf3b2314e8175a7456f3187f2ac67178c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443302"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="994c6-103">获取 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="994c6-103">Get userAccountInformation</span></span>

<span data-ttu-id="994c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="994c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="994c6-105">检索用户配置文件中的 [userAccountInformation](../resources/useraccountinformation.md) 对象的属性和 [关系](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="994c6-105">Retrieve the properties and relationships of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="994c6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="994c6-106">Permissions</span></span>

<span data-ttu-id="994c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="994c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="994c6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="994c6-109">Permission type</span></span>                        | <span data-ttu-id="994c6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="994c6-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="994c6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="994c6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="994c6-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994c6-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="994c6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="994c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="994c6-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994c6-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="994c6-115">Application</span><span class="sxs-lookup"><span data-stu-id="994c6-115">Application</span></span>                            | <span data-ttu-id="994c6-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="994c6-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="994c6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="994c6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account/{id}
GET /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="994c6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="994c6-118">Optional query parameters</span></span>

<span data-ttu-id="994c6-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="994c6-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="994c6-120">指定要包括在响应中的属性列表，用逗号分隔它们。</span><span class="sxs-lookup"><span data-stu-id="994c6-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="994c6-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="994c6-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="994c6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="994c6-122">Request headers</span></span>

| <span data-ttu-id="994c6-123">名称</span><span class="sxs-lookup"><span data-stu-id="994c6-123">Name</span></span>          |<span data-ttu-id="994c6-124">说明</span><span class="sxs-lookup"><span data-stu-id="994c6-124">Description</span></span>                |
|:--------------|:--------------------------|
| <span data-ttu-id="994c6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="994c6-125">Authorization</span></span> | <span data-ttu-id="994c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="994c6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="994c6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="994c6-128">Request body</span></span>

<span data-ttu-id="994c6-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="994c6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="994c6-130">响应</span><span class="sxs-lookup"><span data-stu-id="994c6-130">Response</span></span>

<span data-ttu-id="994c6-131">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [userAccountInformation](../resources/useraccountinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="994c6-131">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="994c6-132">示例</span><span class="sxs-lookup"><span data-stu-id="994c6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="994c6-133">请求</span><span class="sxs-lookup"><span data-stu-id="994c6-133">Request</span></span>

<span data-ttu-id="994c6-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="994c6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="994c6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="994c6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account/{id}
```
# <a name="c"></a>[<span data-ttu-id="994c6-136">C#</span><span class="sxs-lookup"><span data-stu-id="994c6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="994c6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="994c6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="994c6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="994c6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="994c6-139">Java</span><span class="sxs-lookup"><span data-stu-id="994c6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="994c6-140">响应</span><span class="sxs-lookup"><span data-stu-id="994c6-140">Response</span></span>

<span data-ttu-id="994c6-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="994c6-141">The following is an example of the response.</span></span>

> <span data-ttu-id="994c6-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="994c6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
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
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


