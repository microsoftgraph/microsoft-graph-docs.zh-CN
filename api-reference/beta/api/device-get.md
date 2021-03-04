---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8c1c70578ed95ead160895e5d471a8c4ba56e6c8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437203"
---
# <a name="get-device"></a><span data-ttu-id="14866-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="14866-103">Get device</span></span>

<span data-ttu-id="14866-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14866-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14866-105">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14866-105">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="14866-106">由于 **设备** 资源 [支持扩展](/graph/extensibility-overview)，因此您还可以使用该操作获取设备实例中的自定义属性 `GET` 和 **扩展** 数据。</span><span class="sxs-lookup"><span data-stu-id="14866-106">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="14866-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="14866-107">Permissions</span></span>
<span data-ttu-id="14866-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="14866-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14866-110">Permission type</span></span>      | <span data-ttu-id="14866-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14866-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14866-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14866-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14866-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14866-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14866-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14866-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14866-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14866-115">Not supported.</span></span>    |
|<span data-ttu-id="14866-116">Application</span><span class="sxs-lookup"><span data-stu-id="14866-116">Application</span></span> | <span data-ttu-id="14866-117">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14866-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14866-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14866-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14866-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14866-119">Optional query parameters</span></span>
<span data-ttu-id="14866-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="14866-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14866-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="14866-121">Request headers</span></span>
| <span data-ttu-id="14866-122">名称</span><span class="sxs-lookup"><span data-stu-id="14866-122">Name</span></span>       | <span data-ttu-id="14866-123">类型</span><span class="sxs-lookup"><span data-stu-id="14866-123">Type</span></span> | <span data-ttu-id="14866-124">说明</span><span class="sxs-lookup"><span data-stu-id="14866-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14866-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="14866-125">Authorization</span></span>  | <span data-ttu-id="14866-126">string</span><span class="sxs-lookup"><span data-stu-id="14866-126">string</span></span>  | <span data-ttu-id="14866-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14866-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14866-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="14866-129">Request body</span></span>
<span data-ttu-id="14866-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14866-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14866-131">响应</span><span class="sxs-lookup"><span data-stu-id="14866-131">Response</span></span>

<span data-ttu-id="14866-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14866-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14866-133">示例</span><span class="sxs-lookup"><span data-stu-id="14866-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="14866-134">请求</span><span class="sxs-lookup"><span data-stu-id="14866-134">Request</span></span>
<span data-ttu-id="14866-135">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="14866-135">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14866-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="14866-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="14866-137">C#</span><span class="sxs-lookup"><span data-stu-id="14866-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14866-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14866-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14866-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14866-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14866-140">Java</span><span class="sxs-lookup"><span data-stu-id="14866-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="14866-141">**注意：**`id`请求中的是 **设备的 id** 属性，而不是 **deviceId** 属性。</span><span class="sxs-lookup"><span data-stu-id="14866-141">**Note:** The `id` in the request is the **id** property of the device, not the **deviceId** property.</span></span>

### <a name="response"></a><span data-ttu-id="14866-142">响应</span><span class="sxs-lookup"><span data-stu-id="14866-142">Response</span></span>
<span data-ttu-id="14866-143">以下示例显示没有主机名的设备 **的响应**。</span><span class="sxs-lookup"><span data-stu-id="14866-143">The following example shows a response for a device with no **hostNames**.</span></span> 

><span data-ttu-id="14866-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="14866-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 322

{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99,
  "hostNames": []
}
```

<span data-ttu-id="14866-145">以下示例显示对具有 **hostNames** 的设备的响应。</span><span class="sxs-lookup"><span data-stu-id="14866-145">The following example shows a response for a device with **hostNames**.</span></span> 

><span data-ttu-id="14866-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="14866-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 322

{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99,
  "hostnames":["hostname1.contoso.onmicrosoft.com", "hostname1"]
}
```


## <a name="see-also"></a><span data-ttu-id="14866-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="14866-147">See also</span></span>

- [<span data-ttu-id="14866-148">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="14866-148">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="14866-149">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="14866-149">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="14866-150">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="14866-150">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
