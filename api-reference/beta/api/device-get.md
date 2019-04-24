---
title: 获取设备
description: 获取 device 对象的属性和关系。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b0bc325620a27d9383b4a12d5f3da970c0c267
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455280"
---
# <a name="get-device"></a><span data-ttu-id="3eab5-103">获取设备</span><span class="sxs-lookup"><span data-stu-id="3eab5-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eab5-104">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3eab5-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="3eab5-105">由于**设备**资源支持[扩展](/graph/extensibility-overview), 因此您还可以使用此`GET`操作获取**设备**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="3eab5-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eab5-106">权限</span><span class="sxs-lookup"><span data-stu-id="3eab5-106">Permissions</span></span>
<span data-ttu-id="3eab5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3eab5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3eab5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3eab5-109">Permission type</span></span>      | <span data-ttu-id="3eab5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3eab5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eab5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3eab5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3eab5-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3eab5-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3eab5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3eab5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eab5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3eab5-114">Not supported.</span></span>    |
|<span data-ttu-id="3eab5-115">Application</span><span class="sxs-lookup"><span data-stu-id="3eab5-115">Application</span></span> | <span data-ttu-id="3eab5-116">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eab5-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eab5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3eab5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3eab5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3eab5-118">Optional query parameters</span></span>
<span data-ttu-id="3eab5-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3eab5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3eab5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3eab5-120">Request headers</span></span>
| <span data-ttu-id="3eab5-121">名称</span><span class="sxs-lookup"><span data-stu-id="3eab5-121">Name</span></span>       | <span data-ttu-id="3eab5-122">类型</span><span class="sxs-lookup"><span data-stu-id="3eab5-122">Type</span></span> | <span data-ttu-id="3eab5-123">说明</span><span class="sxs-lookup"><span data-stu-id="3eab5-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3eab5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eab5-124">Authorization</span></span>  | <span data-ttu-id="3eab5-125">string</span><span class="sxs-lookup"><span data-stu-id="3eab5-125">string</span></span>  | <span data-ttu-id="3eab5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3eab5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3eab5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3eab5-128">Request body</span></span>
<span data-ttu-id="3eab5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3eab5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eab5-130">响应</span><span class="sxs-lookup"><span data-stu-id="3eab5-130">Response</span></span>

<span data-ttu-id="3eab5-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3eab5-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3eab5-132">示例</span><span class="sxs-lookup"><span data-stu-id="3eab5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3eab5-133">请求</span><span class="sxs-lookup"><span data-stu-id="3eab5-133">Request</span></span>
<span data-ttu-id="3eab5-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3eab5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="3eab5-135">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="3eab5-135">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="3eab5-136">响应</span><span class="sxs-lookup"><span data-stu-id="3eab5-136">Response</span></span>
<span data-ttu-id="3eab5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3eab5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3eab5-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3eab5-140">See also</span></span>

- [<span data-ttu-id="3eab5-141">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3eab5-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3eab5-142">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="3eab5-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3eab5-143">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="3eab5-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
