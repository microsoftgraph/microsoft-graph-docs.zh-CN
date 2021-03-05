---
title: 创建设备
description: 在组织中创建并注册一个新设备。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 89e4b54e91cb027d88b36c426da8146f98fce781
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434529"
---
# <a name="create-device"></a><span data-ttu-id="14eb0-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="14eb0-103">Create device</span></span>

<span data-ttu-id="14eb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14eb0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14eb0-105">在组织中创建并注册一个新设备。</span><span class="sxs-lookup"><span data-stu-id="14eb0-105">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="14eb0-106">权限</span><span class="sxs-lookup"><span data-stu-id="14eb0-106">Permissions</span></span>
<span data-ttu-id="14eb0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14eb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="14eb0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14eb0-109">Permission type</span></span>      | <span data-ttu-id="14eb0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14eb0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14eb0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14eb0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="14eb0-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14eb0-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14eb0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14eb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14eb0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14eb0-114">Not supported.</span></span>    |
|<span data-ttu-id="14eb0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="14eb0-115">Application</span></span> | <span data-ttu-id="14eb0-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14eb0-116">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14eb0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14eb0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="14eb0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="14eb0-118">Request headers</span></span>
| <span data-ttu-id="14eb0-119">名称</span><span class="sxs-lookup"><span data-stu-id="14eb0-119">Name</span></span>       | <span data-ttu-id="14eb0-120">类型</span><span class="sxs-lookup"><span data-stu-id="14eb0-120">Type</span></span> | <span data-ttu-id="14eb0-121">说明</span><span class="sxs-lookup"><span data-stu-id="14eb0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14eb0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14eb0-122">Authorization</span></span>  | <span data-ttu-id="14eb0-123">string</span><span class="sxs-lookup"><span data-stu-id="14eb0-123">string</span></span>  | <span data-ttu-id="14eb0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14eb0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14eb0-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="14eb0-126">Content-type</span></span> | <span data-ttu-id="14eb0-127">string</span><span class="sxs-lookup"><span data-stu-id="14eb0-127">string</span></span> | <span data-ttu-id="14eb0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="14eb0-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="14eb0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="14eb0-129">Request body</span></span>
<span data-ttu-id="14eb0-130">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14eb0-130">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="14eb0-131">响应</span><span class="sxs-lookup"><span data-stu-id="14eb0-131">Response</span></span>

<span data-ttu-id="14eb0-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14eb0-132">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14eb0-133">示例</span><span class="sxs-lookup"><span data-stu-id="14eb0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14eb0-134">请求</span><span class="sxs-lookup"><span data-stu-id="14eb0-134">Request</span></span>
<span data-ttu-id="14eb0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14eb0-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14eb0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="14eb0-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="14eb0-137">C#</span><span class="sxs-lookup"><span data-stu-id="14eb0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14eb0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14eb0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14eb0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14eb0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14eb0-140">Java</span><span class="sxs-lookup"><span data-stu-id="14eb0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="14eb0-141">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14eb0-141">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="14eb0-142">响应</span><span class="sxs-lookup"><span data-stu-id="14eb0-142">Response</span></span>
<span data-ttu-id="14eb0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14eb0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

