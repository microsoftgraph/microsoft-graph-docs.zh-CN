---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 213860aa7a5b93247b1e98de8da2ace8528cd111
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107646"
---
# <a name="list-deleted-items"></a><span data-ttu-id="7cdfe-103">列出已删除项目</span><span class="sxs-lookup"><span data-stu-id="7cdfe-103">List deleted items</span></span>

<span data-ttu-id="7cdfe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cdfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cdfe-105">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="7cdfe-106">目前，仅应用程序、组和用户资源支持已删除的项目[](../resources/application.md)功能。 [](../resources/group.md) [](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="7cdfe-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cdfe-107">权限</span><span class="sxs-lookup"><span data-stu-id="7cdfe-107">Permissions</span></span>

<span data-ttu-id="7cdfe-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="7cdfe-110">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="7cdfe-110">For applications:</span></span>

|<span data-ttu-id="7cdfe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cdfe-111">Permission type</span></span>      | <span data-ttu-id="7cdfe-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cdfe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7cdfe-114">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7cdfe-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7cdfe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cdfe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-116">Not supported.</span></span>    |
|<span data-ttu-id="7cdfe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cdfe-117">Application</span></span> | <span data-ttu-id="7cdfe-118">Application.Read.All、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cdfe-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="7cdfe-119">对于用户：</span><span class="sxs-lookup"><span data-stu-id="7cdfe-119">For users:</span></span>

|<span data-ttu-id="7cdfe-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cdfe-120">Permission type</span></span>      | <span data-ttu-id="7cdfe-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cdfe-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-122">Delegated (work or school account)</span></span> | <span data-ttu-id="7cdfe-123">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7cdfe-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7cdfe-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cdfe-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-125">Not supported.</span></span> |
|<span data-ttu-id="7cdfe-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cdfe-126">Application</span></span> | <span data-ttu-id="7cdfe-127">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cdfe-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="7cdfe-128">对于组：</span><span class="sxs-lookup"><span data-stu-id="7cdfe-128">For groups:</span></span>

|<span data-ttu-id="7cdfe-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cdfe-129">Permission type</span></span>      | <span data-ttu-id="7cdfe-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cdfe-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-131">Delegated (work or school account)</span></span> | <span data-ttu-id="7cdfe-132">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7cdfe-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7cdfe-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cdfe-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cdfe-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-134">Not supported.</span></span>    |
|<span data-ttu-id="7cdfe-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cdfe-135">Application</span></span> | <span data-ttu-id="7cdfe-136">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cdfe-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cdfe-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cdfe-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="7cdfe-138">此 API 当前支持检索应用程序的对象类型 (microsoft.graph.application) 、组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 删除的项目。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-138">This API currently supports retrieving object types of applications (microsoft.graph.application), groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="7cdfe-139">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="7cdfe-140">不支持在没有类型的情况下调用 GET /directory/deleteditems。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-140">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7cdfe-141">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7cdfe-141">Optional query parameters</span></span>
<span data-ttu-id="7cdfe-142">此方法支持 `$orderBy` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-142">This method supports the `$orderBy` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span> 

### <a name="examples-using-the-orderby-odata-query-parameter"></a><span data-ttu-id="7cdfe-143">使用 OData $orderBy参数的示例</span><span class="sxs-lookup"><span data-stu-id="7cdfe-143">Examples using the $orderBy OData query parameter</span></span>

<span data-ttu-id="7cdfe-144">`$orderBy`在已删除的对象类型的 **deletedDateTime** **、displayName** 和 **userPrincipalName** 属性上支持 OData 查询参数。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-144">The `$orderBy` OData query parameter is supported on the **deletedDateTime**, **displayName**, and **userPrincipalName** properties of the deleted object types.</span></span> <span data-ttu-id="7cdfe-145">在 **deletedDateTime** 属性上，查询需要将 [](/graph/aad-advanced-queries)高级查询参数 (**ConsistencyLevel** 标头设置为 ，并 `true` 添加 `$count=true` 查询字符串) 。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-145">On the **deletedDateTime** property, the query requires adding the [advanced query parameters](/graph/aad-advanced-queries) (**ConsistencyLevel** header set to `true` and `$count=true` query string).</span></span>

| <span data-ttu-id="7cdfe-146">OData 转换</span><span class="sxs-lookup"><span data-stu-id="7cdfe-146">OData cast</span></span> | <span data-ttu-id="7cdfe-147">支持属性$orderBy</span><span class="sxs-lookup"><span data-stu-id="7cdfe-147">Properties supporting $orderBy</span></span> | <span data-ttu-id="7cdfe-148">示例</span><span class="sxs-lookup"><span data-stu-id="7cdfe-148">Example</span></span> |
| :--- | :--- | :--- |
| <span data-ttu-id="7cdfe-149">microsoft.graph.user</span><span class="sxs-lookup"><span data-stu-id="7cdfe-149">microsoft.graph.user</span></span> | <span data-ttu-id="7cdfe-150">deletedDateTime、displayName、userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7cdfe-150">deletedDateTime, displayName, userPrincipalName</span></span> | <span data-ttu-id="7cdfe-151">/directory/deletedItems/microsoft.graph.user？$orderBy=userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7cdfe-151">/directory/deletedItems/microsoft.graph.user?$orderBy=userPrincipalName</span></span> |
| <span data-ttu-id="7cdfe-152">microsoft.graph.group</span><span class="sxs-lookup"><span data-stu-id="7cdfe-152">microsoft.graph.group</span></span> | <span data-ttu-id="7cdfe-153">deletedDateTime， displayName</span><span class="sxs-lookup"><span data-stu-id="7cdfe-153">deletedDateTime, displayName</span></span> | <span data-ttu-id="7cdfe-154">/directory/deletedItems/microsoft.graph.group？$orderBy=deletedDateTime asc&$count=true</span><span class="sxs-lookup"><span data-stu-id="7cdfe-154">/directory/deletedItems/microsoft.graph.group?$orderBy=deletedDateTime asc&$count=true</span></span> |
| <span data-ttu-id="7cdfe-155">microsoft.graph.application</span><span class="sxs-lookup"><span data-stu-id="7cdfe-155">microsoft.graph.application</span></span> | <span data-ttu-id="7cdfe-156">deletedDateTime， displayName</span><span class="sxs-lookup"><span data-stu-id="7cdfe-156">deletedDateTime, displayName</span></span> | <span data-ttu-id="7cdfe-157">/directory/deletedItems/microsoft.graph.application？$orderBy=displayName</span><span class="sxs-lookup"><span data-stu-id="7cdfe-157">/directory/deletedItems/microsoft.graph.application?$orderBy=displayName</span></span> |
| <span data-ttu-id="7cdfe-158">microsoft.graph.device</span><span class="sxs-lookup"><span data-stu-id="7cdfe-158">microsoft.graph.device</span></span> | <span data-ttu-id="7cdfe-159">deletedDateTime， displayName</span><span class="sxs-lookup"><span data-stu-id="7cdfe-159">deletedDateTime, displayName</span></span> | <span data-ttu-id="7cdfe-160">/directory/deletedItems/microsoft.graph.device？$orderBy=deletedDateTime&$count=true</span><span class="sxs-lookup"><span data-stu-id="7cdfe-160">/directory/deletedItems/microsoft.graph.device?$orderBy=deletedDateTime&$count=true</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7cdfe-161">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cdfe-161">Request headers</span></span>
| <span data-ttu-id="7cdfe-162">名称</span><span class="sxs-lookup"><span data-stu-id="7cdfe-162">Name</span></span>      |<span data-ttu-id="7cdfe-163">说明</span><span class="sxs-lookup"><span data-stu-id="7cdfe-163">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7cdfe-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cdfe-164">Authorization</span></span>  | <span data-ttu-id="7cdfe-165">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="7cdfe-165">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="7cdfe-166">接受</span><span class="sxs-lookup"><span data-stu-id="7cdfe-166">Accept</span></span>  | <span data-ttu-id="7cdfe-167">application/json</span><span class="sxs-lookup"><span data-stu-id="7cdfe-167">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cdfe-168">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cdfe-168">Request body</span></span>
<span data-ttu-id="7cdfe-169">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cdfe-170">响应</span><span class="sxs-lookup"><span data-stu-id="7cdfe-170">Response</span></span>

<span data-ttu-id="7cdfe-171">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-171">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7cdfe-172">示例</span><span class="sxs-lookup"><span data-stu-id="7cdfe-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cdfe-173">请求</span><span class="sxs-lookup"><span data-stu-id="7cdfe-173">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7cdfe-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cdfe-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="7cdfe-175">C#</span><span class="sxs-lookup"><span data-stu-id="7cdfe-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cdfe-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cdfe-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cdfe-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cdfe-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cdfe-178">Java</span><span class="sxs-lookup"><span data-stu-id="7cdfe-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7cdfe-179">响应</span><span class="sxs-lookup"><span data-stu-id="7cdfe-179">Response</span></span>
<span data-ttu-id="7cdfe-180">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7cdfe-180">Note: The response object shown here might be shortened for readability.</span></span>
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
