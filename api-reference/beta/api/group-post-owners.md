---
title: 添加组所有者
description: 将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。
localization_priority: Normal
ms.openlocfilehash: 3fe136b0ea76ae2d6f535af421d016bf27c58a6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883193"
---
# <a name="add-group-owner"></a><span data-ttu-id="cead5-104">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="cead5-104">Add group owner</span></span>

> <span data-ttu-id="cead5-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cead5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cead5-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cead5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cead5-p103">将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="cead5-p103">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="cead5-109">**重要：** 如果更新组的所有者和创建组团队，它可以最多为 2 小时数所有者以便与 Microsoft 团队进行同步。</span><span class="sxs-lookup"><span data-stu-id="cead5-109">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="cead5-110">此外，如果您希望能够-例如，通过创建计划工具计划-团队中做出的更改的所有者所有者还需要添加为组/工作组成员。</span><span class="sxs-lookup"><span data-stu-id="cead5-110">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cead5-111">权限</span><span class="sxs-lookup"><span data-stu-id="cead5-111">Permissions</span></span>
<span data-ttu-id="cead5-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cead5-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cead5-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="cead5-114">Permission type</span></span>      | <span data-ttu-id="cead5-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cead5-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cead5-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cead5-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cead5-117">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cead5-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cead5-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cead5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cead5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cead5-119">Not supported.</span></span>    |
|<span data-ttu-id="cead5-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="cead5-120">Application</span></span> | <span data-ttu-id="cead5-121">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cead5-121">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cead5-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cead5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cead5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="cead5-123">Request headers</span></span>
| <span data-ttu-id="cead5-124">名称</span><span class="sxs-lookup"><span data-stu-id="cead5-124">Name</span></span>       | <span data-ttu-id="cead5-125">类型</span><span class="sxs-lookup"><span data-stu-id="cead5-125">Type</span></span> | <span data-ttu-id="cead5-126">说明</span><span class="sxs-lookup"><span data-stu-id="cead5-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cead5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cead5-127">Authorization</span></span>  | <span data-ttu-id="cead5-128">string</span><span class="sxs-lookup"><span data-stu-id="cead5-128">string</span></span>  | <span data-ttu-id="cead5-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cead5-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cead5-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="cead5-131">Request body</span></span>
<span data-ttu-id="cead5-132">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cead5-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="cead5-133">响应</span><span class="sxs-lookup"><span data-stu-id="cead5-133">Response</span></span>
<span data-ttu-id="cead5-p107">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cead5-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cead5-136">示例</span><span class="sxs-lookup"><span data-stu-id="cead5-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cead5-137">请求</span><span class="sxs-lookup"><span data-stu-id="cead5-137">Request</span></span>
<span data-ttu-id="cead5-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cead5-138">The following is an example of the request.</span></span>
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
<span data-ttu-id="cead5-139">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cead5-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="cead5-140">响应</span><span class="sxs-lookup"><span data-stu-id="cead5-140">Response</span></span>
<span data-ttu-id="cead5-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cead5-141">The following is an example of the response.</span></span>
><span data-ttu-id="cead5-142">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cead5-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cead5-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cead5-143">All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
