---
title: 删除程序
description: 在 "Azure AD access 评论" 功能中，删除一个程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c7c6fd7ca637d977fe007dc1adc4ed31af08aa69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454995"
---
# <a name="delete-program"></a><span data-ttu-id="22435-103">删除程序</span><span class="sxs-lookup"><span data-stu-id="22435-103">Delete program</span></span>

<span data-ttu-id="22435-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="22435-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22435-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中，删除一个[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="22435-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="22435-106">请勿删除仍与它`programControl`链接的程序，应首先从该程序中删除或取消这些访问审核，并将其链接到其他程序。</span><span class="sxs-lookup"><span data-stu-id="22435-106">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="22435-107">此外，请注意，不能删除内置的默认程序。</span><span class="sxs-lookup"><span data-stu-id="22435-107">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="22435-108">权限</span><span class="sxs-lookup"><span data-stu-id="22435-108">Permissions</span></span>
<span data-ttu-id="22435-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22435-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22435-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="22435-111">Permission type</span></span>                        | <span data-ttu-id="22435-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22435-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="22435-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22435-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="22435-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22435-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="22435-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22435-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22435-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22435-116">Not supported.</span></span> |
|<span data-ttu-id="22435-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="22435-117">Application</span></span>                            | <span data-ttu-id="22435-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="22435-118">Not supported.</span></span> |

<span data-ttu-id="22435-119">登录用户还必须位于允许他们创建程序的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="22435-119">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="22435-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22435-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="22435-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="22435-121">Request headers</span></span>
| <span data-ttu-id="22435-122">名称</span><span class="sxs-lookup"><span data-stu-id="22435-122">Name</span></span>         | <span data-ttu-id="22435-123">类型</span><span class="sxs-lookup"><span data-stu-id="22435-123">Type</span></span>        | <span data-ttu-id="22435-124">说明</span><span class="sxs-lookup"><span data-stu-id="22435-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="22435-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="22435-125">Authorization</span></span> | <span data-ttu-id="22435-126">string</span><span class="sxs-lookup"><span data-stu-id="22435-126">string</span></span> | <span data-ttu-id="22435-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="22435-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22435-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="22435-129">Request body</span></span>
<span data-ttu-id="22435-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22435-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="22435-131">响应</span><span class="sxs-lookup"><span data-stu-id="22435-131">Response</span></span>
<span data-ttu-id="22435-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="22435-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22435-134">示例</span><span class="sxs-lookup"><span data-stu-id="22435-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22435-135">请求</span><span class="sxs-lookup"><span data-stu-id="22435-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="22435-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="22435-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="22435-137">C#</span><span class="sxs-lookup"><span data-stu-id="22435-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22435-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22435-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22435-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22435-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="22435-140">响应</span><span class="sxs-lookup"><span data-stu-id="22435-140">Response</span></span>
><span data-ttu-id="22435-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="22435-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
