---
title: 创建设备
description: 在组织中创建并注册一个新设备。
ms.openlocfilehash: 7dd4ab48c66383990eb3fca4630717ba8063c67a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009299"
---
# <a name="create-device"></a><span data-ttu-id="f190d-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="f190d-103">Create device</span></span>

<span data-ttu-id="f190d-104">在组织中创建并注册一个新设备。</span><span class="sxs-lookup"><span data-stu-id="f190d-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f190d-105">权限</span><span class="sxs-lookup"><span data-stu-id="f190d-105">Permissions</span></span>
<span data-ttu-id="f190d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f190d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f190d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f190d-108">Permission type</span></span>      | <span data-ttu-id="f190d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f190d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f190d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f190d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f190d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f190d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f190d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f190d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f190d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f190d-113">Not supported.</span></span>    |
|<span data-ttu-id="f190d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f190d-114">Application</span></span> | <span data-ttu-id="f190d-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f190d-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f190d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f190d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="f190d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f190d-117">Request headers</span></span>
| <span data-ttu-id="f190d-118">名称</span><span class="sxs-lookup"><span data-stu-id="f190d-118">Name</span></span>       | <span data-ttu-id="f190d-119">类型</span><span class="sxs-lookup"><span data-stu-id="f190d-119">Type</span></span> | <span data-ttu-id="f190d-120">说明</span><span class="sxs-lookup"><span data-stu-id="f190d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f190d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f190d-121">Authorization</span></span>  | <span data-ttu-id="f190d-122">string</span><span class="sxs-lookup"><span data-stu-id="f190d-122">string</span></span>  | <span data-ttu-id="f190d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f190d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f190d-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="f190d-125">Content-type</span></span> | <span data-ttu-id="f190d-126">string</span><span class="sxs-lookup"><span data-stu-id="f190d-126">string</span></span> | <span data-ttu-id="f190d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f190d-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f190d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f190d-128">Request body</span></span>
<span data-ttu-id="f190d-129">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f190d-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f190d-130">响应</span><span class="sxs-lookup"><span data-stu-id="f190d-130">Response</span></span>

<span data-ttu-id="f190d-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f190d-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f190d-132">示例</span><span class="sxs-lookup"><span data-stu-id="f190d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f190d-133">请求</span><span class="sxs-lookup"><span data-stu-id="f190d-133">Request</span></span>
<span data-ttu-id="f190d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f190d-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="f190d-135">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f190d-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f190d-136">响应</span><span class="sxs-lookup"><span data-stu-id="f190d-136">Response</span></span>
<span data-ttu-id="f190d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f190d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
