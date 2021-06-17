---
title: 删除 scopedRoleMember
description: 从管理单元中删除作用域角色成员。
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0974d361ce125ce9f2a337d8d73be44b2e8541d0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992070"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="b0698-103">删除 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="b0698-103">Remove a scopedRoleMember</span></span>

<span data-ttu-id="b0698-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0698-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0698-105">从管理单元中删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="b0698-105">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0698-106">权限</span><span class="sxs-lookup"><span data-stu-id="b0698-106">Permissions</span></span>
<span data-ttu-id="b0698-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b0698-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0698-109">Permission type</span></span>      | <span data-ttu-id="b0698-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0698-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0698-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0698-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0698-112">RoleManagement.ReadWrite.Directory、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0698-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0698-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0698-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0698-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0698-114">Not supported.</span></span>    |
|<span data-ttu-id="b0698-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0698-115">Application</span></span> | <span data-ttu-id="b0698-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="b0698-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0698-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0698-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b0698-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0698-118">Request headers</span></span>
| <span data-ttu-id="b0698-119">名称</span><span class="sxs-lookup"><span data-stu-id="b0698-119">Name</span></span>       | <span data-ttu-id="b0698-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0698-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0698-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0698-121">Authorization</span></span>  | <span data-ttu-id="b0698-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0698-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0698-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0698-124">Request body</span></span>
<span data-ttu-id="b0698-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0698-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0698-126">响应</span><span class="sxs-lookup"><span data-stu-id="b0698-126">Response</span></span>

<span data-ttu-id="b0698-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b0698-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0698-129">示例</span><span class="sxs-lookup"><span data-stu-id="b0698-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0698-130">请求</span><span class="sxs-lookup"><span data-stu-id="b0698-130">Request</span></span>
<span data-ttu-id="b0698-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0698-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0698-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0698-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="b0698-133">C#</span><span class="sxs-lookup"><span data-stu-id="b0698-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0698-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0698-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0698-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0698-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0698-136">Java</span><span class="sxs-lookup"><span data-stu-id="b0698-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0698-137">响应</span><span class="sxs-lookup"><span data-stu-id="b0698-137">Response</span></span>
<span data-ttu-id="b0698-p104">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b0698-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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


