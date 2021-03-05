---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e68966ebf5ba6b59aefea1b4660045d68e011aff
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434606"
---
# <a name="get-device"></a><span data-ttu-id="2b850-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="2b850-103">Get device</span></span>

<span data-ttu-id="2b850-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b850-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b850-105">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2b850-105">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b850-106">权限</span><span class="sxs-lookup"><span data-stu-id="2b850-106">Permissions</span></span>
<span data-ttu-id="2b850-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b850-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b850-109">Permission type</span></span>      | <span data-ttu-id="2b850-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b850-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b850-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b850-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b850-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b850-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b850-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b850-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b850-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b850-114">Not supported.</span></span>    |
|<span data-ttu-id="2b850-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b850-115">Application</span></span> | <span data-ttu-id="2b850-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b850-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b850-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b850-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="2b850-118">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="2b850-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2b850-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2b850-119">Optional query parameters</span></span>
<span data-ttu-id="2b850-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2b850-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b850-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b850-121">Request headers</span></span>
| <span data-ttu-id="2b850-122">名称</span><span class="sxs-lookup"><span data-stu-id="2b850-122">Name</span></span>       | <span data-ttu-id="2b850-123">类型</span><span class="sxs-lookup"><span data-stu-id="2b850-123">Type</span></span> | <span data-ttu-id="2b850-124">说明</span><span class="sxs-lookup"><span data-stu-id="2b850-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b850-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b850-125">Authorization</span></span>  | <span data-ttu-id="2b850-126">string</span><span class="sxs-lookup"><span data-stu-id="2b850-126">string</span></span>  | <span data-ttu-id="2b850-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b850-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b850-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b850-129">Request body</span></span>
<span data-ttu-id="2b850-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b850-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b850-131">响应</span><span class="sxs-lookup"><span data-stu-id="2b850-131">Response</span></span>

<span data-ttu-id="2b850-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2b850-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b850-133">示例</span><span class="sxs-lookup"><span data-stu-id="2b850-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b850-134">请求</span><span class="sxs-lookup"><span data-stu-id="2b850-134">Request</span></span>
<span data-ttu-id="2b850-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b850-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b850-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b850-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="2b850-137">C#</span><span class="sxs-lookup"><span data-stu-id="2b850-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b850-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b850-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b850-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b850-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b850-140">Java</span><span class="sxs-lookup"><span data-stu-id="2b850-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b850-141">响应</span><span class="sxs-lookup"><span data-stu-id="2b850-141">Response</span></span>
<span data-ttu-id="2b850-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b850-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
