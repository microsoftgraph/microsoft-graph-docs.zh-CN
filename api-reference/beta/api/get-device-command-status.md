---
title: 获取设备命令状态
description: 获取设备上的命令的状态。 状态代码的完整列表，请参阅 actionStatus 的列表。
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510111"
---
# <a name="get-device-command-status"></a><span data-ttu-id="9df7b-104">获取设备命令状态</span><span class="sxs-lookup"><span data-stu-id="9df7b-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df7b-105">获取设备上的命令的状态。</span><span class="sxs-lookup"><span data-stu-id="9df7b-105">Get the status of a command on a device.</span></span> <span data-ttu-id="9df7b-106">状态代码的完整列表，请参阅[actionStatus 的列表](#list-of-actionstatus)。</span><span class="sxs-lookup"><span data-stu-id="9df7b-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="9df7b-107">权限</span><span class="sxs-lookup"><span data-stu-id="9df7b-107">Permissions</span></span>

<span data-ttu-id="9df7b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9df7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9df7b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9df7b-110">Permission type</span></span>      | <span data-ttu-id="9df7b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9df7b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9df7b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9df7b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9df7b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9df7b-113">Not supported.</span></span>    |
|<span data-ttu-id="9df7b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9df7b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9df7b-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="9df7b-115">Device.Command</span></span>    |
|<span data-ttu-id="9df7b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9df7b-116">Application</span></span> | <span data-ttu-id="9df7b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9df7b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9df7b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9df7b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9df7b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9df7b-119">Request headers</span></span>

| <span data-ttu-id="9df7b-120">标头</span><span class="sxs-lookup"><span data-stu-id="9df7b-120">Header</span></span> |<span data-ttu-id="9df7b-121">值</span><span class="sxs-lookup"><span data-stu-id="9df7b-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="9df7b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9df7b-122">Authorization</span></span>| <span data-ttu-id="9df7b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9df7b-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9df7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9df7b-125">Accept</span></span> | <span data-ttu-id="9df7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9df7b-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="9df7b-127">响应</span><span class="sxs-lookup"><span data-stu-id="9df7b-127">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a><span data-ttu-id="9df7b-128">ActionStatus 的列表</span><span class="sxs-lookup"><span data-stu-id="9df7b-128">List of actionStatus</span></span>

- <span data-ttu-id="9df7b-129">请求，/ / 命令已创建并正在等待处理</span><span class="sxs-lookup"><span data-stu-id="9df7b-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="9df7b-130">sentToTarget，/ / 命令已发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="9df7b-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="9df7b-131">执行 / / 目标设备确认收到该命令，并且正在执行它</span><span class="sxs-lookup"><span data-stu-id="9df7b-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="9df7b-132">完成，/ / 命令执行完毕</span><span class="sxs-lookup"><span data-stu-id="9df7b-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="9df7b-133">failedToSend，/ / 服务未能发送到目标设备命令</span><span class="sxs-lookup"><span data-stu-id="9df7b-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="9df7b-134">executionFailed，/ / 命令执行失败</span><span class="sxs-lookup"><span data-stu-id="9df7b-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="9df7b-135">commandDropped，/ / 命令而丢弃客户端设备是否处于 ConnectedStandby 状态</span><span class="sxs-lookup"><span data-stu-id="9df7b-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="9df7b-136">取消，/ / 取消命令</span><span class="sxs-lookup"><span data-stu-id="9df7b-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="9df7b-137">正在取消，/ / 取消该命令</span><span class="sxs-lookup"><span data-stu-id="9df7b-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="9df7b-138">canceled、 / / 命令已被取消</span><span class="sxs-lookup"><span data-stu-id="9df7b-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="9df7b-139">重试，/ / 服务正在重试发送到目标的命令</span><span class="sxs-lookup"><span data-stu-id="9df7b-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="9df7b-140">过期，/ / 命令处理超过到期时间</span><span class="sxs-lookup"><span data-stu-id="9df7b-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="9df7b-141">错误: / / 内部处理命令时的错误</span><span class="sxs-lookup"><span data-stu-id="9df7b-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="9df7b-142">自定义 / / 自定义状态</span><span class="sxs-lookup"><span data-stu-id="9df7b-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="9df7b-143">示例</span><span class="sxs-lookup"><span data-stu-id="9df7b-143">Example</span></span>

