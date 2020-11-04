---
title: List device transitive groups
description: 获取设备所属的组。
author: spunukol
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 3c33ae8796420ce1191ca4e79a71aa900063659a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905286"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="b582c-103">List device transitive groups</span><span class="sxs-lookup"><span data-stu-id="b582c-103">List device transitive groups</span></span>

<span data-ttu-id="b582c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b582c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b582c-105">获取设备所属的组。</span><span class="sxs-lookup"><span data-stu-id="b582c-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="b582c-106">此 API 请求是可传递的，并且还将返回设备是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="b582c-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="b582c-107">权限</span><span class="sxs-lookup"><span data-stu-id="b582c-107">Permissions</span></span>

<span data-ttu-id="b582c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b582c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b582c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b582c-110">Permission type</span></span>      | <span data-ttu-id="b582c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b582c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b582c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b582c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b582c-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b582c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b582c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b582c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b582c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b582c-115">Not supported.</span></span>    |
|<span data-ttu-id="b582c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b582c-116">Application</span></span> | <span data-ttu-id="b582c-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b582c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b582c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b582c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b582c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b582c-119">Optional query parameters</span></span>

<span data-ttu-id="b582c-120">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="b582c-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="b582c-121">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="b582c-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="b582c-122">可使用“ **displayName** ”和“ **说明** ”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="b582c-122">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="b582c-123">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="b582c-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b582c-124">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="b582c-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b582c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b582c-125">Request headers</span></span>

| <span data-ttu-id="b582c-126">标头</span><span class="sxs-lookup"><span data-stu-id="b582c-126">Header</span></span>       | <span data-ttu-id="b582c-127">值</span><span class="sxs-lookup"><span data-stu-id="b582c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b582c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b582c-128">Authorization</span></span>  | <span data-ttu-id="b582c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b582c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b582c-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="b582c-131">ConsistencyLevel</span></span> | <span data-ttu-id="b582c-132">最终。</span><span class="sxs-lookup"><span data-stu-id="b582c-132">eventual.</span></span> <span data-ttu-id="b582c-133">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="b582c-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="b582c-134">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="b582c-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b582c-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="b582c-135">Request body</span></span>

<span data-ttu-id="b582c-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b582c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b582c-137">响应</span><span class="sxs-lookup"><span data-stu-id="b582c-137">Response</span></span>

<span data-ttu-id="b582c-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b582c-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b582c-139">示例</span><span class="sxs-lookup"><span data-stu-id="b582c-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="b582c-140">示例1：获取设备是其可传递成员的组</span><span class="sxs-lookup"><span data-stu-id="b582c-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="b582c-141">请求</span><span class="sxs-lookup"><span data-stu-id="b582c-141">Request</span></span>

<span data-ttu-id="b582c-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b582c-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b582c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b582c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="b582c-144">C#</span><span class="sxs-lookup"><span data-stu-id="b582c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b582c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b582c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b582c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b582c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b582c-147">Java</span><span class="sxs-lookup"><span data-stu-id="b582c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b582c-148">响应</span><span class="sxs-lookup"><span data-stu-id="b582c-148">Response</span></span>

<span data-ttu-id="b582c-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b582c-149">The following is an example of the response.</span></span>

><span data-ttu-id="b582c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b582c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="b582c-152">示例 2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="b582c-152">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="b582c-153">请求</span><span class="sxs-lookup"><span data-stu-id="b582c-153">Request</span></span>

<span data-ttu-id="b582c-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b582c-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b582c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b582c-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="b582c-156">C#</span><span class="sxs-lookup"><span data-stu-id="b582c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b582c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b582c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b582c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b582c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b582c-159">Java</span><span class="sxs-lookup"><span data-stu-id="b582c-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b582c-160">响应</span><span class="sxs-lookup"><span data-stu-id="b582c-160">Response</span></span>

<span data-ttu-id="b582c-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b582c-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-odata-cast-and-search-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="b582c-162">示例3：使用 OData 强制转换和 $search 获取带有显示名称的组成员身份，其中包含包含所返回对象的计数的字母 "视频"</span><span class="sxs-lookup"><span data-stu-id="b582c-162">Example 3: Use OData cast and $search to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b582c-163">请求</span><span class="sxs-lookup"><span data-stu-id="b582c-163">Request</span></span>

<span data-ttu-id="b582c-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b582c-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b582c-165">响应</span><span class="sxs-lookup"><span data-stu-id="b582c-165">Response</span></span>

<span data-ttu-id="b582c-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b582c-166">The following is an example of the response.</span></span>

><span data-ttu-id="b582c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b582c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b582c-169">示例4：使用 OData 强制转换和 $filter 获取显示名称以 "A" 开头的成员身份，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="b582c-169">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b582c-170">请求</span><span class="sxs-lookup"><span data-stu-id="b582c-170">Request</span></span>

<span data-ttu-id="b582c-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b582c-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b582c-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="b582c-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="b582c-173">C#</span><span class="sxs-lookup"><span data-stu-id="b582c-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b582c-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b582c-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b582c-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b582c-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b582c-176">Java</span><span class="sxs-lookup"><span data-stu-id="b582c-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b582c-177">响应</span><span class="sxs-lookup"><span data-stu-id="b582c-177">Response</span></span>

<span data-ttu-id="b582c-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b582c-178">The following is an example of the response.</span></span>

><span data-ttu-id="b582c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b582c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
