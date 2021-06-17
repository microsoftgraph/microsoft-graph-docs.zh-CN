---
title: 添加成员
description: 使用此 API 将用户或 (组的成员) 管理单元。
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 46bd9fee6ca7353132fb9bc16183093a7a5dd465
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991919"
---
# <a name="add-a-member"></a><span data-ttu-id="d8063-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="d8063-103">Add a member</span></span>

<span data-ttu-id="d8063-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8063-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8063-105">使用此 API 将用户或 (组的成员) 管理单元。</span><span class="sxs-lookup"><span data-stu-id="d8063-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="d8063-106">权限</span><span class="sxs-lookup"><span data-stu-id="d8063-106">Permissions</span></span>
<span data-ttu-id="d8063-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8063-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8063-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8063-109">Permission type</span></span>      | <span data-ttu-id="d8063-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8063-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8063-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8063-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d8063-112">AdministrativeUnit.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8063-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8063-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8063-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8063-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8063-114">Not supported.</span></span>    |
|<span data-ttu-id="d8063-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8063-115">Application</span></span> | <span data-ttu-id="d8063-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8063-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8063-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8063-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d8063-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8063-118">Request headers</span></span>
| <span data-ttu-id="d8063-119">名称</span><span class="sxs-lookup"><span data-stu-id="d8063-119">Name</span></span>      |<span data-ttu-id="d8063-120">说明</span><span class="sxs-lookup"><span data-stu-id="d8063-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8063-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8063-121">Authorization</span></span>  | <span data-ttu-id="d8063-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8063-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8063-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8063-124">Request body</span></span>
<span data-ttu-id="d8063-125">在请求正文中，提供 `id` 要[添加的用户、](../resources/user.md)[组](../resources/group.md)或[directoryObject](../resources/directoryobject.md)的 。</span><span class="sxs-lookup"><span data-stu-id="d8063-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d8063-126">响应</span><span class="sxs-lookup"><span data-stu-id="d8063-126">Response</span></span>

<span data-ttu-id="d8063-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d8063-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8063-129">示例</span><span class="sxs-lookup"><span data-stu-id="d8063-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8063-130">请求</span><span class="sxs-lookup"><span data-stu-id="d8063-130">Request</span></span>
<span data-ttu-id="d8063-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8063-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d8063-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8063-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeUnits_members"
} -->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="d8063-133">C#</span><span class="sxs-lookup"><span data-stu-id="d8063-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8063-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8063-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8063-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8063-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8063-136">Java</span><span class="sxs-lookup"><span data-stu-id="d8063-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d8063-137">在请求正文中， `id` 提供 [要添加](../resources/user.md) 的用户或 [组](../resources/group.md) 对象的 。</span><span class="sxs-lookup"><span data-stu-id="d8063-137">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="d8063-138">响应</span><span class="sxs-lookup"><span data-stu-id="d8063-138">Response</span></span>
<span data-ttu-id="d8063-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d8063-139">Here is an example of the response.</span></span>
 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


