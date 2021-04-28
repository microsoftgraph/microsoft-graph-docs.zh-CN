---
title: 列出设备
description: 检索组织中注册的 device 对象的列表。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8f17537315e97efb99837a9333cf5821818007ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039725"
---
# <a name="list-devices"></a><span data-ttu-id="56cf4-103">列出设备</span><span class="sxs-lookup"><span data-stu-id="56cf4-103">List devices</span></span>

<span data-ttu-id="56cf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56cf4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56cf4-105">检索组织中注册的 device 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="56cf4-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="56cf4-106">权限</span><span class="sxs-lookup"><span data-stu-id="56cf4-106">Permissions</span></span>
<span data-ttu-id="56cf4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="56cf4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="56cf4-109">Permission type</span></span>      | <span data-ttu-id="56cf4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56cf4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56cf4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56cf4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="56cf4-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56cf4-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56cf4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56cf4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56cf4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="56cf4-114">Not supported.</span></span>    |
|<span data-ttu-id="56cf4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="56cf4-115">Application</span></span> | <span data-ttu-id="56cf4-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56cf4-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56cf4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56cf4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56cf4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56cf4-118">Optional query parameters</span></span>

<span data-ttu-id="56cf4-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="56cf4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="56cf4-120">可使用“**displayName**”和“**说明**”属性上的`$search`。</span><span class="sxs-lookup"><span data-stu-id="56cf4-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="56cf4-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="56cf4-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="56cf4-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="56cf4-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56cf4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="56cf4-123">Request headers</span></span>

| <span data-ttu-id="56cf4-124">名称</span><span class="sxs-lookup"><span data-stu-id="56cf4-124">Name</span></span>       |  <span data-ttu-id="56cf4-125">说明</span><span class="sxs-lookup"><span data-stu-id="56cf4-125">Description</span></span>|
|:-----------|:------------|
| <span data-ttu-id="56cf4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="56cf4-126">Authorization</span></span>  | <span data-ttu-id="56cf4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56cf4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56cf4-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="56cf4-129">ConsistencyLevel</span></span> | <span data-ttu-id="56cf4-130">最终。</span><span class="sxs-lookup"><span data-stu-id="56cf4-130">eventual.</span></span> <span data-ttu-id="56cf4-131">当使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，此标头和 `$count` 是必需的。</span><span class="sxs-lookup"><span data-stu-id="56cf4-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="56cf4-132">它使用的索引可能与对象的最新更改不同步。</span><span class="sxs-lookup"><span data-stu-id="56cf4-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56cf4-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="56cf4-133">Request body</span></span>
<span data-ttu-id="56cf4-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56cf4-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56cf4-135">响应</span><span class="sxs-lookup"><span data-stu-id="56cf4-135">Response</span></span>

<span data-ttu-id="56cf4-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="56cf4-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56cf4-137">示例</span><span class="sxs-lookup"><span data-stu-id="56cf4-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="56cf4-138">示例 1：获取设备列表</span><span class="sxs-lookup"><span data-stu-id="56cf4-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="56cf4-139">请求</span><span class="sxs-lookup"><span data-stu-id="56cf4-139">Request</span></span>

<span data-ttu-id="56cf4-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56cf4-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56cf4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="56cf4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="56cf4-142">C#</span><span class="sxs-lookup"><span data-stu-id="56cf4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56cf4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56cf4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56cf4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56cf4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56cf4-145">Java</span><span class="sxs-lookup"><span data-stu-id="56cf4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="56cf4-146">响应</span><span class="sxs-lookup"><span data-stu-id="56cf4-146">Response</span></span>

<span data-ttu-id="56cf4-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56cf4-147">The following is an example of the response.</span></span>

> <span data-ttu-id="56cf4-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="56cf4-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="56cf4-149">示例 2：仅获取设备计数</span><span class="sxs-lookup"><span data-stu-id="56cf4-149">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="56cf4-150">请求</span><span class="sxs-lookup"><span data-stu-id="56cf4-150">Request</span></span>

<span data-ttu-id="56cf4-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56cf4-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="56cf4-152">响应</span><span class="sxs-lookup"><span data-stu-id="56cf4-152">Response</span></span>

<span data-ttu-id="56cf4-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56cf4-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="56cf4-154">示例 3：使用 $filter 和 $top 获取一显示名称以"a"开头的设备，包括返回的对象计数</span><span class="sxs-lookup"><span data-stu-id="56cf4-154">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="56cf4-155">请求</span><span class="sxs-lookup"><span data-stu-id="56cf4-155">Request</span></span>

<span data-ttu-id="56cf4-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56cf4-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="56cf4-157">响应</span><span class="sxs-lookup"><span data-stu-id="56cf4-157">Response</span></span>

<span data-ttu-id="56cf4-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56cf4-158">The following is an example of the response.</span></span>

><span data-ttu-id="56cf4-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="56cf4-159">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="56cf4-160">示例 4：$search获取显示名称包含字母"Android"的设备，包括返回的对象计数</span><span class="sxs-lookup"><span data-stu-id="56cf4-160">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="56cf4-161">请求</span><span class="sxs-lookup"><span data-stu-id="56cf4-161">Request</span></span>

<span data-ttu-id="56cf4-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56cf4-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="56cf4-163">响应</span><span class="sxs-lookup"><span data-stu-id="56cf4-163">Response</span></span>

<span data-ttu-id="56cf4-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56cf4-164">The following is an example of the response.</span></span>

><span data-ttu-id="56cf4-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="56cf4-165">**Note:** The response object shown here might be shortened for readability.</span></span>

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
