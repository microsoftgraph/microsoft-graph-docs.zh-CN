---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32ca8dc4eefb51706e97d2c4b6b97aadd0d1ff8e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862791"
---
# <a name="get-device"></a><span data-ttu-id="b47ee-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="b47ee-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b47ee-104">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b47ee-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="b47ee-105">由于**设备**资源支持[扩展](/graph/extensibility-overview), 因此您还可以使用此`GET`操作获取**设备**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="b47ee-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="b47ee-106">权限</span><span class="sxs-lookup"><span data-stu-id="b47ee-106">Permissions</span></span>
<span data-ttu-id="b47ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b47ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b47ee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b47ee-109">Permission type</span></span>      | <span data-ttu-id="b47ee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b47ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b47ee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b47ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b47ee-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b47ee-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b47ee-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b47ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b47ee-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b47ee-114">Not supported.</span></span>    |
|<span data-ttu-id="b47ee-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b47ee-115">Application</span></span> | <span data-ttu-id="b47ee-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b47ee-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b47ee-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b47ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b47ee-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b47ee-118">Optional query parameters</span></span>
<span data-ttu-id="b47ee-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b47ee-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b47ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b47ee-120">Request headers</span></span>
| <span data-ttu-id="b47ee-121">名称</span><span class="sxs-lookup"><span data-stu-id="b47ee-121">Name</span></span>       | <span data-ttu-id="b47ee-122">类型</span><span class="sxs-lookup"><span data-stu-id="b47ee-122">Type</span></span> | <span data-ttu-id="b47ee-123">说明</span><span class="sxs-lookup"><span data-stu-id="b47ee-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b47ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b47ee-124">Authorization</span></span>  | <span data-ttu-id="b47ee-125">string</span><span class="sxs-lookup"><span data-stu-id="b47ee-125">string</span></span>  | <span data-ttu-id="b47ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b47ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b47ee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b47ee-128">Request body</span></span>
<span data-ttu-id="b47ee-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b47ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b47ee-130">响应</span><span class="sxs-lookup"><span data-stu-id="b47ee-130">Response</span></span>

<span data-ttu-id="b47ee-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b47ee-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b47ee-132">示例</span><span class="sxs-lookup"><span data-stu-id="b47ee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b47ee-133">请求</span><span class="sxs-lookup"><span data-stu-id="b47ee-133">Request</span></span>
<span data-ttu-id="b47ee-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b47ee-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b47ee-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b47ee-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b47ee-136">C#</span><span class="sxs-lookup"><span data-stu-id="b47ee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b47ee-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b47ee-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b47ee-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="b47ee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b47ee-139">Java</span><span class="sxs-lookup"><span data-stu-id="b47ee-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="b47ee-140">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="b47ee-140">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="b47ee-141">响应</span><span class="sxs-lookup"><span data-stu-id="b47ee-141">Response</span></span>
<span data-ttu-id="b47ee-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b47ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="b47ee-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b47ee-145">See also</span></span>

- [<span data-ttu-id="b47ee-146">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b47ee-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b47ee-147">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="b47ee-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b47ee-148">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="b47ee-148">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
