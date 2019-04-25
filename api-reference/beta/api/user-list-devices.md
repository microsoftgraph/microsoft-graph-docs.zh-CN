---
title: 列出用户设备
description: 获取支持 Project 罗马功能的用户设备列表。 这包括启动应用程序的功能, 或向应用程序发送数据或向其发送数据的功能。 在对我/设备执行 GET 呼叫后, 传入设备的 ID 以将命令发送到设备。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544275"
---
# <a name="list-user-devices"></a><span data-ttu-id="8b610-105">列出用户设备</span><span class="sxs-lookup"><span data-stu-id="8b610-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b610-106">获取支持 Project 罗马功能的用户设备列表。</span><span class="sxs-lookup"><span data-stu-id="8b610-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="8b610-107">这包括启动应用程序的功能, 或向应用程序发送数据或向其发送数据的功能。</span><span class="sxs-lookup"><span data-stu-id="8b610-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="8b610-108">在对我/设备执行 GET 呼叫后, 传入设备的 ID 以[将命令发送](send-device-command.md)到设备。</span><span class="sxs-lookup"><span data-stu-id="8b610-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b610-109">权限</span><span class="sxs-lookup"><span data-stu-id="8b610-109">Permissions</span></span>

<span data-ttu-id="8b610-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b610-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8b610-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b610-112">Permission type</span></span>      | <span data-ttu-id="8b610-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b610-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b610-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b610-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8b610-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b610-115">Not supported.</span></span>    |
|<span data-ttu-id="8b610-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b610-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b610-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="8b610-117">Device.Read</span></span>    |
|<span data-ttu-id="8b610-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b610-118">Application</span></span> | <span data-ttu-id="8b610-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b610-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b610-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b610-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="8b610-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b610-121">Request headers</span></span>

| <span data-ttu-id="8b610-122">标头</span><span class="sxs-lookup"><span data-stu-id="8b610-122">Header</span></span> |<span data-ttu-id="8b610-123">值</span><span class="sxs-lookup"><span data-stu-id="8b610-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="8b610-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b610-124">Authorization</span></span>| <span data-ttu-id="8b610-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b610-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8b610-127">接受</span><span class="sxs-lookup"><span data-stu-id="8b610-127">Accept</span></span> | <span data-ttu-id="8b610-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8b610-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b610-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b610-129">Request body</span></span>
<span data-ttu-id="8b610-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b610-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b610-131">响应</span><span class="sxs-lookup"><span data-stu-id="8b610-131">Response</span></span>

<span data-ttu-id="8b610-132">如果成功, 此方法在响应正文中返回一个200响应代码和用户设备属性。</span><span class="sxs-lookup"><span data-stu-id="8b610-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="8b610-133">示例</span><span class="sxs-lookup"><span data-stu-id="8b610-133">Example</span></span>
<span data-ttu-id="8b610-134">本示例将返回用户的设备列表。</span><span class="sxs-lookup"><span data-stu-id="8b610-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="8b610-135">若要使用`me/devices/{id}/command`命令设备, 您需要获取返回的设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="8b610-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="8b610-136">请求</span><span class="sxs-lookup"><span data-stu-id="8b610-136">Request</span></span>

<span data-ttu-id="8b610-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8b610-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="8b610-138">响应</span><span class="sxs-lookup"><span data-stu-id="8b610-138">Response</span></span>

<span data-ttu-id="8b610-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8b610-139">The following is an example of the response.</span></span> <span data-ttu-id="8b610-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8b610-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8b610-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8b610-141">All of the properties will be returned from an actual call.</span></span>

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
