---
title: 添加组所有者
description: 将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: eb42fef52921840d85f35de2fd832ca40831b866
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593618"
---
# <a name="add-group-owner"></a><span data-ttu-id="aa773-104">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="aa773-104">Add group owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa773-p102">将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="aa773-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="aa773-107">**重要提示：** 如果更新组所有者并为该组创建团队，则所有者与 Microsoft Team 同步需要最多花费 2 小时。</span><span class="sxs-lookup"><span data-stu-id="aa773-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="aa773-108">此外，如果希望所有者能够在团队中进行更改，例如创建 Planner 计划，则还需要将所有者添加为组/团队成员。</span><span class="sxs-lookup"><span data-stu-id="aa773-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="aa773-109">权限</span><span class="sxs-lookup"><span data-stu-id="aa773-109">Permissions</span></span>
<span data-ttu-id="aa773-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa773-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa773-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa773-112">Permission type</span></span>      | <span data-ttu-id="aa773-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa773-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa773-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa773-114">Delegated (work or school account)</span></span> | <span data-ttu-id="aa773-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa773-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa773-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa773-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa773-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa773-117">Not supported.</span></span>    |
|<span data-ttu-id="aa773-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa773-118">Application</span></span> | <span data-ttu-id="aa773-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa773-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa773-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa773-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="aa773-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa773-121">Request headers</span></span>
| <span data-ttu-id="aa773-122">名称</span><span class="sxs-lookup"><span data-stu-id="aa773-122">Name</span></span>       | <span data-ttu-id="aa773-123">类型</span><span class="sxs-lookup"><span data-stu-id="aa773-123">Type</span></span> | <span data-ttu-id="aa773-124">说明</span><span class="sxs-lookup"><span data-stu-id="aa773-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa773-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa773-125">Authorization</span></span>  | <span data-ttu-id="aa773-126">string</span><span class="sxs-lookup"><span data-stu-id="aa773-126">string</span></span>  | <span data-ttu-id="aa773-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa773-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa773-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa773-129">Request body</span></span>
<span data-ttu-id="aa773-130">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa773-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="aa773-131">响应</span><span class="sxs-lookup"><span data-stu-id="aa773-131">Response</span></span>
<span data-ttu-id="aa773-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="aa773-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa773-134">示例</span><span class="sxs-lookup"><span data-stu-id="aa773-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aa773-135">请求</span><span class="sxs-lookup"><span data-stu-id="aa773-135">Request</span></span>
<span data-ttu-id="aa773-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa773-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
<span data-ttu-id="aa773-137">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa773-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="aa773-138">响应</span><span class="sxs-lookup"><span data-stu-id="aa773-138">Response</span></span>
<span data-ttu-id="aa773-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aa773-139">The following is an example of the response.</span></span>
><span data-ttu-id="aa773-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aa773-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aa773-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aa773-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aa773-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="aa773-142">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa773-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa773-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-post-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
