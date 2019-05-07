---
title: 指定经理
description: 使用此 API 指定用户的经理。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 89026e208c83840cbf10b681154b8ebf1c38e991
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637104"
---
# <a name="assign-a-manager"></a><span data-ttu-id="4c4ab-103">指定经理</span><span class="sxs-lookup"><span data-stu-id="4c4ab-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c4ab-104">使用此 API 指定用户的经理。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="4c4ab-105">注意：不能指定直接下属，请改用此 API。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c4ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="4c4ab-106">Permissions</span></span>
<span data-ttu-id="4c4ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c4ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c4ab-109">Permission type</span></span>      | <span data-ttu-id="4c4ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c4ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c4ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c4ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4c4ab-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c4ab-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c4ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c4ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c4ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-114">Not supported.</span></span>    |
|<span data-ttu-id="4c4ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c4ab-115">Application</span></span> | <span data-ttu-id="4c4ab-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c4ab-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c4ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c4ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4c4ab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c4ab-118">Request headers</span></span>
| <span data-ttu-id="4c4ab-119">名称</span><span class="sxs-lookup"><span data-stu-id="4c4ab-119">Name</span></span>       | <span data-ttu-id="4c4ab-120">类型</span><span class="sxs-lookup"><span data-stu-id="4c4ab-120">Type</span></span> | <span data-ttu-id="4c4ab-121">说明</span><span class="sxs-lookup"><span data-stu-id="4c4ab-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c4ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c4ab-122">Authorization</span></span>  | <span data-ttu-id="4c4ab-123">string</span><span class="sxs-lookup"><span data-stu-id="4c4ab-123">string</span></span>  | <span data-ttu-id="4c4ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c4ab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c4ab-126">Request body</span></span>
<span data-ttu-id="4c4ab-127">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="4c4ab-128">响应</span><span class="sxs-lookup"><span data-stu-id="4c4ab-128">Response</span></span>

<span data-ttu-id="4c4ab-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c4ab-131">示例</span><span class="sxs-lookup"><span data-stu-id="4c4ab-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c4ab-132">请求</span><span class="sxs-lookup"><span data-stu-id="4c4ab-132">Request</span></span>
<span data-ttu-id="4c4ab-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="4c4ab-134">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="4c4ab-135">响应</span><span class="sxs-lookup"><span data-stu-id="4c4ab-135">Response</span></span>
<span data-ttu-id="4c4ab-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c4ab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c4ab-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4c4ab-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4c4ab-140">语言</span><span class="sxs-lookup"><span data-stu-id="4c4ab-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c4ab-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c4ab-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-manager.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-manager.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
