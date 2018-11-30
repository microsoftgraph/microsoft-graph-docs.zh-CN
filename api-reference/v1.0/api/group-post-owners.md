---
title: 添加组所有者
description: 将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。
ms.openlocfilehash: 8c879430c78cb1d06150bade842addcb4ba0af38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009528"
---
# <a name="add-group-owner"></a><span data-ttu-id="cdd42-104">添加组所有者</span><span class="sxs-lookup"><span data-stu-id="cdd42-104">Add group owner</span></span>
<span data-ttu-id="cdd42-p102">将用户添加到组所有者。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="cdd42-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdd42-107">权限</span><span class="sxs-lookup"><span data-stu-id="cdd42-107">Permissions</span></span>
<span data-ttu-id="cdd42-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdd42-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdd42-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdd42-110">Permission type</span></span>      | <span data-ttu-id="cdd42-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdd42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdd42-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdd42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd42-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cdd42-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cdd42-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdd42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd42-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdd42-115">Not supported.</span></span>    |
|<span data-ttu-id="cdd42-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdd42-116">Application</span></span> | <span data-ttu-id="cdd42-117">Group.ReadWrite.All 和 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd42-117">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdd42-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdd42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cdd42-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdd42-119">Request headers</span></span>
| <span data-ttu-id="cdd42-120">名称</span><span class="sxs-lookup"><span data-stu-id="cdd42-120">Name</span></span>       | <span data-ttu-id="cdd42-121">类型</span><span class="sxs-lookup"><span data-stu-id="cdd42-121">Type</span></span> | <span data-ttu-id="cdd42-122">说明</span><span class="sxs-lookup"><span data-stu-id="cdd42-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cdd42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdd42-123">Authorization</span></span>  | <span data-ttu-id="cdd42-124">string</span><span class="sxs-lookup"><span data-stu-id="cdd42-124">string</span></span>  | <span data-ttu-id="cdd42-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdd42-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdd42-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdd42-127">Request body</span></span>
<span data-ttu-id="cdd42-128">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdd42-128">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="cdd42-129">响应</span><span class="sxs-lookup"><span data-stu-id="cdd42-129">Response</span></span>
<span data-ttu-id="cdd42-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cdd42-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdd42-132">示例</span><span class="sxs-lookup"><span data-stu-id="cdd42-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cdd42-133">请求</span><span class="sxs-lookup"><span data-stu-id="cdd42-133">Request</span></span>
<span data-ttu-id="cdd42-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdd42-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="cdd42-135">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdd42-135">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="cdd42-136">响应</span><span class="sxs-lookup"><span data-stu-id="cdd42-136">Response</span></span>
<span data-ttu-id="cdd42-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdd42-137">The following is an example of the response.</span></span>
><span data-ttu-id="cdd42-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cdd42-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cdd42-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdd42-139">All the properties will be returned from an actual call.</span></span>
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