<span data-ttu-id="9df7b-144">本示例中，您需要的设备 ID 和的命令的已颁发的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="9df7b-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="9df7b-145">对的设备时发出 GET 返回 ID 调用`/me/devices`，并执行 POST 时，则返回 ID 的命令对调用`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="9df7b-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="9df7b-146">请求</span><span class="sxs-lookup"><span data-stu-id="9df7b-146">Request</span></span>

<span data-ttu-id="9df7b-147">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9df7b-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="9df7b-148">响应</span><span class="sxs-lookup"><span data-stu-id="9df7b-148">Response</span></span>

<span data-ttu-id="9df7b-149">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="9df7b-149">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a><span data-ttu-id="9df7b-150">获取命令负载</span><span class="sxs-lookup"><span data-stu-id="9df7b-150">Get command payload</span></span>

<span data-ttu-id="9df7b-151">获取响应负载设备上的特定操作。</span><span class="sxs-lookup"><span data-stu-id="9df7b-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="9df7b-152">响应负载用于查询应用程序服务时返回带数据。</span><span class="sxs-lookup"><span data-stu-id="9df7b-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="9df7b-153">权限</span><span class="sxs-lookup"><span data-stu-id="9df7b-153">Permissions</span></span>

<span data-ttu-id="9df7b-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9df7b-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9df7b-156">权限类型</span><span class="sxs-lookup"><span data-stu-id="9df7b-156">Permission type</span></span>      | <span data-ttu-id="9df7b-157">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9df7b-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9df7b-158">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9df7b-158">Delegated (work or school account)</span></span> | <span data-ttu-id="9df7b-159">不支持。</span><span class="sxs-lookup"><span data-stu-id="9df7b-159">Not supported.</span></span>    |
|<span data-ttu-id="9df7b-160">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9df7b-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9df7b-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="9df7b-161">Device.Command</span></span>    |
|<span data-ttu-id="9df7b-162">应用程序</span><span class="sxs-lookup"><span data-stu-id="9df7b-162">Application</span></span> | <span data-ttu-id="9df7b-163">不支持。</span><span class="sxs-lookup"><span data-stu-id="9df7b-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="9df7b-164">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9df7b-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="9df7b-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="9df7b-165">Request headers</span></span>

| <span data-ttu-id="9df7b-166">标头</span><span class="sxs-lookup"><span data-stu-id="9df7b-166">Header</span></span> |<span data-ttu-id="9df7b-167">值</span><span class="sxs-lookup"><span data-stu-id="9df7b-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="9df7b-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="9df7b-168">Authorization</span></span>| <span data-ttu-id="9df7b-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9df7b-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9df7b-171">Accept</span><span class="sxs-lookup"><span data-stu-id="9df7b-171">Accept</span></span> | <span data-ttu-id="9df7b-172">application/json</span><span class="sxs-lookup"><span data-stu-id="9df7b-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="9df7b-173">响应</span><span class="sxs-lookup"><span data-stu-id="9df7b-173">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a><span data-ttu-id="9df7b-174">示例</span><span class="sxs-lookup"><span data-stu-id="9df7b-174">Example</span></span>

<span data-ttu-id="9df7b-175">本示例中，您需要的设备 ID 和的命令的已颁发的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="9df7b-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="9df7b-176">在呼叫的设备时发出 GET 返回 ID `/me/devices`，并执行 POST 时，则返回 ID 的命令对调用`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="9df7b-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="9df7b-177">请求</span><span class="sxs-lookup"><span data-stu-id="9df7b-177">Request</span></span>

<span data-ttu-id="9df7b-178">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="9df7b-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="9df7b-179">响应</span><span class="sxs-lookup"><span data-stu-id="9df7b-179">Response</span></span>

<span data-ttu-id="9df7b-180">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="9df7b-180">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
