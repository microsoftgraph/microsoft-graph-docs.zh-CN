---
title: 添加组所有者
description: 将用户添加到组所有者。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e33dc95d60e56c0f2796f5eb9c3aa88b343d8634
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041188"
---
# <a name="add-group-owner"></a><span data-ttu-id="cf4e3-103">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="cf4e3-103">Add group owner</span></span>

<span data-ttu-id="cf4e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf4e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf4e3-105">将用户或服务主体添加到组的所有者。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-105">Add a user or service principal to the group's owners.</span></span> <span data-ttu-id="cf4e3-106">所有者是一组可修改组对象的用户或服务主体。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-106">The owners are a set of users or service principals who are allowed to modify the group object.</span></span>

><span data-ttu-id="cf4e3-107">**重要提示：** 如果更新组所有者并为该组创建团队，则所有者与 Microsoft Team 同步需要最多花费 2 小时。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="cf4e3-108">此外，如果希望所有者能够在团队中进行更改，例如创建 Planner 计划，则还需要将所有者添加为组/团队成员。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cf4e3-109">权限</span><span class="sxs-lookup"><span data-stu-id="cf4e3-109">Permissions</span></span>
<span data-ttu-id="cf4e3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf4e3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf4e3-112">Permission type</span></span>      | <span data-ttu-id="cf4e3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf4e3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf4e3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf4e3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cf4e3-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cf4e3-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cf4e3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf4e3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf4e3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-117">Not supported.</span></span>    |
|<span data-ttu-id="cf4e3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf4e3-118">Application</span></span> | <span data-ttu-id="cf4e3-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4e3-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf4e3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf4e3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cf4e3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf4e3-121">Request headers</span></span>
| <span data-ttu-id="cf4e3-122">名称</span><span class="sxs-lookup"><span data-stu-id="cf4e3-122">Name</span></span>       | <span data-ttu-id="cf4e3-123">说明</span><span class="sxs-lookup"><span data-stu-id="cf4e3-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf4e3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf4e3-124">Authorization</span></span>  | <span data-ttu-id="cf4e3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf4e3-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="cf4e3-127">Content-type</span></span> | <span data-ttu-id="cf4e3-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cf4e3-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf4e3-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf4e3-130">Request body</span></span>
<span data-ttu-id="cf4e3-131">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-131">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="cf4e3-132">响应</span><span class="sxs-lookup"><span data-stu-id="cf4e3-132">Response</span></span>
<span data-ttu-id="cf4e3-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-133">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="cf4e3-134">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-134">It does not return anything in the response body.</span></span> <span data-ttu-id="cf4e3-135">当对象已是组的成员时，此方法将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-135">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="cf4e3-136">当添加的对象不存在时，此方法返回 `404 Not Found` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-136">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span>

## <a name="example"></a><span data-ttu-id="cf4e3-137">示例</span><span class="sxs-lookup"><span data-stu-id="cf4e3-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cf4e3-138">请求</span><span class="sxs-lookup"><span data-stu-id="cf4e3-138">Request</span></span>
<span data-ttu-id="cf4e3-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf4e3-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf4e3-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="cf4e3-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf4e3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf4e3-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf4e3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cf4e3-143">C#</span><span class="sxs-lookup"><span data-stu-id="cf4e3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf4e3-144">Java</span><span class="sxs-lookup"><span data-stu-id="cf4e3-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cf4e3-145">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-145">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="cf4e3-146">响应</span><span class="sxs-lookup"><span data-stu-id="cf4e3-146">Response</span></span>
<span data-ttu-id="cf4e3-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-147">The following is an example of the response.</span></span>
><span data-ttu-id="cf4e3-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cf4e3-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


