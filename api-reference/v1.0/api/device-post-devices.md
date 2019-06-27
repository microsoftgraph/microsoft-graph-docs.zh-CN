---
title: 创建设备
description: 在组织中创建并注册一个新设备。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c70c2f4f3ce4d1d81e9fc1c2df94c41d8683485e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272952"
---
# <a name="create-device"></a><span data-ttu-id="b398e-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="b398e-103">Create device</span></span>

<span data-ttu-id="b398e-104">在组织中创建并注册一个新设备。</span><span class="sxs-lookup"><span data-stu-id="b398e-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b398e-105">权限</span><span class="sxs-lookup"><span data-stu-id="b398e-105">Permissions</span></span>
<span data-ttu-id="b398e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b398e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b398e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b398e-108">Permission type</span></span>      | <span data-ttu-id="b398e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b398e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b398e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b398e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b398e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b398e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b398e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b398e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b398e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b398e-113">Not supported.</span></span>    |
|<span data-ttu-id="b398e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b398e-114">Application</span></span> | <span data-ttu-id="b398e-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b398e-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b398e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b398e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="b398e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b398e-117">Request headers</span></span>
| <span data-ttu-id="b398e-118">名称</span><span class="sxs-lookup"><span data-stu-id="b398e-118">Name</span></span>       | <span data-ttu-id="b398e-119">类型</span><span class="sxs-lookup"><span data-stu-id="b398e-119">Type</span></span> | <span data-ttu-id="b398e-120">说明</span><span class="sxs-lookup"><span data-stu-id="b398e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b398e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b398e-121">Authorization</span></span>  | <span data-ttu-id="b398e-122">string</span><span class="sxs-lookup"><span data-stu-id="b398e-122">string</span></span>  | <span data-ttu-id="b398e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b398e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b398e-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="b398e-125">Content-type</span></span> | <span data-ttu-id="b398e-126">string</span><span class="sxs-lookup"><span data-stu-id="b398e-126">string</span></span> | <span data-ttu-id="b398e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b398e-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b398e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b398e-128">Request body</span></span>
<span data-ttu-id="b398e-129">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b398e-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b398e-130">响应</span><span class="sxs-lookup"><span data-stu-id="b398e-130">Response</span></span>

<span data-ttu-id="b398e-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b398e-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b398e-132">示例</span><span class="sxs-lookup"><span data-stu-id="b398e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b398e-133">请求</span><span class="sxs-lookup"><span data-stu-id="b398e-133">Request</span></span>
<span data-ttu-id="b398e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b398e-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="b398e-135">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b398e-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b398e-136">响应</span><span class="sxs-lookup"><span data-stu-id="b398e-136">Response</span></span>
<span data-ttu-id="b398e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b398e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b398e-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b398e-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b398e-141">C#</span><span class="sxs-lookup"><span data-stu-id="b398e-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_device_from_devices-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b398e-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="b398e-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_device_from_devices-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b398e-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="b398e-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_device_from_devices-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-post-devices.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-post-devices.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-post-devices.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
