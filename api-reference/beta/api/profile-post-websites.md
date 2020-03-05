---
title: 创建 personWebsite
description: 创建新的 personWebsite。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9fee97962e998a010dd4bbf57b9a9e9c4a766296
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455058"
---
# <a name="create-personwebsite"></a><span data-ttu-id="25c85-103">创建 personWebsite</span><span class="sxs-lookup"><span data-stu-id="25c85-103">Create personWebsite</span></span>

<span data-ttu-id="25c85-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="25c85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25c85-105">在用户的[配置文件](../resources/profile.md)中创建新的[personWebsite](../resources/personwebsite.md)对象。</span><span class="sxs-lookup"><span data-stu-id="25c85-105">Create a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25c85-106">权限</span><span class="sxs-lookup"><span data-stu-id="25c85-106">Permissions</span></span>

<span data-ttu-id="25c85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25c85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25c85-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="25c85-109">Permission type</span></span>                        | <span data-ttu-id="25c85-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25c85-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="25c85-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25c85-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25c85-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="25c85-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="25c85-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25c85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25c85-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="25c85-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="25c85-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="25c85-115">Application</span></span>                            | <span data-ttu-id="25c85-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c85-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25c85-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25c85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/websites
```

## <a name="request-headers"></a><span data-ttu-id="25c85-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="25c85-118">Request headers</span></span>

| <span data-ttu-id="25c85-119">名称</span><span class="sxs-lookup"><span data-stu-id="25c85-119">Name</span></span>      |<span data-ttu-id="25c85-120">说明</span><span class="sxs-lookup"><span data-stu-id="25c85-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25c85-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25c85-121">Authorization</span></span>  | <span data-ttu-id="25c85-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25c85-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="25c85-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25c85-124">Content-Type</span></span>   | <span data-ttu-id="25c85-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="25c85-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25c85-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="25c85-127">Request body</span></span>

<span data-ttu-id="25c85-128">在请求正文中，提供[personWebsite](../resources/personwebsite.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25c85-128">In the request body, supply a JSON representation of [personWebsite](../resources/personwebsite.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="25c85-129">响应</span><span class="sxs-lookup"><span data-stu-id="25c85-129">Response</span></span>

<span data-ttu-id="25c85-130">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[personWebsite](../resources/personwebsite.md)对象。</span><span class="sxs-lookup"><span data-stu-id="25c85-130">If successful, this method returns `201, Created` response code and a new [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25c85-131">示例</span><span class="sxs-lookup"><span data-stu-id="25c85-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25c85-132">请求</span><span class="sxs-lookup"><span data-stu-id="25c85-132">Request</span></span>

<span data-ttu-id="25c85-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25c85-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25c85-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="25c85-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personwebsite_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/websites
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
# <a name="c"></a>[<span data-ttu-id="25c85-135">C#</span><span class="sxs-lookup"><span data-stu-id="25c85-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personwebsite-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25c85-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25c85-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personwebsite-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25c85-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25c85-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personwebsite-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25c85-138">响应</span><span class="sxs-lookup"><span data-stu-id="25c85-138">Response</span></span>

<span data-ttu-id="25c85-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25c85-139">The following is an example of the response.</span></span>

> <span data-ttu-id="25c85-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="25c85-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
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
  "description": "Create personWebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
