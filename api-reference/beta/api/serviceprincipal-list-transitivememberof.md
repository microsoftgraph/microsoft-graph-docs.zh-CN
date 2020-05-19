---
title: 列出 servicePrincipal 可传递的 memberOf
description: 获取此服务主体所属的组和目录角色。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: f9807af8d7eda17eceec6a69113bafbcafbe1a7b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290045"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="4547c-103">列出 servicePrincipal 可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="4547c-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="4547c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4547c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4547c-105">获取此[servicePrincipal](../resources/serviceprincipal.md)所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="4547c-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="4547c-106">此操作是可传递的，将包括此服务主体是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="4547c-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4547c-107">权限</span><span class="sxs-lookup"><span data-stu-id="4547c-107">Permissions</span></span>
<span data-ttu-id="4547c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4547c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4547c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4547c-110">Permission type</span></span>      | <span data-ttu-id="4547c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4547c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4547c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4547c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4547c-113">所有的读取全部、全部的 Directory.accessasuser.all、全部、全部、全部、目录、全部、</span><span class="sxs-lookup"><span data-stu-id="4547c-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4547c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4547c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4547c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4547c-115">Not supported.</span></span>    |
|<span data-ttu-id="4547c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4547c-116">Application</span></span> | <span data-ttu-id="4547c-117">应用程序。全部，全部读取全部，全部为，全部为。</span><span class="sxs-lookup"><span data-stu-id="4547c-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="4547c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4547c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4547c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4547c-119">Optional query parameters</span></span>
<span data-ttu-id="4547c-120">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="4547c-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="4547c-121">此外，还会启用 OData 强制转换，例如，您可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="4547c-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="4547c-122">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="4547c-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="4547c-123">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="4547c-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="4547c-124">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="4547c-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4547c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4547c-125">Request headers</span></span>

| <span data-ttu-id="4547c-126">名称</span><span class="sxs-lookup"><span data-stu-id="4547c-126">Name</span></span>       | <span data-ttu-id="4547c-127">类型</span><span class="sxs-lookup"><span data-stu-id="4547c-127">Type</span></span> | <span data-ttu-id="4547c-128">说明</span><span class="sxs-lookup"><span data-stu-id="4547c-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4547c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4547c-129">Authorization</span></span>  | <span data-ttu-id="4547c-130">string</span><span class="sxs-lookup"><span data-stu-id="4547c-130">string</span></span>  | <span data-ttu-id="4547c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4547c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4547c-133">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="4547c-133">ConsistencyLevel</span></span> | <span data-ttu-id="4547c-134">仍然.</span><span class="sxs-lookup"><span data-stu-id="4547c-134">eventual.</span></span> <span data-ttu-id="4547c-135">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="4547c-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="4547c-136">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="4547c-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4547c-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="4547c-137">Request body</span></span>
<span data-ttu-id="4547c-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4547c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4547c-139">响应</span><span class="sxs-lookup"><span data-stu-id="4547c-139">Response</span></span>

<span data-ttu-id="4547c-140">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4547c-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4547c-141">示例</span><span class="sxs-lookup"><span data-stu-id="4547c-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="4547c-142">示例1：获取服务主体是其可传递成员的组和目录角色</span><span class="sxs-lookup"><span data-stu-id="4547c-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="4547c-143">请求</span><span class="sxs-lookup"><span data-stu-id="4547c-143">Request</span></span>

<span data-ttu-id="4547c-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4547c-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```

#### <a name="response"></a><span data-ttu-id="4547c-145">响应</span><span class="sxs-lookup"><span data-stu-id="4547c-145">Response</span></span>

<span data-ttu-id="4547c-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4547c-146">The following is an example of the response.</span></span> 
> <span data-ttu-id="4547c-147">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4547c-147">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4547c-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4547c-148">All of the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="4547c-149">示例2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="4547c-149">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="4547c-150">请求</span><span class="sxs-lookup"><span data-stu-id="4547c-150">Request</span></span>

<span data-ttu-id="4547c-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4547c-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4547c-152">响应</span><span class="sxs-lookup"><span data-stu-id="4547c-152">Response</span></span>

<span data-ttu-id="4547c-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4547c-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="4547c-154">294</span><span class="sxs-lookup"><span data-stu-id="4547c-154">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="4547c-155">示例3：使用 OData 强制转换仅获取组中的可传递成员身份数</span><span class="sxs-lookup"><span data-stu-id="4547c-155">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="4547c-156">请求</span><span class="sxs-lookup"><span data-stu-id="4547c-156">Request</span></span>

<span data-ttu-id="4547c-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4547c-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4547c-158">响应</span><span class="sxs-lookup"><span data-stu-id="4547c-158">Response</span></span>

<span data-ttu-id="4547c-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4547c-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="4547c-160">294</span><span class="sxs-lookup"><span data-stu-id="4547c-160">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="4547c-161">示例4：使用 $search 和 OData 强制转换来获取具有包含字母 "Video" 的显示名称的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="4547c-161">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4547c-162">请求</span><span class="sxs-lookup"><span data-stu-id="4547c-162">Request</span></span>

<span data-ttu-id="4547c-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4547c-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4547c-164">响应</span><span class="sxs-lookup"><span data-stu-id="4547c-164">Response</span></span>

<span data-ttu-id="4547c-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4547c-165">The following is an example of the response.</span></span>
><span data-ttu-id="4547c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4547c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="4547c-168">示例5：使用 $filter 和 OData 强制转换来获取带有以 ' A ' 开头的显示名称的组成员身份，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="4547c-168">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="4547c-169">请求</span><span class="sxs-lookup"><span data-stu-id="4547c-169">Request</span></span>

<span data-ttu-id="4547c-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4547c-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="4547c-171">响应</span><span class="sxs-lookup"><span data-stu-id="4547c-171">Response</span></span>

<span data-ttu-id="4547c-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4547c-172">The following is an example of the response.</span></span>
><span data-ttu-id="4547c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4547c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
