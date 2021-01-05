---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 762d26f8f339037a6a6031f44efe3cf219a03998
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752974"
---
# <a name="get-device"></a><span data-ttu-id="88524-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="88524-103">Get device</span></span>

<span data-ttu-id="88524-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88524-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88524-105">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88524-105">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="88524-106">由于 **设备** 资源 [支持扩展](/graph/extensibility-overview)，因此，您还可以使用该操作获取设备实例中的自定义属性 `GET` 和 **扩展** 数据。</span><span class="sxs-lookup"><span data-stu-id="88524-106">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="88524-107">权限</span><span class="sxs-lookup"><span data-stu-id="88524-107">Permissions</span></span>
<span data-ttu-id="88524-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88524-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88524-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="88524-110">Permission type</span></span>      | <span data-ttu-id="88524-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88524-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88524-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88524-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88524-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88524-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88524-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88524-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88524-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="88524-115">Not supported.</span></span>    |
|<span data-ttu-id="88524-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="88524-116">Application</span></span> | <span data-ttu-id="88524-117">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88524-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88524-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88524-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88524-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88524-119">Optional query parameters</span></span>
<span data-ttu-id="88524-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="88524-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="88524-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="88524-121">Request headers</span></span>
| <span data-ttu-id="88524-122">名称</span><span class="sxs-lookup"><span data-stu-id="88524-122">Name</span></span>       | <span data-ttu-id="88524-123">类型</span><span class="sxs-lookup"><span data-stu-id="88524-123">Type</span></span> | <span data-ttu-id="88524-124">说明</span><span class="sxs-lookup"><span data-stu-id="88524-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="88524-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="88524-125">Authorization</span></span>  | <span data-ttu-id="88524-126">string</span><span class="sxs-lookup"><span data-stu-id="88524-126">string</span></span>  | <span data-ttu-id="88524-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88524-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88524-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="88524-129">Request body</span></span>
<span data-ttu-id="88524-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88524-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88524-131">响应</span><span class="sxs-lookup"><span data-stu-id="88524-131">Response</span></span>

<span data-ttu-id="88524-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88524-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88524-133">示例</span><span class="sxs-lookup"><span data-stu-id="88524-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="88524-134">请求</span><span class="sxs-lookup"><span data-stu-id="88524-134">Request</span></span>
<span data-ttu-id="88524-135">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="88524-135">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88524-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="88524-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="88524-137">C#</span><span class="sxs-lookup"><span data-stu-id="88524-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88524-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88524-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88524-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88524-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88524-140">Java</span><span class="sxs-lookup"><span data-stu-id="88524-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="88524-141">**注意：**`id`请求中的是 **设备的 ID** 属性，而不是 **deviceId** 属性。</span><span class="sxs-lookup"><span data-stu-id="88524-141">**Note:** The `id` in the request is the **id** property of the device, not the **deviceId** property.</span></span>

### <a name="response"></a><span data-ttu-id="88524-142">响应</span><span class="sxs-lookup"><span data-stu-id="88524-142">Response</span></span>
<span data-ttu-id="88524-143">以下示例显示了对没有 **hostNames** 的设备的响应。</span><span class="sxs-lookup"><span data-stu-id="88524-143">The following example shows a response for a device with no **hostNames**.</span></span> 

><span data-ttu-id="88524-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88524-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

<span data-ttu-id="88524-145">以下示例显示了对具有 **hostNames** 的设备的响应。</span><span class="sxs-lookup"><span data-stu-id="88524-145">The following example shows a response for a device with **hostNames**.</span></span> 

><span data-ttu-id="88524-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88524-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="88524-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="88524-147">See also</span></span>

- [<span data-ttu-id="88524-148">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="88524-148">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="88524-149">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="88524-149">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="88524-150">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="88524-150">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
