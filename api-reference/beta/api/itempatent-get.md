---
title: 获取 itemPatent
description: 读取 itemPatent 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7e0dafa14ed5cbb94e48884b54c9300a36cfc456
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969918"
---
# <a name="get-itempatent"></a><span data-ttu-id="5ca9c-103">获取 itemPatent</span><span class="sxs-lookup"><span data-stu-id="5ca9c-103">Get itemPatent</span></span>

<span data-ttu-id="5ca9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ca9c-105">读取 [itemPatent](../resources/itempatent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-105">Read the properties and relationships of an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ca9c-106">Permissions</span></span>

<span data-ttu-id="5ca9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ca9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ca9c-109">Permission type</span></span>                        | <span data-ttu-id="5ca9c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ca9c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5ca9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ca9c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ca9c-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="5ca9c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5ca9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ca9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ca9c-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="5ca9c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5ca9c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ca9c-115">Application</span></span>                            | <span data-ttu-id="5ca9c-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="5ca9c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="5ca9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ca9c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/patents/{id}
GET /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ca9c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5ca9c-118">Optional query parameters</span></span>

<span data-ttu-id="5ca9c-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="5ca9c-120">指定要包含在响应中的属性的列表，并以逗号分隔。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="5ca9c-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ca9c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ca9c-122">Request headers</span></span>
|<span data-ttu-id="5ca9c-123">名称</span><span class="sxs-lookup"><span data-stu-id="5ca9c-123">Name</span></span>|<span data-ttu-id="5ca9c-124">说明</span><span class="sxs-lookup"><span data-stu-id="5ca9c-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ca9c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ca9c-125">Authorization</span></span>|<span data-ttu-id="5ca9c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ca9c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ca9c-128">Request body</span></span>
<span data-ttu-id="5ca9c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca9c-130">响应</span><span class="sxs-lookup"><span data-stu-id="5ca9c-130">Response</span></span>

<span data-ttu-id="5ca9c-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [itemPatent](../resources/itempatent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-131">If successful, this method returns a `200 OK` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ca9c-132">示例</span><span class="sxs-lookup"><span data-stu-id="5ca9c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ca9c-133">请求</span><span class="sxs-lookup"><span data-stu-id="5ca9c-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="5ca9c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca9c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itempatent"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="5ca9c-135">C#</span><span class="sxs-lookup"><span data-stu-id="5ca9c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itempatent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ca9c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ca9c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itempatent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ca9c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ca9c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itempatent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ca9c-138">Java</span><span class="sxs-lookup"><span data-stu-id="5ca9c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-itempatent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5ca9c-139">响应</span><span class="sxs-lookup"><span data-stu-id="5ca9c-139">Response</span></span>

<span data-ttu-id="5ca9c-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5ca9c-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```


