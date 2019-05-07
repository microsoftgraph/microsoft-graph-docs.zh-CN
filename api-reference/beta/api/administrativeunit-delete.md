---
title: 删除 administrativeUnit
description: 删除 administrativeUnit。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fd7b23911c1c42bb98da397f8775dd6f73512d5a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636763"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="9c363-103">删除 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9c363-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c363-104">删除[administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="9c363-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c363-105">权限</span><span class="sxs-lookup"><span data-stu-id="9c363-105">Permissions</span></span>
<span data-ttu-id="9c363-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c363-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9c363-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c363-108">Permission type</span></span>      | <span data-ttu-id="9c363-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c363-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c363-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c363-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c363-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c363-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c363-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c363-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c363-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c363-113">Not supported.</span></span>    |
|<span data-ttu-id="9c363-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c363-114">Application</span></span> | <span data-ttu-id="9c363-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c363-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c363-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c363-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9c363-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c363-117">Request headers</span></span>
| <span data-ttu-id="9c363-118">名称</span><span class="sxs-lookup"><span data-stu-id="9c363-118">Name</span></span>       | <span data-ttu-id="9c363-119">说明</span><span class="sxs-lookup"><span data-stu-id="9c363-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9c363-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c363-120">Authorization</span></span>  | <span data-ttu-id="9c363-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c363-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c363-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c363-123">Request body</span></span>
<span data-ttu-id="9c363-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c363-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c363-125">响应</span><span class="sxs-lookup"><span data-stu-id="9c363-125">Response</span></span>

<span data-ttu-id="9c363-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9c363-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c363-128">示例</span><span class="sxs-lookup"><span data-stu-id="9c363-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c363-129">请求</span><span class="sxs-lookup"><span data-stu-id="9c363-129">Request</span></span>
<span data-ttu-id="9c363-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c363-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="9c363-131">响应</span><span class="sxs-lookup"><span data-stu-id="9c363-131">Response</span></span>
<span data-ttu-id="9c363-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c363-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9c363-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9c363-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9c363-136">语言</span><span class="sxs-lookup"><span data-stu-id="9c363-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c363-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9c363-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
