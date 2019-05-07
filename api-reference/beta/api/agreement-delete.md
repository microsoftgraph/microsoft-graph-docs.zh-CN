---
title: 删除协议
description: 删除协议对象。
localization_priority: Normal
ms.openlocfilehash: ae2326f3ff2d1b13c4b4401a07b116db2e47876e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636595"
---
# <a name="delete-agreement"></a><span data-ttu-id="3bade-103">删除协议</span><span class="sxs-lookup"><span data-stu-id="3bade-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bade-104">删除[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3bade-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3bade-105">权限</span><span class="sxs-lookup"><span data-stu-id="3bade-105">Permissions</span></span>
<span data-ttu-id="3bade-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bade-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bade-108">Permission type</span></span>                        | <span data-ttu-id="3bade-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3bade-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bade-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bade-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bade-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bade-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="3bade-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bade-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bade-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bade-113">Not supported.</span></span> |
|<span data-ttu-id="3bade-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bade-114">Application</span></span>                            | <span data-ttu-id="3bade-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bade-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bade-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bade-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="3bade-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bade-117">Request headers</span></span>
| <span data-ttu-id="3bade-118">名称</span><span class="sxs-lookup"><span data-stu-id="3bade-118">Name</span></span>         | <span data-ttu-id="3bade-119">类型</span><span class="sxs-lookup"><span data-stu-id="3bade-119">Type</span></span>        | <span data-ttu-id="3bade-120">说明</span><span class="sxs-lookup"><span data-stu-id="3bade-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3bade-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bade-121">Authorization</span></span> | <span data-ttu-id="3bade-122">string</span><span class="sxs-lookup"><span data-stu-id="3bade-122">string</span></span> | <span data-ttu-id="3bade-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="3bade-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bade-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bade-125">Request body</span></span>
<span data-ttu-id="3bade-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3bade-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3bade-127">响应</span><span class="sxs-lookup"><span data-stu-id="3bade-127">Response</span></span>
<span data-ttu-id="3bade-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3bade-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bade-130">示例</span><span class="sxs-lookup"><span data-stu-id="3bade-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bade-131">请求</span><span class="sxs-lookup"><span data-stu-id="3bade-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="3bade-132">响应</span><span class="sxs-lookup"><span data-stu-id="3bade-132">Response</span></span>
><span data-ttu-id="3bade-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3bade-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bade-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3bade-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bade-136">语言</span><span class="sxs-lookup"><span data-stu-id="3bade-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_agreement-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bade-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3bade-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_agreement-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
