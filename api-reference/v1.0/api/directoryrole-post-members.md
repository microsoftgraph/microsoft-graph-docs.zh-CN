---
title: 添加目录角色成员
description: 使用此 API 创建新的目录角色成员。
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c5f958f4543c985b6ecf8684080d261ed874028
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181376"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="b4197-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="b4197-103">Add directory role member</span></span>

<span data-ttu-id="b4197-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4197-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4197-105">使用此 API 创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="b4197-105">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4197-106">权限</span><span class="sxs-lookup"><span data-stu-id="b4197-106">Permissions</span></span>
<span data-ttu-id="b4197-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4197-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4197-109">Permission type</span></span>      | <span data-ttu-id="b4197-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4197-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4197-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4197-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4197-112">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="b4197-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4197-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4197-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4197-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4197-114">Not supported.</span></span>    |
|<span data-ttu-id="b4197-115">Application</span><span class="sxs-lookup"><span data-stu-id="b4197-115">Application</span></span> | <span data-ttu-id="b4197-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="b4197-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4197-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4197-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="b4197-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4197-118">Request headers</span></span>
| <span data-ttu-id="b4197-119">名称</span><span class="sxs-lookup"><span data-stu-id="b4197-119">Name</span></span>       | <span data-ttu-id="b4197-120">类型</span><span class="sxs-lookup"><span data-stu-id="b4197-120">Type</span></span> | <span data-ttu-id="b4197-121">说明</span><span class="sxs-lookup"><span data-stu-id="b4197-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b4197-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4197-122">Authorization</span></span>  | <span data-ttu-id="b4197-123">string</span><span class="sxs-lookup"><span data-stu-id="b4197-123">string</span></span>  | <span data-ttu-id="b4197-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4197-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4197-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4197-126">Content-Type</span></span>  | <span data-ttu-id="b4197-127">string</span><span class="sxs-lookup"><span data-stu-id="b4197-127">string</span></span>  | <span data-ttu-id="b4197-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b4197-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4197-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4197-129">Request body</span></span>
<span data-ttu-id="b4197-130">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4197-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="b4197-131">响应</span><span class="sxs-lookup"><span data-stu-id="b4197-131">Response</span></span>

<span data-ttu-id="b4197-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b4197-132">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4197-133">示例</span><span class="sxs-lookup"><span data-stu-id="b4197-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4197-134">请求</span><span class="sxs-lookup"><span data-stu-id="b4197-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b4197-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4197-135">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b4197-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4197-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4197-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4197-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b4197-138">C#</span><span class="sxs-lookup"><span data-stu-id="b4197-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4197-139">Java</span><span class="sxs-lookup"><span data-stu-id="b4197-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b4197-140">响应</span><span class="sxs-lookup"><span data-stu-id="b4197-140">Response</span></span>
<span data-ttu-id="b4197-141">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4197-141">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
