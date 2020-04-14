---
title: 创建设备
description: 创建新设备。
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61570106a40d1635b036673d61e660cb64c2f40b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381803"
---
# <a name="create-device"></a><span data-ttu-id="26066-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="26066-103">Create device</span></span>

<span data-ttu-id="26066-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26066-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26066-105">创建新设备。</span><span class="sxs-lookup"><span data-stu-id="26066-105">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="26066-106">权限</span><span class="sxs-lookup"><span data-stu-id="26066-106">Permissions</span></span>
<span data-ttu-id="26066-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="26066-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26066-109">Permission type</span></span>      | <span data-ttu-id="26066-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26066-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26066-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26066-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26066-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26066-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26066-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26066-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26066-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26066-114">Not supported.</span></span>    |
|<span data-ttu-id="26066-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="26066-115">Application</span></span> | <span data-ttu-id="26066-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26066-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26066-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26066-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="26066-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="26066-118">Request headers</span></span>
| <span data-ttu-id="26066-119">名称</span><span class="sxs-lookup"><span data-stu-id="26066-119">Name</span></span>       | <span data-ttu-id="26066-120">类型</span><span class="sxs-lookup"><span data-stu-id="26066-120">Type</span></span> | <span data-ttu-id="26066-121">说明</span><span class="sxs-lookup"><span data-stu-id="26066-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26066-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26066-122">Authorization</span></span>  | <span data-ttu-id="26066-123">string</span><span class="sxs-lookup"><span data-stu-id="26066-123">string</span></span>  | <span data-ttu-id="26066-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26066-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26066-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26066-126">Request body</span></span>
<span data-ttu-id="26066-127">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26066-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="26066-128">由于**设备**资源支持[扩展](/graph/extensibility-overview)，因此可以在创建设备`POST`实例时使用该操作并向其添加包含自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="26066-128">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="26066-129">响应</span><span class="sxs-lookup"><span data-stu-id="26066-129">Response</span></span>

<span data-ttu-id="26066-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="26066-130">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26066-131">示例</span><span class="sxs-lookup"><span data-stu-id="26066-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26066-132">请求</span><span class="sxs-lookup"><span data-stu-id="26066-132">Request</span></span>
<span data-ttu-id="26066-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26066-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26066-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="26066-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/beta/devices
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
# <a name="c"></a>[<span data-ttu-id="26066-135">C#</span><span class="sxs-lookup"><span data-stu-id="26066-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26066-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26066-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26066-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26066-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="26066-138">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26066-138">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="26066-139">响应</span><span class="sxs-lookup"><span data-stu-id="26066-139">Response</span></span>
<span data-ttu-id="26066-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26066-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="26066-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="26066-143">See also</span></span>

- [<span data-ttu-id="26066-144">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="26066-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="26066-145">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="26066-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="26066-146">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="26066-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
