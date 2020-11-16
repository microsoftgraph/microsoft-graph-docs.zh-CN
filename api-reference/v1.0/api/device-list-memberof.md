---
title: 列出设备组
description: 获取此设备是其直接成员的组。 此操作不可传递。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69e33afef9dba54785dd7b5ea3af5285f4aa37ad
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082074"
---
# <a name="list-device-groups"></a><span data-ttu-id="89a08-104">列出设备组</span><span class="sxs-lookup"><span data-stu-id="89a08-104">List device groups</span></span>

<span data-ttu-id="89a08-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89a08-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89a08-106">获取此设备是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="89a08-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="89a08-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="89a08-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="89a08-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="89a08-108">Permissions</span></span>

<span data-ttu-id="89a08-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89a08-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89a08-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89a08-111">Permission type</span></span>      | <span data-ttu-id="89a08-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89a08-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89a08-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89a08-113">Delegated (work or school account)</span></span> | <span data-ttu-id="89a08-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="89a08-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89a08-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89a08-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89a08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89a08-116">Not supported.</span></span>    |
|<span data-ttu-id="89a08-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89a08-117">Application</span></span> | <span data-ttu-id="89a08-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89a08-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="89a08-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89a08-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89a08-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="89a08-120">Optional query parameters</span></span>

<span data-ttu-id="89a08-121">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="89a08-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="89a08-122">还启用了 OData 强制转换，例如，你可以强制转换为仅获取用户所属的 directoryRoles。</span><span class="sxs-lookup"><span data-stu-id="89a08-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="89a08-123">可使用“ **displayName** ”和“ **说明** ”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="89a08-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="89a08-124">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="89a08-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="89a08-125">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="89a08-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89a08-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="89a08-126">Request headers</span></span>

| <span data-ttu-id="89a08-127">标头</span><span class="sxs-lookup"><span data-stu-id="89a08-127">Header</span></span>       | <span data-ttu-id="89a08-128">值</span><span class="sxs-lookup"><span data-stu-id="89a08-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89a08-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="89a08-129">Authorization</span></span>  | <span data-ttu-id="89a08-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89a08-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="89a08-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="89a08-132">ConsistencyLevel</span></span> | <span data-ttu-id="89a08-133">最终。</span><span class="sxs-lookup"><span data-stu-id="89a08-133">eventual.</span></span> <span data-ttu-id="89a08-134">使用 `$search`、`$filter`、`$orderby` 或 OData 强制转换查询参数时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="89a08-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="89a08-135">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="89a08-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89a08-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="89a08-136">Request body</span></span>
<span data-ttu-id="89a08-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89a08-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89a08-138">响应</span><span class="sxs-lookup"><span data-stu-id="89a08-138">Response</span></span>

<span data-ttu-id="89a08-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="89a08-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89a08-140">示例</span><span class="sxs-lookup"><span data-stu-id="89a08-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="89a08-141">示例1：获取设备是其直接成员的组</span><span class="sxs-lookup"><span data-stu-id="89a08-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="89a08-142">请求</span><span class="sxs-lookup"><span data-stu-id="89a08-142">Request</span></span>

<span data-ttu-id="89a08-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89a08-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89a08-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="89a08-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="89a08-145">C#</span><span class="sxs-lookup"><span data-stu-id="89a08-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89a08-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89a08-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89a08-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89a08-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89a08-148">Java</span><span class="sxs-lookup"><span data-stu-id="89a08-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="89a08-149">响应</span><span class="sxs-lookup"><span data-stu-id="89a08-149">Response</span></span>

<span data-ttu-id="89a08-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89a08-150">The following is an example of the response.</span></span> 

> <span data-ttu-id="89a08-151">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89a08-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="89a08-152">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89a08-152">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="89a08-153">示例 2：仅获取所有可成员身份的计数</span><span class="sxs-lookup"><span data-stu-id="89a08-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="89a08-154">请求</span><span class="sxs-lookup"><span data-stu-id="89a08-154">Request</span></span>

<span data-ttu-id="89a08-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89a08-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="89a08-156">响应</span><span class="sxs-lookup"><span data-stu-id="89a08-156">Response</span></span>

<span data-ttu-id="89a08-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89a08-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="89a08-158">示例3：使用 OData 强制转换和 $search 获取包含包含字母 "视频" 的显示名称的成员资格，包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="89a08-158">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="89a08-159">请求</span><span class="sxs-lookup"><span data-stu-id="89a08-159">Request</span></span>

<span data-ttu-id="89a08-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89a08-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="89a08-161">响应</span><span class="sxs-lookup"><span data-stu-id="89a08-161">Response</span></span>

<span data-ttu-id="89a08-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89a08-162">The following is an example of the response.</span></span>

><span data-ttu-id="89a08-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89a08-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="89a08-165">示例4：使用 OData 强制转换和 $filter 获取显示名称以字母 "A" 开头的成员，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="89a08-165">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="89a08-166">请求</span><span class="sxs-lookup"><span data-stu-id="89a08-166">Request</span></span>

<span data-ttu-id="89a08-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89a08-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="89a08-168">响应</span><span class="sxs-lookup"><span data-stu-id="89a08-168">Response</span></span>

<span data-ttu-id="89a08-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89a08-169">The following is an example of the response.</span></span>

><span data-ttu-id="89a08-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89a08-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
}-->
