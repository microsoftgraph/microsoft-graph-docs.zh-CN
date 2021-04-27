---
title: 列出设备组
description: 获取此设备是其直接成员组。 此操作不可传递。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b7271f38e11505930cb377cb05399a2e7f93d458
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046977"
---
# <a name="list-device-groups"></a><span data-ttu-id="c93d1-104">列出设备组</span><span class="sxs-lookup"><span data-stu-id="c93d1-104">List device groups</span></span>

<span data-ttu-id="c93d1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c93d1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c93d1-106">获取此设备是其直接成员组。</span><span class="sxs-lookup"><span data-stu-id="c93d1-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="c93d1-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="c93d1-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="c93d1-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c93d1-108">Permissions</span></span>

<span data-ttu-id="c93d1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c93d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c93d1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c93d1-111">Permission type</span></span>      | <span data-ttu-id="c93d1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c93d1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c93d1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c93d1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c93d1-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c93d1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c93d1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c93d1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c93d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c93d1-116">Not supported.</span></span>    |
|<span data-ttu-id="c93d1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c93d1-117">Application</span></span> | <span data-ttu-id="c93d1-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c93d1-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c93d1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c93d1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c93d1-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c93d1-120">Optional query parameters</span></span>

<span data-ttu-id="c93d1-121">此方法支持[OData query parameters](/graph/query_parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="c93d1-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="c93d1-122">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="c93d1-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="c93d1-123">`$search`可以用在 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="c93d1-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="c93d1-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="c93d1-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="c93d1-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="c93d1-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c93d1-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c93d1-126">Request headers</span></span>
| <span data-ttu-id="c93d1-127">标头</span><span class="sxs-lookup"><span data-stu-id="c93d1-127">Header</span></span>       | <span data-ttu-id="c93d1-128">值</span><span class="sxs-lookup"><span data-stu-id="c93d1-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c93d1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c93d1-129">Authorization</span></span>  | <span data-ttu-id="c93d1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c93d1-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c93d1-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="c93d1-132">ConsistencyLevel</span></span> | <span data-ttu-id="c93d1-133">最终。</span><span class="sxs-lookup"><span data-stu-id="c93d1-133">eventual.</span></span> <span data-ttu-id="c93d1-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="c93d1-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="c93d1-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="c93d1-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c93d1-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="c93d1-136">Request body</span></span>
<span data-ttu-id="c93d1-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c93d1-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c93d1-138">响应</span><span class="sxs-lookup"><span data-stu-id="c93d1-138">Response</span></span>

<span data-ttu-id="c93d1-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c93d1-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c93d1-140">示例</span><span class="sxs-lookup"><span data-stu-id="c93d1-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="c93d1-141">示例 1：获取设备是其直接成员</span><span class="sxs-lookup"><span data-stu-id="c93d1-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="c93d1-142">请求</span><span class="sxs-lookup"><span data-stu-id="c93d1-142">Request</span></span>

<span data-ttu-id="c93d1-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c93d1-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c93d1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c93d1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="c93d1-145">C#</span><span class="sxs-lookup"><span data-stu-id="c93d1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c93d1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c93d1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c93d1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c93d1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c93d1-148">Java</span><span class="sxs-lookup"><span data-stu-id="c93d1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c93d1-149">响应</span><span class="sxs-lookup"><span data-stu-id="c93d1-149">Response</span></span>

<span data-ttu-id="c93d1-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c93d1-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="c93d1-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c93d1-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="c93d1-152">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="c93d1-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="c93d1-153">请求</span><span class="sxs-lookup"><span data-stu-id="c93d1-153">Request</span></span>

<span data-ttu-id="c93d1-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c93d1-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c93d1-155">响应</span><span class="sxs-lookup"><span data-stu-id="c93d1-155">Response</span></span>

<span data-ttu-id="c93d1-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c93d1-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="c93d1-157">394</span><span class="sxs-lookup"><span data-stu-id="c93d1-157">394</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="c93d1-158">示例 3：使用 OData 转换和$search获取包含字母"Video"的显示名称（包括返回的对象计数）的成员资格</span><span class="sxs-lookup"><span data-stu-id="c93d1-158">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c93d1-159">请求</span><span class="sxs-lookup"><span data-stu-id="c93d1-159">Request</span></span>

<span data-ttu-id="c93d1-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c93d1-160">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c93d1-161">响应</span><span class="sxs-lookup"><span data-stu-id="c93d1-161">Response</span></span>

<span data-ttu-id="c93d1-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c93d1-162">The following is an example of the response.</span></span>
><span data-ttu-id="c93d1-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c93d1-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="c93d1-164">示例 4：使用 OData 转换$filter获取以字母"A"开头显示名称（包括返回的对象计数）的组成员身份</span><span class="sxs-lookup"><span data-stu-id="c93d1-164">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="c93d1-165">请求</span><span class="sxs-lookup"><span data-stu-id="c93d1-165">Request</span></span>

<span data-ttu-id="c93d1-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c93d1-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="c93d1-167">响应</span><span class="sxs-lookup"><span data-stu-id="c93d1-167">Response</span></span>

<span data-ttu-id="c93d1-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c93d1-168">The following is an example of the response.</span></span>
><span data-ttu-id="c93d1-169">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c93d1-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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


