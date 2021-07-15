---
title: 列出设备
description: '检索目录中的注册设备列表。 '
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a045c9459a465eed05d35ecb63f4045ba71602de
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430058"
---
# <a name="list-devices"></a><span data-ttu-id="45c23-103">列出设备</span><span class="sxs-lookup"><span data-stu-id="45c23-103">List devices</span></span>

<span data-ttu-id="45c23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45c23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45c23-105">检索目录中的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="45c23-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="45c23-106">权限</span><span class="sxs-lookup"><span data-stu-id="45c23-106">Permissions</span></span>

<span data-ttu-id="45c23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45c23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="45c23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45c23-109">Permission type</span></span> | <span data-ttu-id="45c23-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45c23-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="45c23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45c23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45c23-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45c23-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="45c23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45c23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45c23-114">Not supported.</span></span> |
| <span data-ttu-id="45c23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45c23-115">Application</span></span> | <span data-ttu-id="45c23-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c23-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45c23-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45c23-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45c23-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="45c23-118">Optional query parameters</span></span>

<span data-ttu-id="45c23-119">此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="45c23-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="45c23-120">只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。</span><span class="sxs-lookup"><span data-stu-id="45c23-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="45c23-121">有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="45c23-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="45c23-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="45c23-122">Request headers</span></span>

| <span data-ttu-id="45c23-123">名称</span><span class="sxs-lookup"><span data-stu-id="45c23-123">Name</span></span> | <span data-ttu-id="45c23-124">说明</span><span class="sxs-lookup"><span data-stu-id="45c23-124">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="45c23-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="45c23-125">Authorization</span></span>  | <span data-ttu-id="45c23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45c23-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45c23-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="45c23-128">ConsistencyLevel</span></span> | <span data-ttu-id="45c23-129">最终。</span><span class="sxs-lookup"><span data-stu-id="45c23-129">eventual.</span></span> <span data-ttu-id="45c23-130">当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。</span><span class="sxs-lookup"><span data-stu-id="45c23-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="45c23-131">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="45c23-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="45c23-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="45c23-132">Request body</span></span>

<span data-ttu-id="45c23-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45c23-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45c23-134">响应</span><span class="sxs-lookup"><span data-stu-id="45c23-134">Response</span></span>

<span data-ttu-id="45c23-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="45c23-135">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45c23-136">示例</span><span class="sxs-lookup"><span data-stu-id="45c23-136">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="45c23-137">示例 1：获取设备列表</span><span class="sxs-lookup"><span data-stu-id="45c23-137">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="45c23-138">请求</span><span class="sxs-lookup"><span data-stu-id="45c23-138">Request</span></span>

<span data-ttu-id="45c23-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45c23-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45c23-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="45c23-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="45c23-141">C#</span><span class="sxs-lookup"><span data-stu-id="45c23-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45c23-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45c23-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45c23-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45c23-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45c23-144">Java</span><span class="sxs-lookup"><span data-stu-id="45c23-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="45c23-145">响应</span><span class="sxs-lookup"><span data-stu-id="45c23-145">Response</span></span>

<span data-ttu-id="45c23-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="45c23-146">Here is an example of the response.</span></span>
> <span data-ttu-id="45c23-147">注意：为了提高可读性，可能缩短此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="45c23-147">Note: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="45c23-148">示例 2：仅获取设备计数</span><span class="sxs-lookup"><span data-stu-id="45c23-148">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="45c23-149">请求</span><span class="sxs-lookup"><span data-stu-id="45c23-149">Request</span></span>

<span data-ttu-id="45c23-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45c23-150">The following is an example of the request.</span></span> <span data-ttu-id="45c23-151">此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。</span><span class="sxs-lookup"><span data-stu-id="45c23-151">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="45c23-152">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="45c23-152">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="45c23-153">响应</span><span class="sxs-lookup"><span data-stu-id="45c23-153">Response</span></span>

<span data-ttu-id="45c23-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45c23-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="45c23-155">294</span><span class="sxs-lookup"><span data-stu-id="45c23-155">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="45c23-156">示例 3：使用 $filter 和 $top 获取一显示名称以"a"开头的设备，包括返回的对象计数</span><span class="sxs-lookup"><span data-stu-id="45c23-156">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="45c23-157">请求</span><span class="sxs-lookup"><span data-stu-id="45c23-157">Request</span></span>

<span data-ttu-id="45c23-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45c23-158">The following is an example of the request.</span></span> <span data-ttu-id="45c23-159">此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="45c23-159">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="45c23-160">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="45c23-160">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="45c23-161">响应</span><span class="sxs-lookup"><span data-stu-id="45c23-161">Response</span></span>

<span data-ttu-id="45c23-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45c23-162">The following is an example of the response.</span></span>
><span data-ttu-id="45c23-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="45c23-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0",
      "hostNames":[]
    },
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000001",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Microsoft",
      "Model":"Surface",
      "operatingSystemVersion":"windows10EnterpriseN",
      "hostNames":["device_1.contoso.onmicrosoft.com", "device_1"]
    }
  ]
}
```

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="45c23-164">示例 4：$search获取显示名称包含字母"Android"的设备，包括返回的对象计数</span><span class="sxs-lookup"><span data-stu-id="45c23-164">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="45c23-165">请求</span><span class="sxs-lookup"><span data-stu-id="45c23-165">Request</span></span>

<span data-ttu-id="45c23-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45c23-166">The following is an example of the request.</span></span> <span data-ttu-id="45c23-167">此请求需要 **将 ConsistencyLevel** 标头设置为 `eventual` ，因为 `$search` 查询 `$count=true` 字符串位于请求中。</span><span class="sxs-lookup"><span data-stu-id="45c23-167">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="45c23-168">有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。</span><span class="sxs-lookup"><span data-stu-id="45c23-168">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>


<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="45c23-169">响应</span><span class="sxs-lookup"><span data-stu-id="45c23-169">Response</span></span>

<span data-ttu-id="45c23-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45c23-170">The following is an example of the response.</span></span>
><span data-ttu-id="45c23-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="45c23-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0",
      "hostNames":[]
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
}
-->


