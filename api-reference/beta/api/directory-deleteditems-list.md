---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 883f23823c58b87e4969b10c96fde63be08058e9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046907"
---
# <a name="list-deleted-items"></a><span data-ttu-id="e4a96-103">列出已删除项目</span><span class="sxs-lookup"><span data-stu-id="e4a96-103">List deleted items</span></span>

<span data-ttu-id="e4a96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4a96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4a96-105">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="e4a96-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="e4a96-106">目前，仅应用程序、组和用户资源支持已删除的项目[](../resources/application.md)功能。 [](../resources/group.md) [](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="e4a96-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a96-107">权限</span><span class="sxs-lookup"><span data-stu-id="e4a96-107">Permissions</span></span>

<span data-ttu-id="e4a96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="e4a96-110">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="e4a96-110">For applications:</span></span>

|<span data-ttu-id="e4a96-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4a96-111">Permission type</span></span>      | <span data-ttu-id="e4a96-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4a96-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a96-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a96-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a96-114">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4a96-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4a96-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a96-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4a96-116">Not supported.</span></span>    |
|<span data-ttu-id="e4a96-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4a96-117">Application</span></span> | <span data-ttu-id="e4a96-118">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a96-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="e4a96-119">对于用户：</span><span class="sxs-lookup"><span data-stu-id="e4a96-119">For users:</span></span>

|<span data-ttu-id="e4a96-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4a96-120">Permission type</span></span>      | <span data-ttu-id="e4a96-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4a96-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a96-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a96-122">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a96-123">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4a96-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e4a96-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a96-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a96-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4a96-125">Not supported.</span></span> |
|<span data-ttu-id="e4a96-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4a96-126">Application</span></span> | <span data-ttu-id="e4a96-127">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a96-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="e4a96-128">对于组：</span><span class="sxs-lookup"><span data-stu-id="e4a96-128">For groups:</span></span>

|<span data-ttu-id="e4a96-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4a96-129">Permission type</span></span>      | <span data-ttu-id="e4a96-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4a96-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a96-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a96-131">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a96-132">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4a96-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e4a96-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4a96-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a96-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4a96-134">Not supported.</span></span>    |
|<span data-ttu-id="e4a96-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4a96-135">Application</span></span> | <span data-ttu-id="e4a96-136">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a96-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4a96-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4a96-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="e4a96-138">此 API 当前支持检索应用程序的对象类型 (microsoft.graph.application) 、组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 删除的项目。</span><span class="sxs-lookup"><span data-stu-id="e4a96-138">This API currently supports retrieving object types of applications (microsoft.graph.application), groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="e4a96-139">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="e4a96-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="e4a96-140">不支持在没有类型的情况下调用 GET /directory/deleteditems。</span><span class="sxs-lookup"><span data-stu-id="e4a96-140">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e4a96-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e4a96-141">Optional query parameters</span></span>
<span data-ttu-id="e4a96-142">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e4a96-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4a96-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4a96-143">Request headers</span></span>
| <span data-ttu-id="e4a96-144">名称</span><span class="sxs-lookup"><span data-stu-id="e4a96-144">Name</span></span>      |<span data-ttu-id="e4a96-145">说明</span><span class="sxs-lookup"><span data-stu-id="e4a96-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4a96-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4a96-146">Authorization</span></span>  | <span data-ttu-id="e4a96-147">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="e4a96-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="e4a96-148">接受</span><span class="sxs-lookup"><span data-stu-id="e4a96-148">Accept</span></span>  | <span data-ttu-id="e4a96-149">application/json</span><span class="sxs-lookup"><span data-stu-id="e4a96-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4a96-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4a96-150">Request body</span></span>
<span data-ttu-id="e4a96-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4a96-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4a96-152">响应</span><span class="sxs-lookup"><span data-stu-id="e4a96-152">Response</span></span>

<span data-ttu-id="e4a96-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e4a96-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4a96-154">示例</span><span class="sxs-lookup"><span data-stu-id="e4a96-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4a96-155">请求</span><span class="sxs-lookup"><span data-stu-id="e4a96-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e4a96-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a96-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="e4a96-157">C#</span><span class="sxs-lookup"><span data-stu-id="e4a96-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4a96-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4a96-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4a96-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4a96-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4a96-160">Java</span><span class="sxs-lookup"><span data-stu-id="e4a96-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e4a96-161">响应</span><span class="sxs-lookup"><span data-stu-id="e4a96-161">Response</span></span>
<span data-ttu-id="e4a96-162">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e4a96-162">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
