---
title: 列出用户设备
description: 获取支持 Project Rome 功能的用户设备列表。 这包括启动应用、发送消息或将数据发送到应用程序的能力。 在"我/设备"上执行 GET 呼叫后，请传递设备的 ID 以向设备发送命令。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b1c2b884b00298fd2b79a85b0ed3fe8f412b2736
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721633"
---
# <a name="list-user-devices"></a><span data-ttu-id="e1454-105">列出用户设备</span><span class="sxs-lookup"><span data-stu-id="e1454-105">List user devices</span></span>

<span data-ttu-id="e1454-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1454-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1454-107">获取支持 Project Rome 功能的用户设备列表。</span><span class="sxs-lookup"><span data-stu-id="e1454-107">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="e1454-108">这包括启动应用、发送消息或将数据发送到应用程序的能力。</span><span class="sxs-lookup"><span data-stu-id="e1454-108">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="e1454-109">在"我/设备"上执行 GET 呼叫后，请传递设备的 ID 以 [向](send-device-command.md) 设备发送命令。</span><span class="sxs-lookup"><span data-stu-id="e1454-109">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1454-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="e1454-110">Permissions</span></span>

<span data-ttu-id="e1454-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1454-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e1454-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1454-113">Permission type</span></span>      | <span data-ttu-id="e1454-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1454-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1454-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1454-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e1454-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1454-116">Not supported.</span></span>    |
|<span data-ttu-id="e1454-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1454-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1454-118">Device.Read</span><span class="sxs-lookup"><span data-stu-id="e1454-118">Device.Read</span></span>    |
|<span data-ttu-id="e1454-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1454-119">Application</span></span> | <span data-ttu-id="e1454-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1454-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1454-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1454-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="e1454-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1454-122">Request headers</span></span>

| <span data-ttu-id="e1454-123">标头</span><span class="sxs-lookup"><span data-stu-id="e1454-123">Header</span></span> |<span data-ttu-id="e1454-124">值</span><span class="sxs-lookup"><span data-stu-id="e1454-124">Value</span></span>
|:----|:------|
|<span data-ttu-id="e1454-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1454-125">Authorization</span></span>| <span data-ttu-id="e1454-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1454-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e1454-128">接受</span><span class="sxs-lookup"><span data-stu-id="e1454-128">Accept</span></span> | <span data-ttu-id="e1454-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e1454-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1454-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1454-130">Request body</span></span>
<span data-ttu-id="e1454-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1454-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1454-132">响应</span><span class="sxs-lookup"><span data-stu-id="e1454-132">Response</span></span>

<span data-ttu-id="e1454-133">如果成功，此方法在响应正文中返回 200 个响应代码和用户设备属性。</span><span class="sxs-lookup"><span data-stu-id="e1454-133">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a><span data-ttu-id="e1454-134">示例</span><span class="sxs-lookup"><span data-stu-id="e1454-134">Example</span></span>
<span data-ttu-id="e1454-135">此示例将返回用户的设备列表。</span><span class="sxs-lookup"><span data-stu-id="e1454-135">This example will return the list of devices for a user.</span></span> <span data-ttu-id="e1454-136">若要使用命令设备 `me/devices/{id}/command` ，你将需要获取返回的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="e1454-136">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="e1454-137">请求</span><span class="sxs-lookup"><span data-stu-id="e1454-137">Request</span></span>

<span data-ttu-id="e1454-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e1454-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="e1454-139">响应</span><span class="sxs-lookup"><span data-stu-id="e1454-139">Response</span></span>

<span data-ttu-id="e1454-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e1454-140">The following is an example of the response.</span></span> <span data-ttu-id="e1454-141">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e1454-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e1454-142">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1454-142">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```


