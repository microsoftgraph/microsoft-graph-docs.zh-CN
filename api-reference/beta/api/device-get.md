---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 632094db64cce86a965751d97b0ae9c92d439d5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348263"
---
# <a name="get-device"></a><span data-ttu-id="176de-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="176de-103">Get device</span></span>

> <span data-ttu-id="176de-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="176de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="176de-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="176de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="176de-106">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="176de-106">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="176de-107">由于**设备**资源支持[扩展](/graph/extensibility-overview)，您还可以使用`GET`操作来获取**设备**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="176de-107">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="176de-108">权限</span><span class="sxs-lookup"><span data-stu-id="176de-108">Permissions</span></span>
<span data-ttu-id="176de-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="176de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="176de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="176de-111">Permission type</span></span>      | <span data-ttu-id="176de-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="176de-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="176de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="176de-113">Delegated (work or school account)</span></span> | <span data-ttu-id="176de-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="176de-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="176de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="176de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="176de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="176de-116">Not supported.</span></span>    |
|<span data-ttu-id="176de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="176de-117">Application</span></span> | <span data-ttu-id="176de-118">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176de-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="176de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="176de-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="176de-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="176de-120">Optional query parameters</span></span>
<span data-ttu-id="176de-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="176de-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="176de-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="176de-122">Request headers</span></span>
| <span data-ttu-id="176de-123">Name</span><span class="sxs-lookup"><span data-stu-id="176de-123">Name</span></span>       | <span data-ttu-id="176de-124">类型</span><span class="sxs-lookup"><span data-stu-id="176de-124">Type</span></span> | <span data-ttu-id="176de-125">说明</span><span class="sxs-lookup"><span data-stu-id="176de-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="176de-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="176de-126">Authorization</span></span>  | <span data-ttu-id="176de-127">string</span><span class="sxs-lookup"><span data-stu-id="176de-127">string</span></span>  | <span data-ttu-id="176de-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="176de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="176de-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="176de-130">Request body</span></span>
<span data-ttu-id="176de-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="176de-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="176de-132">响应</span><span class="sxs-lookup"><span data-stu-id="176de-132">Response</span></span>

<span data-ttu-id="176de-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="176de-133">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="176de-134">示例</span><span class="sxs-lookup"><span data-stu-id="176de-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="176de-135">请求</span><span class="sxs-lookup"><span data-stu-id="176de-135">Request</span></span>
<span data-ttu-id="176de-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="176de-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="176de-137">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="176de-137">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="176de-138">响应</span><span class="sxs-lookup"><span data-stu-id="176de-138">Response</span></span>
<span data-ttu-id="176de-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="176de-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="176de-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="176de-142">See also</span></span>

- [<span data-ttu-id="176de-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="176de-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="176de-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="176de-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="176de-145">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="176de-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->