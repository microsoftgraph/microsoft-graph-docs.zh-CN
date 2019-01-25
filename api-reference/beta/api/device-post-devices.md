---
title: 创建设备
description: 创建一个新的设备。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ad0400a74deec35daa4e28f91cafde5310c65c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514808"
---
# <a name="create-device"></a><span data-ttu-id="49543-103">创建设备</span><span class="sxs-lookup"><span data-stu-id="49543-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49543-104">创建一个新的设备。</span><span class="sxs-lookup"><span data-stu-id="49543-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="49543-105">权限</span><span class="sxs-lookup"><span data-stu-id="49543-105">Permissions</span></span>
<span data-ttu-id="49543-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="49543-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="49543-108">Permission type</span></span>      | <span data-ttu-id="49543-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49543-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49543-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49543-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49543-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49543-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49543-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49543-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49543-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="49543-113">Not supported.</span></span>    |
|<span data-ttu-id="49543-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="49543-114">Application</span></span> | <span data-ttu-id="49543-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49543-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49543-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49543-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="49543-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="49543-117">Request headers</span></span>
| <span data-ttu-id="49543-118">名称</span><span class="sxs-lookup"><span data-stu-id="49543-118">Name</span></span>       | <span data-ttu-id="49543-119">类型</span><span class="sxs-lookup"><span data-stu-id="49543-119">Type</span></span> | <span data-ttu-id="49543-120">说明</span><span class="sxs-lookup"><span data-stu-id="49543-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="49543-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="49543-121">Authorization</span></span>  | <span data-ttu-id="49543-122">string</span><span class="sxs-lookup"><span data-stu-id="49543-122">string</span></span>  | <span data-ttu-id="49543-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49543-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49543-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="49543-125">Request body</span></span>
<span data-ttu-id="49543-126">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49543-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="49543-127">由于**设备**资源支持[扩展](/graph/extensibility-overview)，您可以使用`POST`操作并创建它时将使用您自己的数据的自定义属性添加到设备实例。</span><span class="sxs-lookup"><span data-stu-id="49543-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="49543-128">响应</span><span class="sxs-lookup"><span data-stu-id="49543-128">Response</span></span>

<span data-ttu-id="49543-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49543-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49543-130">示例</span><span class="sxs-lookup"><span data-stu-id="49543-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49543-131">请求</span><span class="sxs-lookup"><span data-stu-id="49543-131">Request</span></span>
<span data-ttu-id="49543-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49543-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="49543-133">在请求正文中，提供 [device](../resources/device.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49543-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="49543-134">响应</span><span class="sxs-lookup"><span data-stu-id="49543-134">Response</span></span>
<span data-ttu-id="49543-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49543-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="49543-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="49543-138">See also</span></span>

- [<span data-ttu-id="49543-139">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="49543-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="49543-140">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="49543-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="49543-141">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="49543-141">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/device-post-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
