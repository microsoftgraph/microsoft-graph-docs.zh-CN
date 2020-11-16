---
title: 列出设备
description: '检索目录中的注册设备列表。 '
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d0fe2403e04751a734da726d6f4c2cb6890813a
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082011"
---
# <a name="list-devices"></a><span data-ttu-id="5c0a7-103">列出设备</span><span class="sxs-lookup"><span data-stu-id="5c0a7-103">List devices</span></span>

<span data-ttu-id="5c0a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c0a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c0a7-105">检索目录中的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5c0a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="5c0a7-106">Permissions</span></span>

<span data-ttu-id="5c0a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="5c0a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c0a7-109">Permission type</span></span> | <span data-ttu-id="5c0a7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c0a7-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="5c0a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c0a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c0a7-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c0a7-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="5c0a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c0a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c0a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-114">Not supported.</span></span> |
| <span data-ttu-id="5c0a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c0a7-115">Application</span></span> | <span data-ttu-id="5c0a7-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c0a7-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c0a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c0a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c0a7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c0a7-118">Optional query parameters</span></span>

<span data-ttu-id="5c0a7-p102">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应，包括 `$search`、`$count` 和 `$filter`。你可以在 **displayName** 属性上使用 `$search`。为该资源添加或更新项目时，将为它们专门创建索引，以与 `$count` 和 `$search` 查询参数一起使用。添加或更新项目与项目在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-p102">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`. You can use `$search` on the **displayName** property. When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters. There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c0a7-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c0a7-123">Request headers</span></span>

| <span data-ttu-id="5c0a7-124">名称</span><span class="sxs-lookup"><span data-stu-id="5c0a7-124">Name</span></span> | <span data-ttu-id="5c0a7-125">说明</span><span class="sxs-lookup"><span data-stu-id="5c0a7-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="5c0a7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c0a7-126">Authorization</span></span>  | <span data-ttu-id="5c0a7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c0a7-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="5c0a7-129">ConsistencyLevel</span></span> | <span data-ttu-id="5c0a7-p104">最终。使用 `$search` 或将 `$filter` 与 `$orderby` 查询参数一起使用时，必须提供此标头和 `$count`。它使用的索引可能未根据该对象的最新更改及时更新。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-p104">eventual. This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter. It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c0a7-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c0a7-133">Request body</span></span>

<span data-ttu-id="5c0a7-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c0a7-135">响应</span><span class="sxs-lookup"><span data-stu-id="5c0a7-135">Response</span></span>

<span data-ttu-id="5c0a7-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c0a7-137">示例</span><span class="sxs-lookup"><span data-stu-id="5c0a7-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="5c0a7-138">示例1：获取设备列表</span><span class="sxs-lookup"><span data-stu-id="5c0a7-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="5c0a7-139">请求</span><span class="sxs-lookup"><span data-stu-id="5c0a7-139">Request</span></span>

<span data-ttu-id="5c0a7-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c0a7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0a7-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="5c0a7-142">C#</span><span class="sxs-lookup"><span data-stu-id="5c0a7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c0a7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c0a7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c0a7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c0a7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c0a7-145">Java</span><span class="sxs-lookup"><span data-stu-id="5c0a7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5c0a7-146">响应</span><span class="sxs-lookup"><span data-stu-id="5c0a7-146">Response</span></span>

<span data-ttu-id="5c0a7-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-147">Here is an example of the response.</span></span>
> <span data-ttu-id="5c0a7-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="5c0a7-150">示例2：仅获取设备计数</span><span class="sxs-lookup"><span data-stu-id="5c0a7-150">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="5c0a7-151">请求</span><span class="sxs-lookup"><span data-stu-id="5c0a7-151">Request</span></span>

<span data-ttu-id="5c0a7-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5c0a7-153">响应</span><span class="sxs-lookup"><span data-stu-id="5c0a7-153">Response</span></span>

<span data-ttu-id="5c0a7-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="5c0a7-155">294</span><span class="sxs-lookup"><span data-stu-id="5c0a7-155">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="5c0a7-156">示例3：使用 $filter 和 $top 获取一个显示名称以 ' a ' 开头的设备，其中包含返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="5c0a7-156">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5c0a7-157">请求</span><span class="sxs-lookup"><span data-stu-id="5c0a7-157">Request</span></span>

<span data-ttu-id="5c0a7-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5c0a7-159">响应</span><span class="sxs-lookup"><span data-stu-id="5c0a7-159">Response</span></span>

<span data-ttu-id="5c0a7-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-160">The following is an example of the response.</span></span>
><span data-ttu-id="5c0a7-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="5c0a7-163">示例4：使用 $search 获取显示名称包含字母 "Android" 的设备，其中包括返回对象的计数</span><span class="sxs-lookup"><span data-stu-id="5c0a7-163">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5c0a7-164">请求</span><span class="sxs-lookup"><span data-stu-id="5c0a7-164">Request</span></span>

<span data-ttu-id="5c0a7-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5c0a7-166">响应</span><span class="sxs-lookup"><span data-stu-id="5c0a7-166">Response</span></span>

<span data-ttu-id="5c0a7-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-167">The following is an example of the response.</span></span>
><span data-ttu-id="5c0a7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5c0a7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
}
-->


