---
title: 创建设备
description: 创建新设备。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 83c67824726e294ed6b60bb32fae7452bf60a3bf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417590"
---
# <a name="create-device"></a><span data-ttu-id="b3dc7-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="b3dc7-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3dc7-104">创建新设备。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3dc7-105">权限</span><span class="sxs-lookup"><span data-stu-id="b3dc7-105">Permissions</span></span>
<span data-ttu-id="b3dc7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b3dc7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3dc7-108">Permission type</span></span>      | <span data-ttu-id="b3dc7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3dc7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3dc7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3dc7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3dc7-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3dc7-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3dc7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3dc7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3dc7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-113">Not supported.</span></span>    |
|<span data-ttu-id="b3dc7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3dc7-114">Application</span></span> | <span data-ttu-id="b3dc7-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3dc7-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3dc7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3dc7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="b3dc7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3dc7-117">Request headers</span></span>
| <span data-ttu-id="b3dc7-118">名称</span><span class="sxs-lookup"><span data-stu-id="b3dc7-118">Name</span></span>       | <span data-ttu-id="b3dc7-119">类型</span><span class="sxs-lookup"><span data-stu-id="b3dc7-119">Type</span></span> | <span data-ttu-id="b3dc7-120">说明</span><span class="sxs-lookup"><span data-stu-id="b3dc7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3dc7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3dc7-121">Authorization</span></span>  | <span data-ttu-id="b3dc7-122">string</span><span class="sxs-lookup"><span data-stu-id="b3dc7-122">string</span></span>  | <span data-ttu-id="b3dc7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3dc7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3dc7-125">Request body</span></span>
<span data-ttu-id="b3dc7-126">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="b3dc7-127">由于**设备**资源支持[扩展](/graph/extensibility-overview), 因此可以在创建设备`POST`实例时使用该操作并向其添加包含自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="b3dc7-128">响应</span><span class="sxs-lookup"><span data-stu-id="b3dc7-128">Response</span></span>

<span data-ttu-id="b3dc7-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3dc7-130">示例</span><span class="sxs-lookup"><span data-stu-id="b3dc7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3dc7-131">请求</span><span class="sxs-lookup"><span data-stu-id="b3dc7-131">Request</span></span>
<span data-ttu-id="b3dc7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b3dc7-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b3dc7-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3dc7-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3dc7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3dc7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3dc7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3dc7-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="b3dc7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b3dc7-137">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-137">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b3dc7-138">响应</span><span class="sxs-lookup"><span data-stu-id="b3dc7-138">Response</span></span>
<span data-ttu-id="b3dc7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3dc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b3dc7-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b3dc7-142">See also</span></span>

- [<span data-ttu-id="b3dc7-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b3dc7-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b3dc7-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="b3dc7-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b3dc7-145">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="b3dc7-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
