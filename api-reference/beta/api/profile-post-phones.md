---
title: 创建 itemPhone
description: 使用此 API 创建新的 itemPhone。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 07d19b6c773f1b92a295f0c1e3471942dda45696
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996525"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="ee611-103">创建 itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ee611-103">Create itemPhoneNumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee611-104">使用此 API 创建新的[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ee611-104">Use this API to create a new [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee611-105">权限</span><span class="sxs-lookup"><span data-stu-id="ee611-105">Permissions</span></span>

<span data-ttu-id="ee611-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee611-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee611-108">Permission type</span></span>                        | <span data-ttu-id="ee611-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee611-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ee611-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee611-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee611-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="ee611-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ee611-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee611-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee611-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="ee611-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ee611-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee611-114">Application</span></span>                            | <span data-ttu-id="ee611-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee611-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee611-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee611-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="ee611-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee611-117">Request headers</span></span>

| <span data-ttu-id="ee611-118">名称</span><span class="sxs-lookup"><span data-stu-id="ee611-118">Name</span></span>      |<span data-ttu-id="ee611-119">说明</span><span class="sxs-lookup"><span data-stu-id="ee611-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee611-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee611-120">Authorization</span></span>  | <span data-ttu-id="ee611-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee611-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ee611-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee611-123">Content-Type</span></span>   | <span data-ttu-id="ee611-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ee611-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee611-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee611-126">Request body</span></span>

<span data-ttu-id="ee611-127">在请求正文中，提供[itemPhone](../resources/itemphone.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee611-127">In the request body, supply a JSON representation of [itemPhone](../resources/itemphone.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ee611-128">响应</span><span class="sxs-lookup"><span data-stu-id="ee611-128">Response</span></span>

<span data-ttu-id="ee611-129">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ee611-129">If successful, this method returns `201, Created` response code and a new [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee611-130">示例</span><span class="sxs-lookup"><span data-stu-id="ee611-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee611-131">请求</span><span class="sxs-lookup"><span data-stu-id="ee611-131">Request</span></span>

<span data-ttu-id="ee611-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ee611-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ee611-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee611-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee611-134">C#</span><span class="sxs-lookup"><span data-stu-id="ee611-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itemphone-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee611-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee611-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itemphone-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee611-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee611-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itemphone-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee611-137">响应</span><span class="sxs-lookup"><span data-stu-id="ee611-137">Response</span></span>

<span data-ttu-id="ee611-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ee611-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ee611-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ee611-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
