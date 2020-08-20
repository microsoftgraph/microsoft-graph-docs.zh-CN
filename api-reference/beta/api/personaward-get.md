---
title: 获取 personAward
description: 读取 personAward 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 738df8ce9d922d5a7f06cb834239368682f02546
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820163"
---
# <a name="get-personaward"></a><span data-ttu-id="f6c26-103">获取 personAward</span><span class="sxs-lookup"><span data-stu-id="f6c26-103">Get personAward</span></span>

<span data-ttu-id="f6c26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6c26-105">从用户的配置文件中 [读取 personAward](../resources/personaward.md) 对象的属性和 [关系](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="f6c26-105">Read the properties and relationships of a [personAward](../resources/personaward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c26-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6c26-106">Permissions</span></span>

<span data-ttu-id="f6c26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6c26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6c26-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6c26-109">Permission type</span></span>                        | <span data-ttu-id="f6c26-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6c26-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f6c26-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c26-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6c26-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c26-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f6c26-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c26-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c26-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f6c26-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6c26-115">Application</span></span>                            | <span data-ttu-id="f6c26-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c26-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f6c26-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6c26-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/awards/{id}
GET /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6c26-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f6c26-118">Optional query parameters</span></span>

<span data-ttu-id="f6c26-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="f6c26-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="f6c26-120">指定要在响应中包含的属性列表，并用逗号将它们分开。</span><span class="sxs-lookup"><span data-stu-id="f6c26-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="f6c26-121">为了获得最佳性能，请仅选择需要的属性子集。</span><span class="sxs-lookup"><span data-stu-id="f6c26-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6c26-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6c26-122">Request headers</span></span>
|<span data-ttu-id="f6c26-123">名称</span><span class="sxs-lookup"><span data-stu-id="f6c26-123">Name</span></span>|<span data-ttu-id="f6c26-124">说明</span><span class="sxs-lookup"><span data-stu-id="f6c26-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6c26-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c26-125">Authorization</span></span>|<span data-ttu-id="f6c26-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6c26-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6c26-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6c26-128">Request body</span></span>
<span data-ttu-id="f6c26-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6c26-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6c26-130">响应</span><span class="sxs-lookup"><span data-stu-id="f6c26-130">Response</span></span>

<span data-ttu-id="f6c26-131">如果成功，此方法在响应 `200 OK` 正文中返回响应代码 [和 personAward](../resources/personaward.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6c26-131">If successful, this method returns a `200 OK` response code and an [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6c26-132">示例</span><span class="sxs-lookup"><span data-stu-id="f6c26-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6c26-133">请求</span><span class="sxs-lookup"><span data-stu-id="f6c26-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="f6c26-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6c26-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personAward"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/awards/{id}
```
# <a name="c"></a>[<span data-ttu-id="f6c26-135">C#</span><span class="sxs-lookup"><span data-stu-id="f6c26-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personaward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6c26-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6c26-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personaward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6c26-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6c26-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personaward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f6c26-138">响应</span><span class="sxs-lookup"><span data-stu-id="f6c26-138">Response</span></span>

<span data-ttu-id="f6c26-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f6c26-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
```
