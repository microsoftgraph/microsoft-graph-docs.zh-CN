---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb9ceac13ad2726942bc445b17a9d8362564be4f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437303"
---
# <a name="get-device"></a><span data-ttu-id="88ebe-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="88ebe-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88ebe-104">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88ebe-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="88ebe-105">由于**设备**资源支持[扩展](/graph/extensibility-overview), 因此您还可以使用此`GET`操作获取**设备**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="88ebe-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="88ebe-106">权限</span><span class="sxs-lookup"><span data-stu-id="88ebe-106">Permissions</span></span>
<span data-ttu-id="88ebe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88ebe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88ebe-109">Permission type</span></span>      | <span data-ttu-id="88ebe-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88ebe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88ebe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88ebe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88ebe-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88ebe-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88ebe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88ebe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88ebe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88ebe-114">Not supported.</span></span>    |
|<span data-ttu-id="88ebe-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88ebe-115">Application</span></span> | <span data-ttu-id="88ebe-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ebe-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88ebe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88ebe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88ebe-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88ebe-118">Optional query parameters</span></span>
<span data-ttu-id="88ebe-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="88ebe-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="88ebe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88ebe-120">Request headers</span></span>
| <span data-ttu-id="88ebe-121">名称</span><span class="sxs-lookup"><span data-stu-id="88ebe-121">Name</span></span>       | <span data-ttu-id="88ebe-122">类型</span><span class="sxs-lookup"><span data-stu-id="88ebe-122">Type</span></span> | <span data-ttu-id="88ebe-123">说明</span><span class="sxs-lookup"><span data-stu-id="88ebe-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="88ebe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88ebe-124">Authorization</span></span>  | <span data-ttu-id="88ebe-125">string</span><span class="sxs-lookup"><span data-stu-id="88ebe-125">string</span></span>  | <span data-ttu-id="88ebe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88ebe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88ebe-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="88ebe-128">Request body</span></span>
<span data-ttu-id="88ebe-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88ebe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88ebe-130">响应</span><span class="sxs-lookup"><span data-stu-id="88ebe-130">Response</span></span>

<span data-ttu-id="88ebe-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88ebe-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88ebe-132">示例</span><span class="sxs-lookup"><span data-stu-id="88ebe-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88ebe-133">请求</span><span class="sxs-lookup"><span data-stu-id="88ebe-133">Request</span></span>
<span data-ttu-id="88ebe-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88ebe-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="88ebe-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="88ebe-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="88ebe-136">C#</span><span class="sxs-lookup"><span data-stu-id="88ebe-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88ebe-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="88ebe-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88ebe-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="88ebe-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="88ebe-139">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="88ebe-139">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="88ebe-140">响应</span><span class="sxs-lookup"><span data-stu-id="88ebe-140">Response</span></span>
<span data-ttu-id="88ebe-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88ebe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="88ebe-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="88ebe-144">See also</span></span>

- [<span data-ttu-id="88ebe-145">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="88ebe-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="88ebe-146">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="88ebe-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="88ebe-147">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="88ebe-147">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
