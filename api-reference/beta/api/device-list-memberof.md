---
title: 列出设备组
description: 获取此设备是其直接成员组的组。 此操作不可传递。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d37036734e1e00d8130612528ee90305c3986476
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437196"
---
# <a name="list-device-groups"></a><span data-ttu-id="9a6eb-104">列出设备组</span><span class="sxs-lookup"><span data-stu-id="9a6eb-104">List device groups</span></span>

<span data-ttu-id="9a6eb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a6eb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a6eb-106">获取此设备是其直接成员组的组。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="9a6eb-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a6eb-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="9a6eb-108">Permissions</span></span>

<span data-ttu-id="9a6eb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a6eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a6eb-111">Permission type</span></span>      | <span data-ttu-id="9a6eb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a6eb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a6eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a6eb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9a6eb-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a6eb-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a6eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a6eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a6eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-116">Not supported.</span></span>    |
|<span data-ttu-id="9a6eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a6eb-117">Application</span></span> | <span data-ttu-id="9a6eb-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a6eb-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="9a6eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a6eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a6eb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9a6eb-120">Optional query parameters</span></span>

<span data-ttu-id="9a6eb-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="9a6eb-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="9a6eb-122">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="9a6eb-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="9a6eb-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="9a6eb-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a6eb-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a6eb-126">Request headers</span></span>
| <span data-ttu-id="9a6eb-127">标头</span><span class="sxs-lookup"><span data-stu-id="9a6eb-127">Header</span></span>       | <span data-ttu-id="9a6eb-128">值</span><span class="sxs-lookup"><span data-stu-id="9a6eb-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a6eb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a6eb-129">Authorization</span></span>  | <span data-ttu-id="9a6eb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9a6eb-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="9a6eb-132">ConsistencyLevel</span></span> | <span data-ttu-id="9a6eb-133">最终。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-133">eventual.</span></span> <span data-ttu-id="9a6eb-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="9a6eb-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a6eb-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a6eb-136">Request body</span></span>
<span data-ttu-id="9a6eb-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a6eb-138">响应</span><span class="sxs-lookup"><span data-stu-id="9a6eb-138">Response</span></span>

<span data-ttu-id="9a6eb-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a6eb-140">示例</span><span class="sxs-lookup"><span data-stu-id="9a6eb-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="9a6eb-141">示例 1：获取设备是其直接成员</span><span class="sxs-lookup"><span data-stu-id="9a6eb-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="9a6eb-142">请求</span><span class="sxs-lookup"><span data-stu-id="9a6eb-142">Request</span></span>

<span data-ttu-id="9a6eb-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a6eb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a6eb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="9a6eb-145">C#</span><span class="sxs-lookup"><span data-stu-id="9a6eb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a6eb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a6eb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a6eb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a6eb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a6eb-148">Java</span><span class="sxs-lookup"><span data-stu-id="9a6eb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a6eb-149">响应</span><span class="sxs-lookup"><span data-stu-id="9a6eb-149">Response</span></span>

<span data-ttu-id="9a6eb-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="9a6eb-151">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9a6eb-152">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-152">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="9a6eb-153">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="9a6eb-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="9a6eb-154">请求</span><span class="sxs-lookup"><span data-stu-id="9a6eb-154">Request</span></span>

<span data-ttu-id="9a6eb-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9a6eb-156">响应</span><span class="sxs-lookup"><span data-stu-id="9a6eb-156">Response</span></span>

<span data-ttu-id="9a6eb-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="9a6eb-158">394</span><span class="sxs-lookup"><span data-stu-id="9a6eb-158">394</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="9a6eb-159">示例 3：使用 OData 转换和$search获取显示名称的成员资格，这些显示名称包含字母"Video"（包括返回的对象数）</span><span class="sxs-lookup"><span data-stu-id="9a6eb-159">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9a6eb-160">请求</span><span class="sxs-lookup"><span data-stu-id="9a6eb-160">Request</span></span>

<span data-ttu-id="9a6eb-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-161">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9a6eb-162">响应</span><span class="sxs-lookup"><span data-stu-id="9a6eb-162">Response</span></span>

<span data-ttu-id="9a6eb-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-163">The following is an example of the response.</span></span>
><span data-ttu-id="9a6eb-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="9a6eb-166">示例 4：使用 OData 转换和$filter获取以字母"A"开头的 显示名称 的成员资格，其中包括返回的对象数</span><span class="sxs-lookup"><span data-stu-id="9a6eb-166">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="9a6eb-167">请求</span><span class="sxs-lookup"><span data-stu-id="9a6eb-167">Request</span></span>

<span data-ttu-id="9a6eb-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="9a6eb-169">响应</span><span class="sxs-lookup"><span data-stu-id="9a6eb-169">Response</span></span>

<span data-ttu-id="9a6eb-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-170">The following is an example of the response.</span></span>
><span data-ttu-id="9a6eb-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9a6eb-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


