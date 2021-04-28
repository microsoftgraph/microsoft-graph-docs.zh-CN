---
title: List device transitive groups
description: 获取设备是其中一个成员的组。
author: spunukol
ms.prod: directory-management
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: cf86bfa5235ae00450e14e8c5d221bb41f60e4f2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053221"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="8c281-103">List device transitive groups</span><span class="sxs-lookup"><span data-stu-id="8c281-103">List device transitive groups</span></span>

<span data-ttu-id="8c281-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c281-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c281-105">获取设备是其中一个成员的组。</span><span class="sxs-lookup"><span data-stu-id="8c281-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="8c281-106">此 API 请求是可传递的，并且还将返回设备是嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="8c281-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c281-107">权限</span><span class="sxs-lookup"><span data-stu-id="8c281-107">Permissions</span></span>

<span data-ttu-id="8c281-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c281-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c281-110">Permission type</span></span>      | <span data-ttu-id="8c281-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c281-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c281-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c281-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c281-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c281-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c281-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c281-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c281-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c281-115">Not supported.</span></span>    |
|<span data-ttu-id="8c281-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c281-116">Application</span></span> | <span data-ttu-id="8c281-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c281-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8c281-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c281-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c281-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8c281-119">Optional query parameters</span></span>

<span data-ttu-id="8c281-120">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="8c281-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="8c281-121">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="8c281-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="8c281-122">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="8c281-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="8c281-123">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="8c281-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="8c281-124">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="8c281-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c281-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c281-125">Request headers</span></span>

| <span data-ttu-id="8c281-126">标头</span><span class="sxs-lookup"><span data-stu-id="8c281-126">Header</span></span>       | <span data-ttu-id="8c281-127">值</span><span class="sxs-lookup"><span data-stu-id="8c281-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c281-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c281-128">Authorization</span></span>  | <span data-ttu-id="8c281-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c281-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8c281-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8c281-131">ConsistencyLevel</span></span> | <span data-ttu-id="8c281-132">最终。</span><span class="sxs-lookup"><span data-stu-id="8c281-132">eventual.</span></span> <span data-ttu-id="8c281-133">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="8c281-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="8c281-134">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="8c281-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c281-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c281-135">Request body</span></span>

<span data-ttu-id="8c281-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c281-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c281-137">响应</span><span class="sxs-lookup"><span data-stu-id="8c281-137">Response</span></span>

<span data-ttu-id="8c281-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c281-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c281-139">示例</span><span class="sxs-lookup"><span data-stu-id="8c281-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="8c281-140">示例 1：获取设备是可传递成员</span><span class="sxs-lookup"><span data-stu-id="8c281-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="8c281-141">请求</span><span class="sxs-lookup"><span data-stu-id="8c281-141">Request</span></span>

<span data-ttu-id="8c281-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8c281-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c281-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c281-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="8c281-144">C#</span><span class="sxs-lookup"><span data-stu-id="8c281-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c281-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c281-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c281-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c281-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c281-147">Java</span><span class="sxs-lookup"><span data-stu-id="8c281-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8c281-148">响应</span><span class="sxs-lookup"><span data-stu-id="8c281-148">Response</span></span>

<span data-ttu-id="8c281-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8c281-149">The following is an example of the response.</span></span>

><span data-ttu-id="8c281-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8c281-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="8c281-151">示例 2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="8c281-151">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="8c281-152">请求</span><span class="sxs-lookup"><span data-stu-id="8c281-152">Request</span></span>

<span data-ttu-id="8c281-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8c281-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8c281-154">响应</span><span class="sxs-lookup"><span data-stu-id="8c281-154">Response</span></span>

<span data-ttu-id="8c281-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8c281-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-and-search-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="8c281-156">示例 3：使用 OData 转换和$search获取显示名称包含字母"Video"（包括返回对象计数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="8c281-156">Example 3: Use OData cast and $search to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8c281-157">请求</span><span class="sxs-lookup"><span data-stu-id="8c281-157">Request</span></span>

<span data-ttu-id="8c281-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8c281-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8c281-159">响应</span><span class="sxs-lookup"><span data-stu-id="8c281-159">Response</span></span>

<span data-ttu-id="8c281-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8c281-160">The following is an example of the response.</span></span>

><span data-ttu-id="8c281-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8c281-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8c281-162">示例 4：使用 OData 转换$filter获取以"A"开头显示名称（包括返回对象计数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="8c281-162">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8c281-163">请求</span><span class="sxs-lookup"><span data-stu-id="8c281-163">Request</span></span>

<span data-ttu-id="8c281-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8c281-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8c281-165">响应</span><span class="sxs-lookup"><span data-stu-id="8c281-165">Response</span></span>

<span data-ttu-id="8c281-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8c281-166">The following is an example of the response.</span></span>

><span data-ttu-id="8c281-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8c281-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
