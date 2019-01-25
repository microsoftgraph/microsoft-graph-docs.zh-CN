---
title: 列出用户设备
description: 获取支持 Project Rome 功能的用户设备的列表。 这包括以启动应用程序，或者邮件或将数据发送到应用程序的能力。 在您之后执行 GET 呼叫我/设备，传递中要向您的设备发送命令的设备 ID。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509523"
---
# <a name="list-user-devices"></a><span data-ttu-id="7c00a-105">列出用户设备</span><span class="sxs-lookup"><span data-stu-id="7c00a-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c00a-106">获取支持 Project Rome 功能的用户设备的列表。</span><span class="sxs-lookup"><span data-stu-id="7c00a-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="7c00a-107">这包括以启动应用程序，或者邮件或将数据发送到应用程序的能力。</span><span class="sxs-lookup"><span data-stu-id="7c00a-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="7c00a-108">在您之后执行 GET 呼叫我/设备中的设备 ID 传递到向设备[发送命令](send-device-command.md)。</span><span class="sxs-lookup"><span data-stu-id="7c00a-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c00a-109">权限</span><span class="sxs-lookup"><span data-stu-id="7c00a-109">Permissions</span></span>

<span data-ttu-id="7c00a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c00a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7c00a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c00a-112">Permission type</span></span>      | <span data-ttu-id="7c00a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c00a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c00a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c00a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7c00a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c00a-115">Not supported.</span></span>    |
|<span data-ttu-id="7c00a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c00a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c00a-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="7c00a-117">Device.Read</span></span>    |
|<span data-ttu-id="7c00a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c00a-118">Application</span></span> | <span data-ttu-id="7c00a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c00a-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c00a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c00a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="7c00a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c00a-121">Request headers</span></span>

| <span data-ttu-id="7c00a-122">标头</span><span class="sxs-lookup"><span data-stu-id="7c00a-122">Header</span></span> |<span data-ttu-id="7c00a-123">值</span><span class="sxs-lookup"><span data-stu-id="7c00a-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="7c00a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c00a-124">Authorization</span></span>| <span data-ttu-id="7c00a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c00a-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="7c00a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7c00a-127">Accept</span></span> | <span data-ttu-id="7c00a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7c00a-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c00a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c00a-129">Request body</span></span>
<span data-ttu-id="7c00a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c00a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c00a-131">响应</span><span class="sxs-lookup"><span data-stu-id="7c00a-131">Response</span></span>

<span data-ttu-id="7c00a-132">如果成功，此方法将在响应正文中返回一个 200 响应代码以及用户设备属性。</span><span class="sxs-lookup"><span data-stu-id="7c00a-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="7c00a-133">示例</span><span class="sxs-lookup"><span data-stu-id="7c00a-133">Example</span></span>
<span data-ttu-id="7c00a-134">本示例将返回用户的设备的列表。</span><span class="sxs-lookup"><span data-stu-id="7c00a-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="7c00a-135">若要命令设备使用`me/devices/{id}/command`，您将需要获取的设备，则返回的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c00a-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="7c00a-136">请求</span><span class="sxs-lookup"><span data-stu-id="7c00a-136">Request</span></span>

<span data-ttu-id="7c00a-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c00a-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="7c00a-138">响应</span><span class="sxs-lookup"><span data-stu-id="7c00a-138">Response</span></span>

<span data-ttu-id="7c00a-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7c00a-139">The following is an example of the response.</span></span> <span data-ttu-id="7c00a-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7c00a-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7c00a-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c00a-141">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
