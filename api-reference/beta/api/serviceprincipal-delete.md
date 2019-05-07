---
title: 删除 servicePrincipal
description: 删除 servicePrincipal。
localization_priority: Normal
ms.openlocfilehash: 224ebf07dbe569add6f8a47d08d0be6f4d53e379
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638828"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="be1f5-103">删除 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="be1f5-103">Delete servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be1f5-104">删除 servicePrincipal。</span><span class="sxs-lookup"><span data-stu-id="be1f5-104">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="be1f5-105">权限</span><span class="sxs-lookup"><span data-stu-id="be1f5-105">Permissions</span></span>
<span data-ttu-id="be1f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be1f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be1f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="be1f5-108">Permission type</span></span>      | <span data-ttu-id="be1f5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be1f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be1f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be1f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be1f5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="be1f5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="be1f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be1f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be1f5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="be1f5-113">Not supported.</span></span>    |
|<span data-ttu-id="be1f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="be1f5-114">Application</span></span> | <span data-ttu-id="be1f5-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="be1f5-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be1f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be1f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="be1f5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="be1f5-117">Request headers</span></span>
| <span data-ttu-id="be1f5-118">名称</span><span class="sxs-lookup"><span data-stu-id="be1f5-118">Name</span></span>       | <span data-ttu-id="be1f5-119">类型</span><span class="sxs-lookup"><span data-stu-id="be1f5-119">Type</span></span> | <span data-ttu-id="be1f5-120">说明</span><span class="sxs-lookup"><span data-stu-id="be1f5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="be1f5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be1f5-121">Authorization</span></span>  | <span data-ttu-id="be1f5-122">string</span><span class="sxs-lookup"><span data-stu-id="be1f5-122">string</span></span>  | <span data-ttu-id="be1f5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be1f5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be1f5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="be1f5-125">Request body</span></span>
<span data-ttu-id="be1f5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be1f5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be1f5-127">响应</span><span class="sxs-lookup"><span data-stu-id="be1f5-127">Response</span></span>

<span data-ttu-id="be1f5-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="be1f5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be1f5-130">示例</span><span class="sxs-lookup"><span data-stu-id="be1f5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be1f5-131">请求</span><span class="sxs-lookup"><span data-stu-id="be1f5-131">Request</span></span>
<span data-ttu-id="be1f5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be1f5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="be1f5-133">响应</span><span class="sxs-lookup"><span data-stu-id="be1f5-133">Response</span></span>
<span data-ttu-id="be1f5-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="be1f5-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="be1f5-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="be1f5-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="be1f5-136">语言</span><span class="sxs-lookup"><span data-stu-id="be1f5-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_serviceprincipal-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be1f5-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="be1f5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_serviceprincipal-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
