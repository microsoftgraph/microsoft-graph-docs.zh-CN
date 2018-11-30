---
title: 创建设备
description: 创建一个新的设备。
ms.openlocfilehash: 33dc1f8da40e29e8c135cf24f35ec3ce52af9b06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046122"
---
# <a name="create-device"></a><span data-ttu-id="38aa2-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="38aa2-103">Create device</span></span>

> <span data-ttu-id="38aa2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38aa2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38aa2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38aa2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38aa2-106">创建一个新的设备。</span><span class="sxs-lookup"><span data-stu-id="38aa2-106">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="38aa2-107">权限</span><span class="sxs-lookup"><span data-stu-id="38aa2-107">Permissions</span></span>
<span data-ttu-id="38aa2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38aa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="38aa2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38aa2-110">Permission type</span></span>      | <span data-ttu-id="38aa2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38aa2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38aa2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38aa2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="38aa2-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38aa2-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38aa2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38aa2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38aa2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38aa2-115">Not supported.</span></span>    |
|<span data-ttu-id="38aa2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="38aa2-116">Application</span></span> | <span data-ttu-id="38aa2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38aa2-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38aa2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38aa2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="38aa2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38aa2-119">Request headers</span></span>
| <span data-ttu-id="38aa2-120">名称</span><span class="sxs-lookup"><span data-stu-id="38aa2-120">Name</span></span>       | <span data-ttu-id="38aa2-121">类型</span><span class="sxs-lookup"><span data-stu-id="38aa2-121">Type</span></span> | <span data-ttu-id="38aa2-122">说明</span><span class="sxs-lookup"><span data-stu-id="38aa2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38aa2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38aa2-123">Authorization</span></span>  | <span data-ttu-id="38aa2-124">string</span><span class="sxs-lookup"><span data-stu-id="38aa2-124">string</span></span>  | <span data-ttu-id="38aa2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38aa2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38aa2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38aa2-127">Request body</span></span>
<span data-ttu-id="38aa2-128">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38aa2-128">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="38aa2-129">由于**设备**资源支持[扩展](/graph/extensibility-overview)，您可以使用`POST`操作并创建它时将使用您自己的数据的自定义属性添加到设备实例。</span><span class="sxs-lookup"><span data-stu-id="38aa2-129">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="38aa2-130">响应</span><span class="sxs-lookup"><span data-stu-id="38aa2-130">Response</span></span>

<span data-ttu-id="38aa2-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38aa2-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38aa2-132">示例</span><span class="sxs-lookup"><span data-stu-id="38aa2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38aa2-133">请求</span><span class="sxs-lookup"><span data-stu-id="38aa2-133">Request</span></span>
<span data-ttu-id="38aa2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38aa2-134">Here is an example of the request.</span></span>
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
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
<span data-ttu-id="38aa2-135">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38aa2-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="38aa2-136">响应</span><span class="sxs-lookup"><span data-stu-id="38aa2-136">Response</span></span>
<span data-ttu-id="38aa2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38aa2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="38aa2-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="38aa2-140">See also</span></span>

- [<span data-ttu-id="38aa2-141">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="38aa2-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="38aa2-142">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="38aa2-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="38aa2-143">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="38aa2-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->