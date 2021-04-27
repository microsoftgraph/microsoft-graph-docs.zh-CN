---
title: 创建设备
description: 创建新设备。
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2c316b2c6a4eac5e37d94b1182c3b3f5bfbce7c9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046942"
---
# <a name="create-device"></a><span data-ttu-id="c91e5-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="c91e5-103">Create device</span></span>

<span data-ttu-id="c91e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c91e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c91e5-105">创建新设备。</span><span class="sxs-lookup"><span data-stu-id="c91e5-105">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="c91e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="c91e5-106">Permissions</span></span>
<span data-ttu-id="c91e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c91e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c91e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c91e5-109">Permission type</span></span>      | <span data-ttu-id="c91e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c91e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c91e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c91e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c91e5-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c91e5-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c91e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c91e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c91e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c91e5-114">Not supported.</span></span>    |
|<span data-ttu-id="c91e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c91e5-115">Application</span></span> | <span data-ttu-id="c91e5-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c91e5-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c91e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c91e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="c91e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c91e5-118">Request headers</span></span>
| <span data-ttu-id="c91e5-119">名称</span><span class="sxs-lookup"><span data-stu-id="c91e5-119">Name</span></span>       | <span data-ttu-id="c91e5-120">类型</span><span class="sxs-lookup"><span data-stu-id="c91e5-120">Type</span></span> | <span data-ttu-id="c91e5-121">说明</span><span class="sxs-lookup"><span data-stu-id="c91e5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c91e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c91e5-122">Authorization</span></span>  | <span data-ttu-id="c91e5-123">string</span><span class="sxs-lookup"><span data-stu-id="c91e5-123">string</span></span>  | <span data-ttu-id="c91e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c91e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c91e5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c91e5-126">Request body</span></span>
<span data-ttu-id="c91e5-127">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c91e5-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="c91e5-128">由于 **设备** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作，并在创建设备实例时将包含你自己的数据的 `POST` 自定义属性添加到设备实例。</span><span class="sxs-lookup"><span data-stu-id="c91e5-128">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="c91e5-129">响应</span><span class="sxs-lookup"><span data-stu-id="c91e5-129">Response</span></span>

<span data-ttu-id="c91e5-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c91e5-130">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c91e5-131">示例</span><span class="sxs-lookup"><span data-stu-id="c91e5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c91e5-132">请求</span><span class="sxs-lookup"><span data-stu-id="c91e5-132">Request</span></span>
<span data-ttu-id="c91e5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c91e5-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c91e5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c91e5-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c91e5-135">C#</span><span class="sxs-lookup"><span data-stu-id="c91e5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c91e5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c91e5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c91e5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c91e5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c91e5-138">Java</span><span class="sxs-lookup"><span data-stu-id="c91e5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c91e5-139">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c91e5-139">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c91e5-140">响应</span><span class="sxs-lookup"><span data-stu-id="c91e5-140">Response</span></span>
<span data-ttu-id="c91e5-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c91e5-141">Here is an example of the response.</span></span> <span data-ttu-id="c91e5-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c91e5-142">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c91e5-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c91e5-143">See also</span></span>

- [<span data-ttu-id="c91e5-144">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c91e5-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c91e5-145">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="c91e5-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c91e5-146">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="c91e5-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


