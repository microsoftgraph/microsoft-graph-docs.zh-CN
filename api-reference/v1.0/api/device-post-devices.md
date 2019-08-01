---
title: 创建设备
description: 在组织中创建并注册一个新设备。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3fcaaa3e2da274848495eb0dfbb259ed4200db87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002963"
---
# <a name="create-device"></a><span data-ttu-id="af190-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="af190-103">Create device</span></span>

<span data-ttu-id="af190-104">在组织中创建并注册一个新设备。</span><span class="sxs-lookup"><span data-stu-id="af190-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="af190-105">权限</span><span class="sxs-lookup"><span data-stu-id="af190-105">Permissions</span></span>
<span data-ttu-id="af190-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="af190-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="af190-108">Permission type</span></span>      | <span data-ttu-id="af190-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af190-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af190-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af190-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af190-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af190-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af190-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af190-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af190-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="af190-113">Not supported.</span></span>    |
|<span data-ttu-id="af190-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="af190-114">Application</span></span> | <span data-ttu-id="af190-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af190-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af190-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af190-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="af190-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="af190-117">Request headers</span></span>
| <span data-ttu-id="af190-118">名称</span><span class="sxs-lookup"><span data-stu-id="af190-118">Name</span></span>       | <span data-ttu-id="af190-119">类型</span><span class="sxs-lookup"><span data-stu-id="af190-119">Type</span></span> | <span data-ttu-id="af190-120">说明</span><span class="sxs-lookup"><span data-stu-id="af190-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="af190-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af190-121">Authorization</span></span>  | <span data-ttu-id="af190-122">string</span><span class="sxs-lookup"><span data-stu-id="af190-122">string</span></span>  | <span data-ttu-id="af190-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="af190-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af190-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="af190-125">Content-type</span></span> | <span data-ttu-id="af190-126">string</span><span class="sxs-lookup"><span data-stu-id="af190-126">string</span></span> | <span data-ttu-id="af190-127">application/json</span><span class="sxs-lookup"><span data-stu-id="af190-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="af190-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="af190-128">Request body</span></span>
<span data-ttu-id="af190-129">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af190-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="af190-130">响应</span><span class="sxs-lookup"><span data-stu-id="af190-130">Response</span></span>

<span data-ttu-id="af190-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af190-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af190-132">示例</span><span class="sxs-lookup"><span data-stu-id="af190-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af190-133">请求</span><span class="sxs-lookup"><span data-stu-id="af190-133">Request</span></span>
<span data-ttu-id="af190-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af190-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="af190-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="af190-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af190-136">C#</span><span class="sxs-lookup"><span data-stu-id="af190-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af190-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="af190-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="af190-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="af190-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="af190-139">Java</span><span class="sxs-lookup"><span data-stu-id="af190-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="af190-140">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af190-140">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="af190-141">响应</span><span class="sxs-lookup"><span data-stu-id="af190-141">Response</span></span>
<span data-ttu-id="af190-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af190-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
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
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
