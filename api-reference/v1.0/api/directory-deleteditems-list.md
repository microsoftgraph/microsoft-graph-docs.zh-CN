---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 806c27af7410aae660f5d932c60f9b4165519b8c
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460430"
---
# <a name="list-deleted-items"></a><span data-ttu-id="0b312-103">列出已删除项目</span><span class="sxs-lookup"><span data-stu-id="0b312-103">List deleted items</span></span>

<span data-ttu-id="0b312-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b312-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b312-105">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="0b312-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="0b312-106">目前，仅支持 [应用程序](../resources/application.md)、 [组](../resources/group.md) 和 [用户](../resources/user.md) 资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="0b312-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b312-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0b312-107">Permissions</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

<span data-ttu-id="0b312-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="0b312-110">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="0b312-110">For applications:</span></span>

|<span data-ttu-id="0b312-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b312-111">Permission type</span></span>      | <span data-ttu-id="0b312-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b312-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b312-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b312-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0b312-114">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b312-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b312-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b312-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b312-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b312-116">Not supported.</span></span>    |
|<span data-ttu-id="0b312-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b312-117">Application</span></span> | <span data-ttu-id="0b312-118">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b312-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="0b312-119">对于用户：</span><span class="sxs-lookup"><span data-stu-id="0b312-119">For users:</span></span>

|<span data-ttu-id="0b312-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b312-120">Permission type</span></span>      | <span data-ttu-id="0b312-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b312-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b312-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b312-122">Delegated (work or school account)</span></span> | <span data-ttu-id="0b312-123">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b312-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0b312-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b312-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b312-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b312-125">Not supported.</span></span> |
|<span data-ttu-id="0b312-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b312-126">Application</span></span> | <span data-ttu-id="0b312-127">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b312-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="0b312-128">对于组：</span><span class="sxs-lookup"><span data-stu-id="0b312-128">For groups:</span></span>

|<span data-ttu-id="0b312-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b312-129">Permission type</span></span>      | <span data-ttu-id="0b312-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b312-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b312-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b312-131">Delegated (work or school account)</span></span> | <span data-ttu-id="0b312-132">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b312-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0b312-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b312-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b312-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b312-134">Not supported.</span></span>    |
|<span data-ttu-id="0b312-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b312-135">Application</span></span> | <span data-ttu-id="0b312-136">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b312-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b312-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b312-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="0b312-138">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="0b312-138">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="0b312-139">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="0b312-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="0b312-140">不支持不使用类型调用 GET/directory/deletedItems。</span><span class="sxs-lookup"><span data-stu-id="0b312-140">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="0b312-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b312-141">Optional query parameters</span></span>
<span data-ttu-id="0b312-142">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b312-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b312-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b312-143">Request headers</span></span>
| <span data-ttu-id="0b312-144">名称</span><span class="sxs-lookup"><span data-stu-id="0b312-144">Name</span></span>      |<span data-ttu-id="0b312-145">说明</span><span class="sxs-lookup"><span data-stu-id="0b312-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b312-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b312-146">Authorization</span></span>  | <span data-ttu-id="0b312-147">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="0b312-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="0b312-148">接受</span><span class="sxs-lookup"><span data-stu-id="0b312-148">Accept</span></span>  | <span data-ttu-id="0b312-149">application/json</span><span class="sxs-lookup"><span data-stu-id="0b312-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b312-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b312-150">Request body</span></span>
<span data-ttu-id="0b312-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b312-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b312-152">响应</span><span class="sxs-lookup"><span data-stu-id="0b312-152">Response</span></span>

<span data-ttu-id="0b312-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0b312-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b312-154">示例</span><span class="sxs-lookup"><span data-stu-id="0b312-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b312-155">请求</span><span class="sxs-lookup"><span data-stu-id="0b312-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0b312-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b312-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="0b312-157">C#</span><span class="sxs-lookup"><span data-stu-id="0b312-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b312-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b312-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b312-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b312-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b312-160">Java</span><span class="sxs-lookup"><span data-stu-id="0b312-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b312-161">响应</span><span class="sxs-lookup"><span data-stu-id="0b312-161">Response</span></span>
<span data-ttu-id="0b312-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b312-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
