---
title: 删除程序
description: 在 Azure AD 访问评审功能中，删除程序对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: a80b84aa0835fe0c8fa3e21cf1f8da37e851b394
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440986"
---
# <a name="delete-program"></a><span data-ttu-id="a9f7d-103">删除程序</span><span class="sxs-lookup"><span data-stu-id="a9f7d-103">Delete program</span></span>

<span data-ttu-id="a9f7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9f7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9f7d-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，删除 [程序](../resources/program.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="a9f7d-106">不要删除仍链接到该程序的程序，应首先从该程序中删除或取消链接这些访问评审，并链接到 `programControl` 其他程序。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-106">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="a9f7d-107">此外，请注意，无法删除内置默认程序。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-107">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="a9f7d-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="a9f7d-108">Permissions</span></span>
<span data-ttu-id="a9f7d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9f7d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9f7d-111">Permission type</span></span>                        | <span data-ttu-id="a9f7d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9f7d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9f7d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9f7d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9f7d-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f7d-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="a9f7d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9f7d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9f7d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-116">Not supported.</span></span> |
|<span data-ttu-id="a9f7d-117">Application</span><span class="sxs-lookup"><span data-stu-id="a9f7d-117">Application</span></span>                            | <span data-ttu-id="a9f7d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-118">Not supported.</span></span> |

<span data-ttu-id="a9f7d-119">登录用户还必须具有允许其创建程序的目录角色。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-119">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="a9f7d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9f7d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a9f7d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9f7d-121">Request headers</span></span>
| <span data-ttu-id="a9f7d-122">名称</span><span class="sxs-lookup"><span data-stu-id="a9f7d-122">Name</span></span>         | <span data-ttu-id="a9f7d-123">类型</span><span class="sxs-lookup"><span data-stu-id="a9f7d-123">Type</span></span>        | <span data-ttu-id="a9f7d-124">说明</span><span class="sxs-lookup"><span data-stu-id="a9f7d-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a9f7d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9f7d-125">Authorization</span></span> | <span data-ttu-id="a9f7d-126">string</span><span class="sxs-lookup"><span data-stu-id="a9f7d-126">string</span></span> | <span data-ttu-id="a9f7d-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9f7d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9f7d-129">Request body</span></span>
<span data-ttu-id="a9f7d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a9f7d-131">响应</span><span class="sxs-lookup"><span data-stu-id="a9f7d-131">Response</span></span>
<span data-ttu-id="a9f7d-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f7d-134">示例</span><span class="sxs-lookup"><span data-stu-id="a9f7d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9f7d-135">请求</span><span class="sxs-lookup"><span data-stu-id="a9f7d-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a9f7d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9f7d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="a9f7d-137">C#</span><span class="sxs-lookup"><span data-stu-id="a9f7d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9f7d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9f7d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9f7d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9f7d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9f7d-140">Java</span><span class="sxs-lookup"><span data-stu-id="a9f7d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9f7d-141">响应</span><span class="sxs-lookup"><span data-stu-id="a9f7d-141">Response</span></span>
><span data-ttu-id="a9f7d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a9f7d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


