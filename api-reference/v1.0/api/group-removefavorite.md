---
title: 'group: removeFavorite'
description: 从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 87a57d1f97ba35146c4a3c787e50c09dc6979747
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516954"
---
# <a name="group-removefavorite"></a><span data-ttu-id="edc2e-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="edc2e-104">group: removeFavorite</span></span>

<span data-ttu-id="edc2e-105">命名空间： microsoft. graph 从当前用户的收藏夹组列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="edc2e-105">Namespace: microsoft.graph Remove the group from the list of the current user's favorite groups.</span></span> <span data-ttu-id="edc2e-106">仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="edc2e-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="edc2e-107">权限</span><span class="sxs-lookup"><span data-stu-id="edc2e-107">Permissions</span></span>
<span data-ttu-id="edc2e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edc2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edc2e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="edc2e-110">Permission type</span></span>      | <span data-ttu-id="edc2e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edc2e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edc2e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edc2e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="edc2e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc2e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="edc2e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edc2e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edc2e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc2e-115">Not supported.</span></span>    |
|<span data-ttu-id="edc2e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="edc2e-116">Application</span></span> | <span data-ttu-id="edc2e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc2e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="edc2e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edc2e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="edc2e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="edc2e-119">Request headers</span></span>
| <span data-ttu-id="edc2e-120">标头</span><span class="sxs-lookup"><span data-stu-id="edc2e-120">Header</span></span>       | <span data-ttu-id="edc2e-121">值</span><span class="sxs-lookup"><span data-stu-id="edc2e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="edc2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="edc2e-122">Authorization</span></span>  | <span data-ttu-id="edc2e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edc2e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="edc2e-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="edc2e-125">Prefer</span></span> | <span data-ttu-id="edc2e-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="edc2e-126">return=minimal.</span></span> <span data-ttu-id="edc2e-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="edc2e-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="edc2e-128">可选。</span><span class="sxs-lookup"><span data-stu-id="edc2e-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="edc2e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="edc2e-129">Request body</span></span>
<span data-ttu-id="edc2e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="edc2e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edc2e-131">响应</span><span class="sxs-lookup"><span data-stu-id="edc2e-131">Response</span></span>
<span data-ttu-id="edc2e-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="edc2e-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edc2e-134">示例</span><span class="sxs-lookup"><span data-stu-id="edc2e-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="edc2e-135">请求</span><span class="sxs-lookup"><span data-stu-id="edc2e-135">Request</span></span>
<span data-ttu-id="edc2e-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="edc2e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="edc2e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="edc2e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```
# <a name="c"></a>[<span data-ttu-id="edc2e-138">C#</span><span class="sxs-lookup"><span data-stu-id="edc2e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edc2e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edc2e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edc2e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edc2e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edc2e-141">Java</span><span class="sxs-lookup"><span data-stu-id="edc2e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removefavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="edc2e-142">响应</span><span class="sxs-lookup"><span data-stu-id="edc2e-142">Response</span></span>
<span data-ttu-id="edc2e-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="edc2e-143">The following is an example of the response.</span></span>
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
