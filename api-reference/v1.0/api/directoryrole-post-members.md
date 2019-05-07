---
title: 添加目录角色成员
description: 使用此 API 创建新的目录角色成员。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 768e2a780fcfe96bd14d883d0f7ea0d03ac434cc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33617085"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="ed5ad-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="ed5ad-103">Add directory role member</span></span>

<span data-ttu-id="ed5ad-104">使用此 API 创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed5ad-105">权限</span><span class="sxs-lookup"><span data-stu-id="ed5ad-105">Permissions</span></span>
<span data-ttu-id="ed5ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed5ad-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed5ad-108">Permission type</span></span>      | <span data-ttu-id="ed5ad-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed5ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed5ad-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed5ad-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed5ad-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed5ad-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed5ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed5ad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-113">Not supported.</span></span>    |
|<span data-ttu-id="ed5ad-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed5ad-114">Application</span></span> | <span data-ttu-id="ed5ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed5ad-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed5ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="ed5ad-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed5ad-117">Request headers</span></span>
| <span data-ttu-id="ed5ad-118">名称</span><span class="sxs-lookup"><span data-stu-id="ed5ad-118">Name</span></span>       | <span data-ttu-id="ed5ad-119">类型</span><span class="sxs-lookup"><span data-stu-id="ed5ad-119">Type</span></span> | <span data-ttu-id="ed5ad-120">说明</span><span class="sxs-lookup"><span data-stu-id="ed5ad-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed5ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed5ad-121">Authorization</span></span>  | <span data-ttu-id="ed5ad-122">string</span><span class="sxs-lookup"><span data-stu-id="ed5ad-122">string</span></span>  | <span data-ttu-id="ed5ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed5ad-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed5ad-125">Content-Type</span></span>  | <span data-ttu-id="ed5ad-126">string</span><span class="sxs-lookup"><span data-stu-id="ed5ad-126">string</span></span>  | <span data-ttu-id="ed5ad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ed5ad-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed5ad-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed5ad-128">Request body</span></span>
<span data-ttu-id="ed5ad-129">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="ed5ad-130">响应</span><span class="sxs-lookup"><span data-stu-id="ed5ad-130">Response</span></span>

<span data-ttu-id="ed5ad-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed5ad-132">示例</span><span class="sxs-lookup"><span data-stu-id="ed5ad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed5ad-133">请求</span><span class="sxs-lookup"><span data-stu-id="ed5ad-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="ed5ad-134">响应</span><span class="sxs-lookup"><span data-stu-id="ed5ad-134">Response</span></span>
<span data-ttu-id="ed5ad-135">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed5ad-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed5ad-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ed5ad-136">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed5ad-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed5ad-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
