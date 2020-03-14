---
title: 添加组所有者
description: 将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d141d6f6543f452c681d6d371a2548b12eabc58c
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639910"
---
# <a name="add-group-owner"></a><span data-ttu-id="08e3e-104">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="08e3e-104">Add group owner</span></span>

<span data-ttu-id="08e3e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08e3e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08e3e-106">将用户添加到组所有者。</span><span class="sxs-lookup"><span data-stu-id="08e3e-106">Add a user to the group's owners.</span></span> <span data-ttu-id="08e3e-107">所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="08e3e-107">The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="08e3e-108">**重要提示：** 如果更新组所有者并为该组创建团队，则所有者与 Microsoft Team 同步需要最多花费 2 小时。</span><span class="sxs-lookup"><span data-stu-id="08e3e-108">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="08e3e-109">此外，如果希望所有者能够在团队中进行更改，例如创建 Planner 计划，则还需要将所有者添加为组/团队成员。</span><span class="sxs-lookup"><span data-stu-id="08e3e-109">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="08e3e-110">权限</span><span class="sxs-lookup"><span data-stu-id="08e3e-110">Permissions</span></span>
<span data-ttu-id="08e3e-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08e3e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08e3e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="08e3e-113">Permission type</span></span>      | <span data-ttu-id="08e3e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08e3e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08e3e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08e3e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="08e3e-116">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08e3e-116">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08e3e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08e3e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08e3e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="08e3e-118">Not supported.</span></span>    |
|<span data-ttu-id="08e3e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="08e3e-119">Application</span></span> | <span data-ttu-id="08e3e-120">Group.ReadWrite.All 和 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e3e-120">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08e3e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08e3e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="08e3e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="08e3e-122">Request headers</span></span>
| <span data-ttu-id="08e3e-123">名称</span><span class="sxs-lookup"><span data-stu-id="08e3e-123">Name</span></span>       | <span data-ttu-id="08e3e-124">说明</span><span class="sxs-lookup"><span data-stu-id="08e3e-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08e3e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08e3e-125">Authorization</span></span>  | <span data-ttu-id="08e3e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08e3e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08e3e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08e3e-128">Content-Type</span></span> | <span data-ttu-id="08e3e-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="08e3e-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08e3e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="08e3e-131">Request body</span></span>
<span data-ttu-id="08e3e-132">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08e3e-132">In the request body, supply a JSON representation of the [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="08e3e-133">响应</span><span class="sxs-lookup"><span data-stu-id="08e3e-133">Response</span></span>
<span data-ttu-id="08e3e-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="08e3e-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e3e-136">示例</span><span class="sxs-lookup"><span data-stu-id="08e3e-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="08e3e-137">请求</span><span class="sxs-lookup"><span data-stu-id="08e3e-137">Request</span></span>
<span data-ttu-id="08e3e-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08e3e-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08e3e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="08e3e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="08e3e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08e3e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08e3e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08e3e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="08e3e-142">C#</span><span class="sxs-lookup"><span data-stu-id="08e3e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08e3e-143">Java</span><span class="sxs-lookup"><span data-stu-id="08e3e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="08e3e-144">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08e3e-144">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="08e3e-145">响应</span><span class="sxs-lookup"><span data-stu-id="08e3e-145">Response</span></span>
<span data-ttu-id="08e3e-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="08e3e-146">The following is an example of the response.</span></span>
><span data-ttu-id="08e3e-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="08e3e-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="08e3e-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="08e3e-148">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

