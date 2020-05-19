---
title: 列出 servicePrincipal memberOf
description: 获取此服务主体是其直接成员的组和目录角色。 此操作不可传递。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 31f40cc2abd804d29e63f7532542657a4d268d16
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291221"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="33801-104">列出 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="33801-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="33801-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33801-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33801-106">获取此[servicePrincipal](../resources/serviceprincipal.md)是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="33801-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="33801-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="33801-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="33801-108">权限</span><span class="sxs-lookup"><span data-stu-id="33801-108">Permissions</span></span>

<span data-ttu-id="33801-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33801-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33801-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="33801-111">Permission type</span></span>      | <span data-ttu-id="33801-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33801-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33801-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33801-113">Delegated (work or school account)</span></span> | <span data-ttu-id="33801-114">"Application"、"all"、"Directory.accessasuser.all"、"全部"、"全部"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="33801-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33801-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33801-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33801-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="33801-116">Not supported.</span></span>    |
|<span data-ttu-id="33801-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="33801-117">Application</span></span> | <span data-ttu-id="33801-118">"Application.readwrite.ownedby"、"全部"、"全部"、"全部"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="33801-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="33801-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33801-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33801-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="33801-120">Optional query parameters</span></span>

<span data-ttu-id="33801-121">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="33801-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="33801-122">此外，还会启用 OData 强制转换，例如，您可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="33801-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="33801-123">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="33801-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="33801-124">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="33801-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="33801-125">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="33801-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33801-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="33801-126">Request headers</span></span>

| <span data-ttu-id="33801-127">名称</span><span class="sxs-lookup"><span data-stu-id="33801-127">Name</span></span>       | <span data-ttu-id="33801-128">类型</span><span class="sxs-lookup"><span data-stu-id="33801-128">Type</span></span> | <span data-ttu-id="33801-129">说明</span><span class="sxs-lookup"><span data-stu-id="33801-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33801-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="33801-130">Authorization</span></span>  | <span data-ttu-id="33801-131">string</span><span class="sxs-lookup"><span data-stu-id="33801-131">string</span></span>  | <span data-ttu-id="33801-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33801-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33801-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="33801-134">ConsistencyLevel</span></span> | <span data-ttu-id="33801-135">仍然.</span><span class="sxs-lookup"><span data-stu-id="33801-135">eventual.</span></span> <span data-ttu-id="33801-136">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="33801-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="33801-137">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="33801-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33801-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="33801-138">Request body</span></span>
<span data-ttu-id="33801-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33801-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33801-140">响应</span><span class="sxs-lookup"><span data-stu-id="33801-140">Response</span></span>

<span data-ttu-id="33801-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="33801-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33801-142">示例</span><span class="sxs-lookup"><span data-stu-id="33801-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="33801-143">示例1：获取服务主体是其直接成员的组和目录角色</span><span class="sxs-lookup"><span data-stu-id="33801-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="33801-144">请求</span><span class="sxs-lookup"><span data-stu-id="33801-144">Request</span></span>

<span data-ttu-id="33801-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="33801-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="33801-146">响应</span><span class="sxs-lookup"><span data-stu-id="33801-146">Response</span></span>

<span data-ttu-id="33801-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="33801-147">The following is an example of the response.</span></span> 
> <span data-ttu-id="33801-148">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="33801-148">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="33801-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="33801-149">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="33801-150">示例2：仅获取所有成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="33801-150">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="33801-151">请求</span><span class="sxs-lookup"><span data-stu-id="33801-151">Request</span></span>

<span data-ttu-id="33801-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="33801-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="33801-153">响应</span><span class="sxs-lookup"><span data-stu-id="33801-153">Response</span></span>

<span data-ttu-id="33801-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="33801-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="33801-155">394</span><span class="sxs-lookup"><span data-stu-id="33801-155">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="33801-156">示例3：使用 OData 强制转换仅获取组成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="33801-156">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="33801-157">请求</span><span class="sxs-lookup"><span data-stu-id="33801-157">Request</span></span>

<span data-ttu-id="33801-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="33801-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="33801-159">响应</span><span class="sxs-lookup"><span data-stu-id="33801-159">Response</span></span>

<span data-ttu-id="33801-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="33801-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="33801-161">394</span><span class="sxs-lookup"><span data-stu-id="33801-161">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="33801-162">示例4：使用 $search 和 OData 强制转换来获取具有包含字母 "Video" 的显示名称的组成员身份，其中包括返回的对象的计数</span><span class="sxs-lookup"><span data-stu-id="33801-162">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="33801-163">请求</span><span class="sxs-lookup"><span data-stu-id="33801-163">Request</span></span>

<span data-ttu-id="33801-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="33801-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="33801-165">响应</span><span class="sxs-lookup"><span data-stu-id="33801-165">Response</span></span>

<span data-ttu-id="33801-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="33801-166">The following is an example of the response.</span></span>
><span data-ttu-id="33801-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="33801-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":1396,
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="33801-169">示例5：使用 $filter 和 OData 强制转换来获取具有以字母 "A" 开头的显示名称的组成员身份，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="33801-169">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="33801-170">请求</span><span class="sxs-lookup"><span data-stu-id="33801-170">Request</span></span>

<span data-ttu-id="33801-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="33801-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="33801-172">响应</span><span class="sxs-lookup"><span data-stu-id="33801-172">Response</span></span>

<span data-ttu-id="33801-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="33801-173">The following is an example of the response.</span></span>
><span data-ttu-id="33801-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="33801-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":76,
  "value":[
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
