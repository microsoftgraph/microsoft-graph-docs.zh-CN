---
title: 创建 itemPhone
description: 使用此 API 创建新的 itemPhone。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 54fb9ff1453573fbf8c2904d581f54790093dfa6
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229316"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="31e44-103">创建 itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="31e44-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="31e44-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31e44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31e44-105">使用此 API 创建新的[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31e44-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31e44-106">权限</span><span class="sxs-lookup"><span data-stu-id="31e44-106">Permissions</span></span>

<span data-ttu-id="31e44-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31e44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31e44-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31e44-109">Permission type</span></span>                        | <span data-ttu-id="31e44-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31e44-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31e44-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31e44-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="31e44-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="31e44-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="31e44-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31e44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31e44-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="31e44-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="31e44-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31e44-115">Application</span></span>                            | <span data-ttu-id="31e44-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e44-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="31e44-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31e44-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="31e44-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="31e44-118">Request headers</span></span>

| <span data-ttu-id="31e44-119">名称</span><span class="sxs-lookup"><span data-stu-id="31e44-119">Name</span></span>           | <span data-ttu-id="31e44-120">说明</span><span class="sxs-lookup"><span data-stu-id="31e44-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="31e44-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31e44-121">Authorization</span></span>  | <span data-ttu-id="31e44-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31e44-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="31e44-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31e44-124">Content-Type</span></span>   | <span data-ttu-id="31e44-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="31e44-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31e44-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31e44-127">Request body</span></span>

<span data-ttu-id="31e44-128">在请求正文中，提供[itemPhone](../resources/itemphone.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31e44-128">In the request body, supply a JSON representation of [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="31e44-129">响应</span><span class="sxs-lookup"><span data-stu-id="31e44-129">Response</span></span>

<span data-ttu-id="31e44-130">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31e44-130">If successful, this method returns `201, Created` response code and a new [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31e44-131">示例</span><span class="sxs-lookup"><span data-stu-id="31e44-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31e44-132">请求</span><span class="sxs-lookup"><span data-stu-id="31e44-132">Request</span></span>

<span data-ttu-id="31e44-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31e44-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31e44-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="31e44-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemphone_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/phones
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```
# <a name="c"></a>[<span data-ttu-id="31e44-135">C#</span><span class="sxs-lookup"><span data-stu-id="31e44-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31e44-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31e44-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31e44-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31e44-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31e44-138">响应</span><span class="sxs-lookup"><span data-stu-id="31e44-138">Response</span></span>

<span data-ttu-id="31e44-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="31e44-139">The following is an example of the response.</span></span>

> <span data-ttu-id="31e44-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="31e44-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
