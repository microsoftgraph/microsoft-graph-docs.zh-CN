---
title: 删除 scopedRoleMember
description: 从管理单元中删除作用域角色成员。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90272c109e7304071f7245f588607c764999d0b2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636679"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="7c7cb-103">删除 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="7c7cb-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7cb-104">从管理单元中删除作用域角色成员。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c7cb-105">权限</span><span class="sxs-lookup"><span data-stu-id="7c7cb-105">Permissions</span></span>
<span data-ttu-id="7c7cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7c7cb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c7cb-108">Permission type</span></span>      | <span data-ttu-id="7c7cb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c7cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c7cb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c7cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c7cb-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7c7cb-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7c7cb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c7cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c7cb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-113">Not supported.</span></span>    |
|<span data-ttu-id="7c7cb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c7cb-114">Application</span></span> | <span data-ttu-id="7c7cb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c7cb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c7cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7c7cb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c7cb-117">Request headers</span></span>
| <span data-ttu-id="7c7cb-118">名称</span><span class="sxs-lookup"><span data-stu-id="7c7cb-118">Name</span></span>       | <span data-ttu-id="7c7cb-119">说明</span><span class="sxs-lookup"><span data-stu-id="7c7cb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c7cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c7cb-120">Authorization</span></span>  | <span data-ttu-id="7c7cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c7cb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c7cb-123">Request body</span></span>
<span data-ttu-id="7c7cb-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c7cb-125">响应</span><span class="sxs-lookup"><span data-stu-id="7c7cb-125">Response</span></span>

<span data-ttu-id="7c7cb-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c7cb-128">示例</span><span class="sxs-lookup"><span data-stu-id="7c7cb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c7cb-129">请求</span><span class="sxs-lookup"><span data-stu-id="7c7cb-129">Request</span></span>
<span data-ttu-id="7c7cb-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="7c7cb-131">响应</span><span class="sxs-lookup"><span data-stu-id="7c7cb-131">Response</span></span>
<span data-ttu-id="7c7cb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c7cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7c7cb-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7c7cb-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7c7cb-136">语言</span><span class="sxs-lookup"><span data-stu-id="7c7cb-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c7cb-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c7cb-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
