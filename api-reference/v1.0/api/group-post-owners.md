---
title: 添加组所有者
description: 将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a0f46e67de69762ebf26600726dd58e74fbcbe5e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337139"
---
# <a name="add-group-owner"></a><span data-ttu-id="4328e-104">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="4328e-104">Add group owner</span></span>
<span data-ttu-id="4328e-p102">将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="4328e-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="4328e-107">**重要提示：** 如果更新组所有者并为该组创建团队，则所有者与 Microsoft Team 同步需要最多花费 2 小时。</span><span class="sxs-lookup"><span data-stu-id="4328e-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="4328e-108">此外，如果希望所有者能够在团队中进行更改，例如创建 Planner 计划，则还需要将所有者添加为组/团队成员。</span><span class="sxs-lookup"><span data-stu-id="4328e-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4328e-109">权限</span><span class="sxs-lookup"><span data-stu-id="4328e-109">Permissions</span></span>
<span data-ttu-id="4328e-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4328e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4328e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4328e-112">Permission type</span></span>      | <span data-ttu-id="4328e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4328e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4328e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4328e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4328e-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4328e-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4328e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4328e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4328e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4328e-117">Not supported.</span></span>    |
|<span data-ttu-id="4328e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4328e-118">Application</span></span> | <span data-ttu-id="4328e-119">Group.ReadWrite.All 和 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4328e-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4328e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4328e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4328e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4328e-121">Request headers</span></span>
| <span data-ttu-id="4328e-122">名称</span><span class="sxs-lookup"><span data-stu-id="4328e-122">Name</span></span>       | <span data-ttu-id="4328e-123">类型</span><span class="sxs-lookup"><span data-stu-id="4328e-123">Type</span></span> | <span data-ttu-id="4328e-124">说明</span><span class="sxs-lookup"><span data-stu-id="4328e-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4328e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4328e-125">Authorization</span></span>  | <span data-ttu-id="4328e-126">string</span><span class="sxs-lookup"><span data-stu-id="4328e-126">string</span></span>  | <span data-ttu-id="4328e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4328e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4328e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4328e-129">Request body</span></span>
<span data-ttu-id="4328e-130">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4328e-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="4328e-131">响应</span><span class="sxs-lookup"><span data-stu-id="4328e-131">Response</span></span>
<span data-ttu-id="4328e-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4328e-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4328e-134">示例</span><span class="sxs-lookup"><span data-stu-id="4328e-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4328e-135">请求</span><span class="sxs-lookup"><span data-stu-id="4328e-135">Request</span></span>
<span data-ttu-id="4328e-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4328e-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4328e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4328e-137">--Http</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4328e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4328e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4328e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4328e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="4328e-140">C#</span><span class="sxs-lookup"><span data-stu-id="4328e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4328e-141">Java</span><span class="sxs-lookup"><span data-stu-id="4328e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4328e-142">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4328e-142">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="4328e-143">响应</span><span class="sxs-lookup"><span data-stu-id="4328e-143">Response</span></span>
<span data-ttu-id="4328e-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4328e-144">The following is an example of the response.</span></span>
><span data-ttu-id="4328e-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4328e-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4328e-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4328e-146">All the properties will be returned from an actual call.</span></span>
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

