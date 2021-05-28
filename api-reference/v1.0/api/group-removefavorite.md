---
title: 'group: removeFavorite'
description: 从当前用户收藏夹组列表中删除组。 仅支持 Microsoft 365 组。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 526272a7c4252a23914b222ce15691b98bdf9de4
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682073"
---
# <a name="group-removefavorite"></a><span data-ttu-id="5c19f-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="5c19f-104">group: removeFavorite</span></span>

<span data-ttu-id="5c19f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c19f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c19f-106">从当前用户收藏夹组列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="5c19f-106">Remove the group from the list of the current user's favorite groups.</span></span> <span data-ttu-id="5c19f-107">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="5c19f-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c19f-108">权限</span><span class="sxs-lookup"><span data-stu-id="5c19f-108">Permissions</span></span>
<span data-ttu-id="5c19f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c19f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c19f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c19f-111">Permission type</span></span>      | <span data-ttu-id="5c19f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c19f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c19f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c19f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5c19f-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c19f-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c19f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c19f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c19f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c19f-116">Not supported.</span></span>    |
|<span data-ttu-id="5c19f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c19f-117">Application</span></span> | <span data-ttu-id="5c19f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c19f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c19f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c19f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="5c19f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c19f-120">Request headers</span></span>
| <span data-ttu-id="5c19f-121">标头</span><span class="sxs-lookup"><span data-stu-id="5c19f-121">Header</span></span>       | <span data-ttu-id="5c19f-122">值</span><span class="sxs-lookup"><span data-stu-id="5c19f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c19f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c19f-123">Authorization</span></span>  | <span data-ttu-id="5c19f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c19f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5c19f-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="5c19f-126">Prefer</span></span> | <span data-ttu-id="5c19f-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="5c19f-127">return=minimal.</span></span> <span data-ttu-id="5c19f-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="5c19f-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="5c19f-129">可选。</span><span class="sxs-lookup"><span data-stu-id="5c19f-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="5c19f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c19f-130">Request body</span></span>
<span data-ttu-id="5c19f-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c19f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c19f-132">响应</span><span class="sxs-lookup"><span data-stu-id="5c19f-132">Response</span></span>
<span data-ttu-id="5c19f-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5c19f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c19f-135">示例</span><span class="sxs-lookup"><span data-stu-id="5c19f-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5c19f-136">请求</span><span class="sxs-lookup"><span data-stu-id="5c19f-136">Request</span></span>
<span data-ttu-id="5c19f-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c19f-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c19f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c19f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```
# <a name="c"></a>[<span data-ttu-id="5c19f-139">C#</span><span class="sxs-lookup"><span data-stu-id="5c19f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c19f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c19f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c19f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c19f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c19f-142">Java</span><span class="sxs-lookup"><span data-stu-id="5c19f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removefavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5c19f-143">响应</span><span class="sxs-lookup"><span data-stu-id="5c19f-143">Response</span></span>
<span data-ttu-id="5c19f-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c19f-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

