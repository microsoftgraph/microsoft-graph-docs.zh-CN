---
title: 列出设备组
description: 获取此设备是其直接成员的组。 此操作不可传递。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6b869a51b0c81e2d80bd46da82fac69bf540fd1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956413"
---
# <a name="list-device-groups"></a><span data-ttu-id="adbc2-104">列出设备组</span><span class="sxs-lookup"><span data-stu-id="adbc2-104">List device groups</span></span>

<span data-ttu-id="adbc2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adbc2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adbc2-106">获取此设备是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="adbc2-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="adbc2-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="adbc2-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="adbc2-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="adbc2-108">Permissions</span></span>

<span data-ttu-id="adbc2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adbc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adbc2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="adbc2-111">Permission type</span></span>      | <span data-ttu-id="adbc2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adbc2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adbc2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adbc2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="adbc2-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="adbc2-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="adbc2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adbc2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adbc2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="adbc2-116">Not supported.</span></span>    |
|<span data-ttu-id="adbc2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="adbc2-117">Application</span></span> | <span data-ttu-id="adbc2-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbc2-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="adbc2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adbc2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="adbc2-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="adbc2-120">Optional query parameters</span></span>

<span data-ttu-id="adbc2-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="adbc2-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="adbc2-122">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="adbc2-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="adbc2-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="adbc2-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="adbc2-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="adbc2-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="adbc2-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="adbc2-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="adbc2-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="adbc2-126">Request headers</span></span>
| <span data-ttu-id="adbc2-127">标头</span><span class="sxs-lookup"><span data-stu-id="adbc2-127">Header</span></span>       | <span data-ttu-id="adbc2-128">值</span><span class="sxs-lookup"><span data-stu-id="adbc2-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="adbc2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="adbc2-129">Authorization</span></span>  | <span data-ttu-id="adbc2-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="adbc2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="adbc2-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="adbc2-132">ConsistencyLevel</span></span> | <span data-ttu-id="adbc2-133">最终。</span><span class="sxs-lookup"><span data-stu-id="adbc2-133">eventual.</span></span> <span data-ttu-id="adbc2-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="adbc2-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="adbc2-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="adbc2-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adbc2-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="adbc2-136">Request body</span></span>
<span data-ttu-id="adbc2-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="adbc2-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adbc2-138">响应</span><span class="sxs-lookup"><span data-stu-id="adbc2-138">Response</span></span>

<span data-ttu-id="adbc2-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="adbc2-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adbc2-140">示例</span><span class="sxs-lookup"><span data-stu-id="adbc2-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="adbc2-141">示例1：获取设备是其直接成员的组</span><span class="sxs-lookup"><span data-stu-id="adbc2-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="adbc2-142">请求</span><span class="sxs-lookup"><span data-stu-id="adbc2-142">Request</span></span>

<span data-ttu-id="adbc2-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adbc2-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adbc2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbc2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="adbc2-145">C#</span><span class="sxs-lookup"><span data-stu-id="adbc2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbc2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbc2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbc2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbc2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbc2-148">Java</span><span class="sxs-lookup"><span data-stu-id="adbc2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="adbc2-149">响应</span><span class="sxs-lookup"><span data-stu-id="adbc2-149">Response</span></span>

<span data-ttu-id="adbc2-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adbc2-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="adbc2-151">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="adbc2-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="adbc2-152">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adbc2-152">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="adbc2-153">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="adbc2-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="adbc2-154">请求</span><span class="sxs-lookup"><span data-stu-id="adbc2-154">Request</span></span>

<span data-ttu-id="adbc2-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adbc2-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adbc2-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbc2-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="adbc2-157">C#</span><span class="sxs-lookup"><span data-stu-id="adbc2-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbc2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbc2-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbc2-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbc2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbc2-160">Java</span><span class="sxs-lookup"><span data-stu-id="adbc2-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="adbc2-161">响应</span><span class="sxs-lookup"><span data-stu-id="adbc2-161">Response</span></span>

<span data-ttu-id="adbc2-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adbc2-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="adbc2-163">394</span><span class="sxs-lookup"><span data-stu-id="adbc2-163">394</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="adbc2-164">示例3：使用 OData 强制转换和 $search 获取包含包含字母 "视频" 的显示名称的成员资格，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="adbc2-164">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="adbc2-165">请求</span><span class="sxs-lookup"><span data-stu-id="adbc2-165">Request</span></span>

<span data-ttu-id="adbc2-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adbc2-166">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="adbc2-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbc2-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="adbc2-168">C#</span><span class="sxs-lookup"><span data-stu-id="adbc2-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbc2-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbc2-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbc2-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbc2-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="adbc2-171">响应</span><span class="sxs-lookup"><span data-stu-id="adbc2-171">Response</span></span>

<span data-ttu-id="adbc2-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adbc2-172">The following is an example of the response.</span></span>
><span data-ttu-id="adbc2-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="adbc2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="adbc2-175">示例4：使用 OData 强制转换和 $filter 获取显示名称以字母 "A" 开头的成员，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="adbc2-175">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="adbc2-176">请求</span><span class="sxs-lookup"><span data-stu-id="adbc2-176">Request</span></span>

<span data-ttu-id="adbc2-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adbc2-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adbc2-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="adbc2-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="adbc2-179">C#</span><span class="sxs-lookup"><span data-stu-id="adbc2-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adbc2-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adbc2-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adbc2-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adbc2-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adbc2-182">Java</span><span class="sxs-lookup"><span data-stu-id="adbc2-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="adbc2-183">响应</span><span class="sxs-lookup"><span data-stu-id="adbc2-183">Response</span></span>

<span data-ttu-id="adbc2-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adbc2-184">The following is an example of the response.</span></span>
><span data-ttu-id="adbc2-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="adbc2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName":"AAD Contoso Videos",
      "mail":"AADContosoVideos@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Videos",
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


