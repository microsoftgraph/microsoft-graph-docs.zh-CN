---
title: 创建 personInterest
description: 创建新的 personInterest。
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: 390526786ae6761259ae6a83cec987dbcf74d6db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455100"
---
# <a name="create-personinterest"></a><span data-ttu-id="e5547-103">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="e5547-103">Create personInterest</span></span>

<span data-ttu-id="e5547-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e5547-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5547-105">创建新的 [personInterest] （.。。/resources/personinterest.md].</span><span class="sxs-lookup"><span data-stu-id="e5547-105">Create a new [personInterest](../resources/personinterest.md].</span></span>

## <a name="permissions"></a><span data-ttu-id="e5547-106">权限</span><span class="sxs-lookup"><span data-stu-id="e5547-106">Permissions</span></span>

<span data-ttu-id="e5547-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5547-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5547-109">Permission type</span></span>                        | <span data-ttu-id="e5547-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5547-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5547-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5547-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5547-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e5547-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e5547-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5547-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5547-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e5547-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e5547-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5547-115">Application</span></span>                            | <span data-ttu-id="e5547-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5547-116">User.ReadWrite.All</span></span> |
## <a name="http-request"></a><span data-ttu-id="e5547-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5547-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="e5547-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5547-118">Request headers</span></span>

| <span data-ttu-id="e5547-119">名称</span><span class="sxs-lookup"><span data-stu-id="e5547-119">Name</span></span>      |<span data-ttu-id="e5547-120">说明</span><span class="sxs-lookup"><span data-stu-id="e5547-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5547-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5547-121">Authorization</span></span>  | <span data-ttu-id="e5547-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5547-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e5547-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5547-124">Content-Type</span></span>   | <span data-ttu-id="e5547-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5547-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5547-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5547-127">Request body</span></span>

<span data-ttu-id="e5547-128">在请求正文中，提供[personInterest](../resources/personinterest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5547-128">In the request body, supply a JSON representation of [personInterest](../resources/personinterest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e5547-129">响应</span><span class="sxs-lookup"><span data-stu-id="e5547-129">Response</span></span>

<span data-ttu-id="e5547-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[personInterest](../resources/personinterest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5547-130">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5547-131">示例</span><span class="sxs-lookup"><span data-stu-id="e5547-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5547-132">请求</span><span class="sxs-lookup"><span data-stu-id="e5547-132">Request</span></span>

<span data-ttu-id="e5547-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5547-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5547-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5547-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e5547-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5547-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5547-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5547-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5547-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5547-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5547-138">响应</span><span class="sxs-lookup"><span data-stu-id="e5547-138">Response</span></span>

<span data-ttu-id="e5547-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5547-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e5547-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5547-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personInterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
