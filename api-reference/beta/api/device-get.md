---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e52d339b4be3af43ab6d1c3e5cb6f30bc16c262e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435883"
---
# <a name="get-device"></a><span data-ttu-id="9e7b9-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="9e7b9-103">Get device</span></span>

<span data-ttu-id="9e7b9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9e7b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e7b9-105">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-105">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="9e7b9-106">由于**设备**资源支持[扩展](/graph/extensibility-overview)，因此您还可以使用此`GET`操作获取**设备**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-106">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e7b9-107">权限</span><span class="sxs-lookup"><span data-stu-id="9e7b9-107">Permissions</span></span>
<span data-ttu-id="9e7b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e7b9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e7b9-110">Permission type</span></span>      | <span data-ttu-id="9e7b9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e7b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e7b9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e7b9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9e7b9-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e7b9-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e7b9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e7b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e7b9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-115">Not supported.</span></span>    |
|<span data-ttu-id="9e7b9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e7b9-116">Application</span></span> | <span data-ttu-id="9e7b9-117">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e7b9-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e7b9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e7b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e7b9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9e7b9-119">Optional query parameters</span></span>
<span data-ttu-id="9e7b9-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9e7b9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e7b9-121">Request headers</span></span>
| <span data-ttu-id="9e7b9-122">名称</span><span class="sxs-lookup"><span data-stu-id="9e7b9-122">Name</span></span>       | <span data-ttu-id="9e7b9-123">类型</span><span class="sxs-lookup"><span data-stu-id="9e7b9-123">Type</span></span> | <span data-ttu-id="9e7b9-124">说明</span><span class="sxs-lookup"><span data-stu-id="9e7b9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9e7b9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e7b9-125">Authorization</span></span>  | <span data-ttu-id="9e7b9-126">string</span><span class="sxs-lookup"><span data-stu-id="9e7b9-126">string</span></span>  | <span data-ttu-id="9e7b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e7b9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e7b9-129">Request body</span></span>
<span data-ttu-id="9e7b9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e7b9-131">响应</span><span class="sxs-lookup"><span data-stu-id="9e7b9-131">Response</span></span>

<span data-ttu-id="9e7b9-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e7b9-133">示例</span><span class="sxs-lookup"><span data-stu-id="9e7b9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e7b9-134">请求</span><span class="sxs-lookup"><span data-stu-id="9e7b9-134">Request</span></span>
<span data-ttu-id="9e7b9-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e7b9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e7b9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="9e7b9-137">C#</span><span class="sxs-lookup"><span data-stu-id="9e7b9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e7b9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e7b9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e7b9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e7b9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="9e7b9-140">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-140">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="9e7b9-141">响应</span><span class="sxs-lookup"><span data-stu-id="9e7b9-141">Response</span></span>
<span data-ttu-id="9e7b9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e7b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9e7b9-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9e7b9-145">See also</span></span>

- [<span data-ttu-id="9e7b9-146">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="9e7b9-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9e7b9-147">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="9e7b9-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9e7b9-148">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="9e7b9-148">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
