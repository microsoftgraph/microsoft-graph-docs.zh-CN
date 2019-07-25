---
title: 删除 administrativeUnit
description: 删除 administrativeUnit。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f2f8073058767e54bcb36626ad864ea3257924fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855874"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="b0209-103">删除 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b0209-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0209-104">删除[administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="b0209-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0209-105">权限</span><span class="sxs-lookup"><span data-stu-id="b0209-105">Permissions</span></span>
<span data-ttu-id="b0209-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0209-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0209-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0209-108">Permission type</span></span>      | <span data-ttu-id="b0209-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0209-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0209-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0209-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0209-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0209-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0209-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0209-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0209-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0209-113">Not supported.</span></span>    |
|<span data-ttu-id="b0209-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0209-114">Application</span></span> | <span data-ttu-id="b0209-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0209-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0209-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0209-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b0209-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0209-117">Request headers</span></span>
| <span data-ttu-id="b0209-118">名称</span><span class="sxs-lookup"><span data-stu-id="b0209-118">Name</span></span>       | <span data-ttu-id="b0209-119">说明</span><span class="sxs-lookup"><span data-stu-id="b0209-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0209-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0209-120">Authorization</span></span>  | <span data-ttu-id="b0209-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0209-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0209-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0209-123">Request body</span></span>
<span data-ttu-id="b0209-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0209-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0209-125">响应</span><span class="sxs-lookup"><span data-stu-id="b0209-125">Response</span></span>

<span data-ttu-id="b0209-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b0209-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0209-128">示例</span><span class="sxs-lookup"><span data-stu-id="b0209-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0209-129">请求</span><span class="sxs-lookup"><span data-stu-id="b0209-129">Request</span></span>
<span data-ttu-id="b0209-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0209-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0209-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b0209-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0209-132">C#</span><span class="sxs-lookup"><span data-stu-id="b0209-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0209-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0209-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0209-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="b0209-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b0209-135">Java</span><span class="sxs-lookup"><span data-stu-id="b0209-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0209-136">响应</span><span class="sxs-lookup"><span data-stu-id="b0209-136">Response</span></span>
<span data-ttu-id="b0209-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0209-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
