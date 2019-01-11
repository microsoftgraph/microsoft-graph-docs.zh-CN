---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1402b74f9af411a6d41ac9b37c5c54b4736de499
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811226"
---
# <a name="get-device"></a><span data-ttu-id="f2f27-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="f2f27-103">Get device</span></span>

<span data-ttu-id="f2f27-104">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2f27-104">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2f27-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2f27-105">Permissions</span></span>
<span data-ttu-id="f2f27-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2f27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f2f27-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2f27-108">Permission type</span></span>      | <span data-ttu-id="f2f27-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2f27-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2f27-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2f27-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2f27-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2f27-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2f27-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2f27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2f27-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2f27-113">Not supported.</span></span>    |
|<span data-ttu-id="f2f27-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2f27-114">Application</span></span> | <span data-ttu-id="f2f27-115">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2f27-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2f27-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2f27-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="f2f27-117">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="f2f27-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f2f27-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f2f27-118">Optional query parameters</span></span>
<span data-ttu-id="f2f27-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f2f27-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2f27-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2f27-120">Request headers</span></span>
| <span data-ttu-id="f2f27-121">名称</span><span class="sxs-lookup"><span data-stu-id="f2f27-121">Name</span></span>       | <span data-ttu-id="f2f27-122">类型</span><span class="sxs-lookup"><span data-stu-id="f2f27-122">Type</span></span> | <span data-ttu-id="f2f27-123">说明</span><span class="sxs-lookup"><span data-stu-id="f2f27-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2f27-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2f27-124">Authorization</span></span>  | <span data-ttu-id="f2f27-125">string</span><span class="sxs-lookup"><span data-stu-id="f2f27-125">string</span></span>  | <span data-ttu-id="f2f27-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2f27-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2f27-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2f27-128">Request body</span></span>
<span data-ttu-id="f2f27-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2f27-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2f27-130">响应</span><span class="sxs-lookup"><span data-stu-id="f2f27-130">Response</span></span>

<span data-ttu-id="f2f27-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2f27-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2f27-132">示例</span><span class="sxs-lookup"><span data-stu-id="f2f27-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2f27-133">请求</span><span class="sxs-lookup"><span data-stu-id="f2f27-133">Request</span></span>
<span data-ttu-id="f2f27-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2f27-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="f2f27-135">响应</span><span class="sxs-lookup"><span data-stu-id="f2f27-135">Response</span></span>
<span data-ttu-id="f2f27-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2f27-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
