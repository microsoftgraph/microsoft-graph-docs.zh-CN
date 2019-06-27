---
title: 删除 programControl
description: 在 "Azure AD access 评论" 功能中, 删除 programControl 对象。  这会断开某个程序的访问评审。
localization_priority: Normal
ms.openlocfilehash: ddbd040d05d6e2c236a024e3d5eb8710562cebe9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264090"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="2cebf-104">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="2cebf-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cebf-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 删除[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2cebf-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="2cebf-106">这会断开某个程序的访问评审。</span><span class="sxs-lookup"><span data-stu-id="2cebf-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="2cebf-107">权限</span><span class="sxs-lookup"><span data-stu-id="2cebf-107">Permissions</span></span>
<span data-ttu-id="2cebf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cebf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cebf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cebf-110">Permission type</span></span>                        | <span data-ttu-id="2cebf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cebf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cebf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cebf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2cebf-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cebf-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="2cebf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cebf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cebf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cebf-115">Not supported.</span></span> |
|<span data-ttu-id="2cebf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cebf-116">Application</span></span>                            | <span data-ttu-id="2cebf-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cebf-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="2cebf-118">登录用户还必须位于允许他们删除的`programControl`目录角色中。</span><span class="sxs-lookup"><span data-stu-id="2cebf-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="2cebf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cebf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="2cebf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cebf-120">Request headers</span></span>
| <span data-ttu-id="2cebf-121">名称</span><span class="sxs-lookup"><span data-stu-id="2cebf-121">Name</span></span>         | <span data-ttu-id="2cebf-122">类型</span><span class="sxs-lookup"><span data-stu-id="2cebf-122">Type</span></span>        | <span data-ttu-id="2cebf-123">说明</span><span class="sxs-lookup"><span data-stu-id="2cebf-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2cebf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cebf-124">Authorization</span></span> | <span data-ttu-id="2cebf-125">string</span><span class="sxs-lookup"><span data-stu-id="2cebf-125">string</span></span> | <span data-ttu-id="2cebf-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="2cebf-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cebf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cebf-128">Request body</span></span>
<span data-ttu-id="2cebf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2cebf-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2cebf-130">响应</span><span class="sxs-lookup"><span data-stu-id="2cebf-130">Response</span></span>
<span data-ttu-id="2cebf-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2cebf-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cebf-133">示例</span><span class="sxs-lookup"><span data-stu-id="2cebf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cebf-134">请求</span><span class="sxs-lookup"><span data-stu-id="2cebf-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
##### <a name="response"></a><span data-ttu-id="2cebf-135">响应</span><span class="sxs-lookup"><span data-stu-id="2cebf-135">Response</span></span>
><span data-ttu-id="2cebf-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2cebf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2cebf-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2cebf-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2cebf-139">C#</span><span class="sxs-lookup"><span data-stu-id="2cebf-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_programControl-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2cebf-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="2cebf-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_programControl-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2cebf-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="2cebf-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_programControl-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
