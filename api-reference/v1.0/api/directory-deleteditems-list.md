---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b2ef97fe5af0fc691b88303133007dee4347e08
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869968"
---
# <a name="list-deleted-items"></a><span data-ttu-id="b742f-103">列出已删除的项目</span><span class="sxs-lookup"><span data-stu-id="b742f-103">List deleted items</span></span>

<span data-ttu-id="b742f-104">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="b742f-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="b742f-105">目前，仅支持[应用程序](../resources/application.md)、[组](../resources/group.md)和[用户](../resources/user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="b742f-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="b742f-106">权限</span><span class="sxs-lookup"><span data-stu-id="b742f-106">Permissions</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

<span data-ttu-id="b742f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b742f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="b742f-109">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="b742f-109">For applications:</span></span>

|<span data-ttu-id="b742f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b742f-110">Permission type</span></span>      | <span data-ttu-id="b742f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b742f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b742f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b742f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b742f-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b742f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b742f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b742f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b742f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b742f-115">Not supported.</span></span>    |
|<span data-ttu-id="b742f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b742f-116">Application</span></span> | <span data-ttu-id="b742f-117">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b742f-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="b742f-118">对于用户：</span><span class="sxs-lookup"><span data-stu-id="b742f-118">For users:</span></span>

|<span data-ttu-id="b742f-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="b742f-119">Permission type</span></span>      | <span data-ttu-id="b742f-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b742f-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b742f-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b742f-121">Delegated (work or school account)</span></span> | <span data-ttu-id="b742f-122">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b742f-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b742f-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b742f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b742f-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="b742f-124">Not supported.</span></span> |
|<span data-ttu-id="b742f-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="b742f-125">Application</span></span> | <span data-ttu-id="b742f-126">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b742f-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="b742f-127">对于组：</span><span class="sxs-lookup"><span data-stu-id="b742f-127">For groups:</span></span>

|<span data-ttu-id="b742f-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="b742f-128">Permission type</span></span>      | <span data-ttu-id="b742f-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b742f-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b742f-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b742f-130">Delegated (work or school account)</span></span> | <span data-ttu-id="b742f-131">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b742f-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b742f-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b742f-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b742f-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="b742f-133">Not supported.</span></span>    |
|<span data-ttu-id="b742f-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="b742f-134">Application</span></span> | <span data-ttu-id="b742f-135">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b742f-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b742f-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b742f-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="b742f-137">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="b742f-137">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="b742f-138">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="b742f-138">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="b742f-139">不支持不使用类型调用 GET/directory/deletedItems。</span><span class="sxs-lookup"><span data-stu-id="b742f-139">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="b742f-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b742f-140">Optional query parameters</span></span>
<span data-ttu-id="b742f-141">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b742f-141">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b742f-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="b742f-142">Request headers</span></span>
| <span data-ttu-id="b742f-143">名称</span><span class="sxs-lookup"><span data-stu-id="b742f-143">Name</span></span>      |<span data-ttu-id="b742f-144">说明</span><span class="sxs-lookup"><span data-stu-id="b742f-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b742f-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="b742f-145">Authorization</span></span>  | <span data-ttu-id="b742f-146">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="b742f-146">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="b742f-147">接受</span><span class="sxs-lookup"><span data-stu-id="b742f-147">Accept</span></span>  | <span data-ttu-id="b742f-148">application/json</span><span class="sxs-lookup"><span data-stu-id="b742f-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b742f-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="b742f-149">Request body</span></span>
<span data-ttu-id="b742f-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b742f-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b742f-151">响应</span><span class="sxs-lookup"><span data-stu-id="b742f-151">Response</span></span>

<span data-ttu-id="b742f-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b742f-152">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b742f-153">示例</span><span class="sxs-lookup"><span data-stu-id="b742f-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b742f-154">请求</span><span class="sxs-lookup"><span data-stu-id="b742f-154">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b742f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b742f-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b742f-156">C#</span><span class="sxs-lookup"><span data-stu-id="b742f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b742f-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b742f-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b742f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b742f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b742f-159">Java</span><span class="sxs-lookup"><span data-stu-id="b742f-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b742f-160">响应</span><span class="sxs-lookup"><span data-stu-id="b742f-160">Response</span></span>
<span data-ttu-id="b742f-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b742f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
