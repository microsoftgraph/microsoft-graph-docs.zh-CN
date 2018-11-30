---
title: 列出用户设备
description: 获取支持 Project Rome 功能的用户设备的列表。 这包括以启动应用程序，或者邮件或将数据发送到应用程序的能力。 在您之后执行 GET 呼叫我/设备，传递中要向您的设备发送命令的设备 ID。
ms.openlocfilehash: b9e6132af0e16deae1a4175bfc811f74c18e1ae6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048608"
---
# <a name="list-user-devices"></a><span data-ttu-id="f8ee1-105">列出用户设备</span><span class="sxs-lookup"><span data-stu-id="f8ee1-105">List user devices</span></span>

> <span data-ttu-id="f8ee1-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8ee1-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8ee1-108">获取支持 Project Rome 功能的用户设备的列表。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-108">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="f8ee1-109">这包括以启动应用程序，或者邮件或将数据发送到应用程序的能力。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-109">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="f8ee1-110">在您之后执行 GET 呼叫我/设备中的设备 ID 传递到向设备[发送命令](send-device-command.md)。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-110">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8ee1-111">权限</span><span class="sxs-lookup"><span data-stu-id="f8ee1-111">Permissions</span></span>

<span data-ttu-id="f8ee1-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f8ee1-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8ee1-114">Permission type</span></span>      | <span data-ttu-id="f8ee1-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8ee1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8ee1-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8ee1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f8ee1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-117">Not supported.</span></span>    |
|<span data-ttu-id="f8ee1-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8ee1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8ee1-119">Device.Read</span><span class="sxs-lookup"><span data-stu-id="f8ee1-119">Device.Read</span></span>    |
|<span data-ttu-id="f8ee1-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8ee1-120">Application</span></span> | <span data-ttu-id="f8ee1-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8ee1-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8ee1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="f8ee1-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8ee1-123">Request headers</span></span>

| <span data-ttu-id="f8ee1-124">标头</span><span class="sxs-lookup"><span data-stu-id="f8ee1-124">Header</span></span> |<span data-ttu-id="f8ee1-125">值</span><span class="sxs-lookup"><span data-stu-id="f8ee1-125">Value</span></span>
|:----|:------|
|<span data-ttu-id="f8ee1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8ee1-126">Authorization</span></span>| <span data-ttu-id="f8ee1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f8ee1-129">Accept</span><span class="sxs-lookup"><span data-stu-id="f8ee1-129">Accept</span></span> | <span data-ttu-id="f8ee1-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f8ee1-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8ee1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8ee1-131">Request body</span></span>
<span data-ttu-id="f8ee1-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8ee1-133">响应</span><span class="sxs-lookup"><span data-stu-id="f8ee1-133">Response</span></span>

<span data-ttu-id="f8ee1-134">如果成功，此方法将在响应正文中返回一个 200 响应代码以及用户设备属性。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-134">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="f8ee1-135">示例</span><span class="sxs-lookup"><span data-stu-id="f8ee1-135">Example</span></span>
<span data-ttu-id="f8ee1-136">本示例将返回用户的设备的列表。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-136">This example will return the list of devices for a user.</span></span> <span data-ttu-id="f8ee1-137">若要命令设备使用`me/devices/{id}/command`，您将需要获取的设备，则返回的 ID。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-137">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="f8ee1-138">请求</span><span class="sxs-lookup"><span data-stu-id="f8ee1-138">Request</span></span>

<span data-ttu-id="f8ee1-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f8ee1-140">响应</span><span class="sxs-lookup"><span data-stu-id="f8ee1-140">Response</span></span>

<span data-ttu-id="f8ee1-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-141">The following is an example of the response.</span></span> <span data-ttu-id="f8ee1-142">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8ee1-143">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8ee1-143">All of the properties will be returned from an actual call.</span></span>

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
