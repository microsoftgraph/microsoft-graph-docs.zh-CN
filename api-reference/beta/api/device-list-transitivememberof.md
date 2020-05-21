---
title: 列出设备可传递组
description: 获取设备所属的组。
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab4a13a3ae319847125a5ccbae22913c0be32a9a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333218"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="7e52c-103">列出设备可传递组</span><span class="sxs-lookup"><span data-stu-id="7e52c-103">List device transitive groups</span></span>

<span data-ttu-id="7e52c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e52c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e52c-105">获取设备所属的组。</span><span class="sxs-lookup"><span data-stu-id="7e52c-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="7e52c-106">此 API 请求是可传递的，并且还将返回设备是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="7e52c-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e52c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e52c-107">Permissions</span></span>

<span data-ttu-id="7e52c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e52c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e52c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e52c-110">Permission type</span></span>      | <span data-ttu-id="7e52c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e52c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e52c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e52c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e52c-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e52c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e52c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e52c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e52c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e52c-115">Not supported.</span></span>    |
|<span data-ttu-id="7e52c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e52c-116">Application</span></span> | <span data-ttu-id="7e52c-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e52c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]


## <a name="http-request"></a><span data-ttu-id="7e52c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e52c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e52c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7e52c-119">Optional query parameters</span></span>

<span data-ttu-id="7e52c-120">此方法支持[OData 查询参数](/graph/query_parameters)，以帮助自定义响应，包括 `$search` 、 `$count` 和 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="7e52c-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="7e52c-121">此外，还会启用 OData 强制转换，例如，您可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="7e52c-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="7e52c-122">您可以 `$search` 在**displayName**属性上使用。</span><span class="sxs-lookup"><span data-stu-id="7e52c-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="7e52c-123">为此资源添加或更新项目时，将对其进行专门编制索引，以便 `$count` 与 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="7e52c-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="7e52c-124">在添加或更新项目以及在索引中可用时，可能会出现轻微的延迟。</span><span class="sxs-lookup"><span data-stu-id="7e52c-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e52c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e52c-125">Request headers</span></span>

| <span data-ttu-id="7e52c-126">标头</span><span class="sxs-lookup"><span data-stu-id="7e52c-126">Header</span></span>       | <span data-ttu-id="7e52c-127">值</span><span class="sxs-lookup"><span data-stu-id="7e52c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e52c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e52c-128">Authorization</span></span>  | <span data-ttu-id="7e52c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e52c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7e52c-131">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="7e52c-131">ConsistencyLevel</span></span> | <span data-ttu-id="7e52c-132">仍然.</span><span class="sxs-lookup"><span data-stu-id="7e52c-132">eventual.</span></span> <span data-ttu-id="7e52c-133">在 `$count` 使用 `$search` 、 `$filter` 、 `$orderby` 或 OData 转换查询参数时，此标头和是必需的。</span><span class="sxs-lookup"><span data-stu-id="7e52c-133">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="7e52c-134">它使用的索引可能不是最新的，并包含对对象的最新更改。</span><span class="sxs-lookup"><span data-stu-id="7e52c-134">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e52c-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e52c-135">Request body</span></span>

<span data-ttu-id="7e52c-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7e52c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e52c-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e52c-137">Response</span></span>

<span data-ttu-id="7e52c-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7e52c-138">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e52c-139">示例</span><span class="sxs-lookup"><span data-stu-id="7e52c-139">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-transitive-member-of"></a><span data-ttu-id="7e52c-140">示例1：获取设备是其可传递成员的组</span><span class="sxs-lookup"><span data-stu-id="7e52c-140">Example 1: Get groups that the device is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="7e52c-141">请求</span><span class="sxs-lookup"><span data-stu-id="7e52c-141">Request</span></span>

<span data-ttu-id="7e52c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e52c-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e52c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e52c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="7e52c-144">C#</span><span class="sxs-lookup"><span data-stu-id="7e52c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e52c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e52c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e52c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e52c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e52c-147">响应</span><span class="sxs-lookup"><span data-stu-id="7e52c-147">Response</span></span>

<span data-ttu-id="7e52c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e52c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="7e52c-151">示例2：仅获取所有可传递成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="7e52c-151">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="7e52c-152">请求</span><span class="sxs-lookup"><span data-stu-id="7e52c-152">Request</span></span>

<span data-ttu-id="7e52c-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e52c-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e52c-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e52c-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7e52c-155">C#</span><span class="sxs-lookup"><span data-stu-id="7e52c-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e52c-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e52c-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e52c-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e52c-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e52c-158">响应</span><span class="sxs-lookup"><span data-stu-id="7e52c-158">Response</span></span>

<span data-ttu-id="7e52c-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7e52c-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="7e52c-160">294</span><span class="sxs-lookup"><span data-stu-id="7e52c-160">294</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="7e52c-161">示例3：使用 OData 强制转换和 $search 获取包含包含字母 "视频" 的显示名称的成员资格，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="7e52c-161">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7e52c-162">请求</span><span class="sxs-lookup"><span data-stu-id="7e52c-162">Request</span></span>

<span data-ttu-id="7e52c-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e52c-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e52c-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e52c-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="7e52c-165">C#</span><span class="sxs-lookup"><span data-stu-id="7e52c-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e52c-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e52c-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e52c-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e52c-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e52c-168">响应</span><span class="sxs-lookup"><span data-stu-id="7e52c-168">Response</span></span>

<span data-ttu-id="7e52c-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e52c-169">The following is an example of the response.</span></span>
><span data-ttu-id="7e52c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7e52c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="7e52c-172">示例4：使用 OData 强制转换和 $filter 获取显示名称以 "A" 开头的成员身份，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="7e52c-172">Example 4: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="7e52c-173">请求</span><span class="sxs-lookup"><span data-stu-id="7e52c-173">Request</span></span>

<span data-ttu-id="7e52c-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e52c-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="7e52c-175">响应</span><span class="sxs-lookup"><span data-stu-id="7e52c-175">Response</span></span>

<span data-ttu-id="7e52c-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e52c-176">The following is an example of the response.</span></span>
><span data-ttu-id="7e52c-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7e52c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
