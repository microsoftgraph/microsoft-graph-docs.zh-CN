---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: eb5ccfae61b94d5d8771f2ae5fef7d4e690324bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448703"
---
# <a name="list-deleted-items"></a><span data-ttu-id="23731-103">列出已删除项目</span><span class="sxs-lookup"><span data-stu-id="23731-103">List deleted items</span></span>

<span data-ttu-id="23731-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23731-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23731-105">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="23731-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="23731-106">目前，仅应用程序、组和用户资源支持已删除的项目[](../resources/application.md)功能。 [](../resources/group.md) [](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="23731-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="23731-107">权限</span><span class="sxs-lookup"><span data-stu-id="23731-107">Permissions</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

<span data-ttu-id="23731-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="23731-110">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="23731-110">For applications:</span></span>

|<span data-ttu-id="23731-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="23731-111">Permission type</span></span>      | <span data-ttu-id="23731-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23731-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23731-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23731-113">Delegated (work or school account)</span></span> | <span data-ttu-id="23731-114">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23731-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="23731-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23731-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23731-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="23731-116">Not supported.</span></span>    |
|<span data-ttu-id="23731-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="23731-117">Application</span></span> | <span data-ttu-id="23731-118">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23731-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="23731-119">对于用户：</span><span class="sxs-lookup"><span data-stu-id="23731-119">For users:</span></span>

|<span data-ttu-id="23731-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="23731-120">Permission type</span></span>      | <span data-ttu-id="23731-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23731-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23731-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23731-122">Delegated (work or school account)</span></span> | <span data-ttu-id="23731-123">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23731-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="23731-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23731-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23731-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="23731-125">Not supported.</span></span> |
|<span data-ttu-id="23731-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="23731-126">Application</span></span> | <span data-ttu-id="23731-127">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23731-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="23731-128">对于组：</span><span class="sxs-lookup"><span data-stu-id="23731-128">For groups:</span></span>

|<span data-ttu-id="23731-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="23731-129">Permission type</span></span>      | <span data-ttu-id="23731-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23731-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23731-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23731-131">Delegated (work or school account)</span></span> | <span data-ttu-id="23731-132">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23731-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="23731-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23731-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23731-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="23731-134">Not supported.</span></span>    |
|<span data-ttu-id="23731-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="23731-135">Application</span></span> | <span data-ttu-id="23731-136">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23731-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23731-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23731-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="23731-138">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="23731-138">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="23731-139">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="23731-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="23731-140">不支持在没有类型的情况下调用 GET /directory/deletedItems。</span><span class="sxs-lookup"><span data-stu-id="23731-140">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="23731-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23731-141">Optional query parameters</span></span>
<span data-ttu-id="23731-142">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23731-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23731-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="23731-143">Request headers</span></span>
| <span data-ttu-id="23731-144">名称</span><span class="sxs-lookup"><span data-stu-id="23731-144">Name</span></span>      |<span data-ttu-id="23731-145">说明</span><span class="sxs-lookup"><span data-stu-id="23731-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23731-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="23731-146">Authorization</span></span>  | <span data-ttu-id="23731-147">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="23731-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="23731-148">接受</span><span class="sxs-lookup"><span data-stu-id="23731-148">Accept</span></span>  | <span data-ttu-id="23731-149">application/json</span><span class="sxs-lookup"><span data-stu-id="23731-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="23731-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="23731-150">Request body</span></span>
<span data-ttu-id="23731-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23731-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23731-152">响应</span><span class="sxs-lookup"><span data-stu-id="23731-152">Response</span></span>

<span data-ttu-id="23731-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="23731-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23731-154">示例</span><span class="sxs-lookup"><span data-stu-id="23731-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23731-155">请求</span><span class="sxs-lookup"><span data-stu-id="23731-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="23731-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="23731-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="23731-157">C#</span><span class="sxs-lookup"><span data-stu-id="23731-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23731-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23731-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23731-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23731-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23731-160">Java</span><span class="sxs-lookup"><span data-stu-id="23731-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="23731-161">响应</span><span class="sxs-lookup"><span data-stu-id="23731-161">Response</span></span>
<span data-ttu-id="23731-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23731-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
