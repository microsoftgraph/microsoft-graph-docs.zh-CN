---
title: 指定经理
description: 使用此 API 指定用户的经理。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e7405817115ef725e15f80a11d9c1cb63d65ed7e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278713"
---
# <a name="assign-a-manager"></a><span data-ttu-id="789e5-103">指定经理</span><span class="sxs-lookup"><span data-stu-id="789e5-103">Assign a manager</span></span>

<span data-ttu-id="789e5-104">使用此 API 指定用户的经理。</span><span class="sxs-lookup"><span data-stu-id="789e5-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="789e5-105">注意：不能指定直接下属，请改用此 API。</span><span class="sxs-lookup"><span data-stu-id="789e5-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="789e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="789e5-106">Permissions</span></span>
<span data-ttu-id="789e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="789e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="789e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="789e5-109">Permission type</span></span>      | <span data-ttu-id="789e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="789e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="789e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="789e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="789e5-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="789e5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="789e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="789e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="789e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="789e5-114">Not supported.</span></span>    |
|<span data-ttu-id="789e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="789e5-115">Application</span></span> | <span data-ttu-id="789e5-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="789e5-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="789e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="789e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="789e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="789e5-118">Request headers</span></span>
| <span data-ttu-id="789e5-119">名称</span><span class="sxs-lookup"><span data-stu-id="789e5-119">Name</span></span>       | <span data-ttu-id="789e5-120">类型</span><span class="sxs-lookup"><span data-stu-id="789e5-120">Type</span></span> | <span data-ttu-id="789e5-121">说明</span><span class="sxs-lookup"><span data-stu-id="789e5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="789e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="789e5-122">Authorization</span></span>  | <span data-ttu-id="789e5-123">string</span><span class="sxs-lookup"><span data-stu-id="789e5-123">string</span></span>  | <span data-ttu-id="789e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="789e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="789e5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="789e5-126">Request body</span></span>
<span data-ttu-id="789e5-127">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="789e5-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="789e5-128">响应</span><span class="sxs-lookup"><span data-stu-id="789e5-128">Response</span></span>

<span data-ttu-id="789e5-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="789e5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="789e5-131">示例</span><span class="sxs-lookup"><span data-stu-id="789e5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="789e5-132">请求</span><span class="sxs-lookup"><span data-stu-id="789e5-132">Request</span></span>
<span data-ttu-id="789e5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="789e5-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="789e5-134">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="789e5-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="789e5-135">响应</span><span class="sxs-lookup"><span data-stu-id="789e5-135">Response</span></span>
<span data-ttu-id="789e5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="789e5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="789e5-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="789e5-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="789e5-140">C#</span><span class="sxs-lookup"><span data-stu-id="789e5-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="789e5-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="789e5-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="789e5-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="789e5-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/user-post-manager.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-post-manager.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-post-manager.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
