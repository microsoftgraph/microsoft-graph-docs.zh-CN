---
title: 删除 appRoleAssignment
description: 删除 appRoleAssignment。
localization_priority: Normal
ms.openlocfilehash: f8c282a3d33560e95dcb43384227a34e6bd8ccf4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636511"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="75474-103">删除 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75474-103">Delete appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75474-104">删除 appRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="75474-104">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="75474-105">权限</span><span class="sxs-lookup"><span data-stu-id="75474-105">Permissions</span></span>
<span data-ttu-id="75474-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75474-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="75474-108">Permission type</span></span>      | <span data-ttu-id="75474-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75474-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75474-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75474-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75474-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75474-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="75474-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75474-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75474-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="75474-113">Not supported.</span></span>    |
|<span data-ttu-id="75474-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="75474-114">Application</span></span> | <span data-ttu-id="75474-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75474-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75474-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75474-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="75474-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="75474-117">Request headers</span></span>
| <span data-ttu-id="75474-118">名称</span><span class="sxs-lookup"><span data-stu-id="75474-118">Name</span></span>       | <span data-ttu-id="75474-119">类型</span><span class="sxs-lookup"><span data-stu-id="75474-119">Type</span></span> | <span data-ttu-id="75474-120">说明</span><span class="sxs-lookup"><span data-stu-id="75474-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="75474-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="75474-121">Authorization</span></span>  | <span data-ttu-id="75474-122">string</span><span class="sxs-lookup"><span data-stu-id="75474-122">string</span></span>  | <span data-ttu-id="75474-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75474-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75474-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="75474-125">Request body</span></span>
<span data-ttu-id="75474-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75474-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75474-127">响应</span><span class="sxs-lookup"><span data-stu-id="75474-127">Response</span></span>

<span data-ttu-id="75474-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="75474-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75474-130">示例</span><span class="sxs-lookup"><span data-stu-id="75474-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75474-131">请求</span><span class="sxs-lookup"><span data-stu-id="75474-131">Request</span></span>
<span data-ttu-id="75474-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75474-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="75474-133">响应</span><span class="sxs-lookup"><span data-stu-id="75474-133">Response</span></span>
<span data-ttu-id="75474-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="75474-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="75474-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="75474-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="75474-136">语言</span><span class="sxs-lookup"><span data-stu-id="75474-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_approleassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75474-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="75474-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_approleassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/approleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
