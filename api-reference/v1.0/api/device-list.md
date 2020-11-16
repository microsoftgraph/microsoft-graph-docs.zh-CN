---
title: 列出设备
description: 检索组织中注册的 device 对象的列表。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 14ef2993f6dd7766846bb006d047cd4e2f90c615
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082230"
---
# <a name="list-devices"></a><span data-ttu-id="77d27-103">列出设备</span><span class="sxs-lookup"><span data-stu-id="77d27-103">List devices</span></span>

<span data-ttu-id="77d27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77d27-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77d27-105">检索组织中注册的 device 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="77d27-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="77d27-106">权限</span><span class="sxs-lookup"><span data-stu-id="77d27-106">Permissions</span></span>
<span data-ttu-id="77d27-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="77d27-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="77d27-109">Permission type</span></span>      | <span data-ttu-id="77d27-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77d27-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77d27-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77d27-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77d27-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77d27-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77d27-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77d27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77d27-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="77d27-114">Not supported.</span></span>    |
|<span data-ttu-id="77d27-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="77d27-115">Application</span></span> | <span data-ttu-id="77d27-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d27-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77d27-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77d27-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77d27-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77d27-118">Optional query parameters</span></span>

<span data-ttu-id="77d27-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="77d27-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="77d27-120">可使用“ **displayName** ”和“ **说明** ”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="77d27-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="77d27-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="77d27-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="77d27-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="77d27-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77d27-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="77d27-123">Request headers</span></span>

| <span data-ttu-id="77d27-124">名称</span><span class="sxs-lookup"><span data-stu-id="77d27-124">Name</span></span>       |  <span data-ttu-id="77d27-125">说明</span><span class="sxs-lookup"><span data-stu-id="77d27-125">Description</span></span>|
|:-----------|:------------|
| <span data-ttu-id="77d27-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="77d27-126">Authorization</span></span>  | <span data-ttu-id="77d27-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77d27-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77d27-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="77d27-129">ConsistencyLevel</span></span> | <span data-ttu-id="77d27-p104">最终。使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="77d27-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77d27-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="77d27-133">Request body</span></span>
<span data-ttu-id="77d27-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77d27-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77d27-135">响应</span><span class="sxs-lookup"><span data-stu-id="77d27-135">Response</span></span>

<span data-ttu-id="77d27-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77d27-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77d27-137">示例</span><span class="sxs-lookup"><span data-stu-id="77d27-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="77d27-138">示例1：获取设备列表</span><span class="sxs-lookup"><span data-stu-id="77d27-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="77d27-139">请求</span><span class="sxs-lookup"><span data-stu-id="77d27-139">Request</span></span>

<span data-ttu-id="77d27-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77d27-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77d27-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="77d27-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="77d27-142">C#</span><span class="sxs-lookup"><span data-stu-id="77d27-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77d27-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77d27-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77d27-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77d27-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77d27-145">Java</span><span class="sxs-lookup"><span data-stu-id="77d27-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="77d27-146">响应</span><span class="sxs-lookup"><span data-stu-id="77d27-146">Response</span></span>

<span data-ttu-id="77d27-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77d27-147">The following is an example of the response.</span></span>

> <span data-ttu-id="77d27-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="77d27-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="77d27-150">示例2：仅获取设备计数</span><span class="sxs-lookup"><span data-stu-id="77d27-150">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="77d27-151">请求</span><span class="sxs-lookup"><span data-stu-id="77d27-151">Request</span></span>

<span data-ttu-id="77d27-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77d27-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="77d27-153">响应</span><span class="sxs-lookup"><span data-stu-id="77d27-153">Response</span></span>

<span data-ttu-id="77d27-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77d27-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="77d27-155">示例3：使用 $filter 和 $top 获取一个显示名称以 ' a ' 开头的设备，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="77d27-155">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="77d27-156">请求</span><span class="sxs-lookup"><span data-stu-id="77d27-156">Request</span></span>

<span data-ttu-id="77d27-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77d27-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="77d27-158">响应</span><span class="sxs-lookup"><span data-stu-id="77d27-158">Response</span></span>

<span data-ttu-id="77d27-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77d27-159">The following is an example of the response.</span></span>

><span data-ttu-id="77d27-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="77d27-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="77d27-162">示例4：使用 $search 获取显示名称包含字母 "Android" 的设备，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="77d27-162">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="77d27-163">请求</span><span class="sxs-lookup"><span data-stu-id="77d27-163">Request</span></span>

<span data-ttu-id="77d27-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77d27-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="77d27-165">响应</span><span class="sxs-lookup"><span data-stu-id="77d27-165">Response</span></span>

<span data-ttu-id="77d27-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77d27-166">The following is an example of the response.</span></span>

><span data-ttu-id="77d27-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="77d27-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- 
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
