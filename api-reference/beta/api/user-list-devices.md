---
title: 列出用户设备
description: 获取支持 Project 罗马功能的用户设备列表。 这包括启动应用程序的功能，或向应用程序发送数据或向其发送数据的功能。 在对我/设备执行 GET 呼叫后，传入设备的 ID 以将命令发送到设备。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: acd31b5d5b115646716199842d862bf6637ea504
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107701"
---
# <a name="list-user-devices"></a><span data-ttu-id="55891-105">列出用户设备</span><span class="sxs-lookup"><span data-stu-id="55891-105">List user devices</span></span>

<span data-ttu-id="55891-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55891-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55891-107">获取支持 Project 罗马功能的用户设备列表。</span><span class="sxs-lookup"><span data-stu-id="55891-107">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="55891-108">这包括启动应用程序的功能，或向应用程序发送数据或向其发送数据的功能。</span><span class="sxs-lookup"><span data-stu-id="55891-108">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="55891-109">在对我/设备执行 GET 呼叫后，传入设备的 ID 以[将命令发送](send-device-command.md)到设备。</span><span class="sxs-lookup"><span data-stu-id="55891-109">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="55891-110">权限</span><span class="sxs-lookup"><span data-stu-id="55891-110">Permissions</span></span>

<span data-ttu-id="55891-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55891-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="55891-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="55891-113">Permission type</span></span>      | <span data-ttu-id="55891-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55891-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55891-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55891-115">Delegated (work or school account)</span></span> | <span data-ttu-id="55891-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55891-116">Not supported.</span></span>    |
|<span data-ttu-id="55891-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55891-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55891-118">Device.Read</span><span class="sxs-lookup"><span data-stu-id="55891-118">Device.Read</span></span>    |
|<span data-ttu-id="55891-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="55891-119">Application</span></span> | <span data-ttu-id="55891-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="55891-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55891-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55891-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="55891-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="55891-122">Request headers</span></span>

| <span data-ttu-id="55891-123">标头</span><span class="sxs-lookup"><span data-stu-id="55891-123">Header</span></span> |<span data-ttu-id="55891-124">值</span><span class="sxs-lookup"><span data-stu-id="55891-124">Value</span></span>
|:----|:------|
|<span data-ttu-id="55891-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="55891-125">Authorization</span></span>| <span data-ttu-id="55891-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55891-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="55891-128">接受</span><span class="sxs-lookup"><span data-stu-id="55891-128">Accept</span></span> | <span data-ttu-id="55891-129">application/json</span><span class="sxs-lookup"><span data-stu-id="55891-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="55891-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="55891-130">Request body</span></span>
<span data-ttu-id="55891-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55891-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55891-132">响应</span><span class="sxs-lookup"><span data-stu-id="55891-132">Response</span></span>

<span data-ttu-id="55891-133">如果成功，此方法在响应正文中返回一个200响应代码和用户设备属性。</span><span class="sxs-lookup"><span data-stu-id="55891-133">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="55891-134">示例</span><span class="sxs-lookup"><span data-stu-id="55891-134">Example</span></span>
<span data-ttu-id="55891-135">本示例将返回用户的设备列表。</span><span class="sxs-lookup"><span data-stu-id="55891-135">This example will return the list of devices for a user.</span></span> <span data-ttu-id="55891-136">若要使用`me/devices/{id}/command`命令设备，您需要获取返回的设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="55891-136">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="55891-137">请求</span><span class="sxs-lookup"><span data-stu-id="55891-137">Request</span></span>

<span data-ttu-id="55891-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="55891-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="55891-139">响应</span><span class="sxs-lookup"><span data-stu-id="55891-139">Response</span></span>

<span data-ttu-id="55891-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55891-140">The following is an example of the response.</span></span> <span data-ttu-id="55891-141">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="55891-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="55891-142">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55891-142">All of the properties will be returned from an actual call.</span></span>

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
