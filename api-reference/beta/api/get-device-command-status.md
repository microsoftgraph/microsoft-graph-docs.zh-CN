---
title: 获取设备命令状态
description: 获取设备上的命令的状态。 状态代码的完整列表，请参阅 actionStatus 的列表。
localization_priority: Normal
ms.openlocfilehash: 9dca743a50f248abee76fb4d54352df3d400ada1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883130"
---
# <a name="get-device-command-status"></a><span data-ttu-id="f5c11-104">获取设备命令状态</span><span class="sxs-lookup"><span data-stu-id="f5c11-104">Get device command status</span></span>

> <span data-ttu-id="f5c11-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f5c11-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5c11-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5c11-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5c11-107">获取设备上的命令的状态。</span><span class="sxs-lookup"><span data-stu-id="f5c11-107">Get the status of a command on a device.</span></span> <span data-ttu-id="f5c11-108">状态代码的完整列表，请参阅[actionStatus 的列表](#list-of-actionstatus)。</span><span class="sxs-lookup"><span data-stu-id="f5c11-108">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5c11-109">权限</span><span class="sxs-lookup"><span data-stu-id="f5c11-109">Permissions</span></span>

<span data-ttu-id="f5c11-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5c11-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5c11-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5c11-112">Permission type</span></span>      | <span data-ttu-id="f5c11-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5c11-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5c11-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5c11-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f5c11-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5c11-115">Not supported.</span></span>    |
|<span data-ttu-id="f5c11-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5c11-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5c11-117">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f5c11-117">Device.Command</span></span>    |
|<span data-ttu-id="f5c11-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5c11-118">Application</span></span> | <span data-ttu-id="f5c11-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5c11-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5c11-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5c11-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5c11-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5c11-121">Request headers</span></span>

| <span data-ttu-id="f5c11-122">标头</span><span class="sxs-lookup"><span data-stu-id="f5c11-122">Header</span></span> |<span data-ttu-id="f5c11-123">值</span><span class="sxs-lookup"><span data-stu-id="f5c11-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="f5c11-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5c11-124">Authorization</span></span>| <span data-ttu-id="f5c11-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5c11-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f5c11-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f5c11-127">Accept</span></span> | <span data-ttu-id="f5c11-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f5c11-128">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="f5c11-129">响应</span><span class="sxs-lookup"><span data-stu-id="f5c11-129">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="f5c11-130">ActionStatus 的列表</span><span class="sxs-lookup"><span data-stu-id="f5c11-130">List of actionStatus</span></span>

- <span data-ttu-id="f5c11-131">请求，/ / 命令已创建并正在等待处理</span><span class="sxs-lookup"><span data-stu-id="f5c11-131">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="f5c11-132">sentToTarget，/ / 命令已发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="f5c11-132">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="f5c11-133">执行 / / 目标设备确认收到该命令，并且正在执行它</span><span class="sxs-lookup"><span data-stu-id="f5c11-133">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="f5c11-134">完成，/ / 命令执行完毕</span><span class="sxs-lookup"><span data-stu-id="f5c11-134">completed, // Command execution completed</span></span>
- <span data-ttu-id="f5c11-135">failedToSend，/ / 服务未能发送到目标设备命令</span><span class="sxs-lookup"><span data-stu-id="f5c11-135">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="f5c11-136">executionFailed，/ / 命令执行失败</span><span class="sxs-lookup"><span data-stu-id="f5c11-136">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="f5c11-137">commandDropped，/ / 命令而丢弃客户端设备是否处于 ConnectedStandby 状态</span><span class="sxs-lookup"><span data-stu-id="f5c11-137">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="f5c11-138">取消，/ / 取消命令</span><span class="sxs-lookup"><span data-stu-id="f5c11-138">cancel, // Cancel the command</span></span>
- <span data-ttu-id="f5c11-139">正在取消，/ / 取消该命令</span><span class="sxs-lookup"><span data-stu-id="f5c11-139">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="f5c11-140">canceled、 / / 命令已被取消</span><span class="sxs-lookup"><span data-stu-id="f5c11-140">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="f5c11-141">重试，/ / 服务正在重试发送到目标的命令</span><span class="sxs-lookup"><span data-stu-id="f5c11-141">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="f5c11-142">过期，/ / 命令处理超过到期时间</span><span class="sxs-lookup"><span data-stu-id="f5c11-142">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="f5c11-143">错误: / / 内部处理命令时的错误</span><span class="sxs-lookup"><span data-stu-id="f5c11-143">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="f5c11-144">自定义 / / 自定义状态</span><span class="sxs-lookup"><span data-stu-id="f5c11-144">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="f5c11-145">示例</span><span class="sxs-lookup"><span data-stu-id="f5c11-145">Example</span></span>

<span data-ttu-id="f5c11-146">本示例中，您需要的设备 ID 和的命令的已颁发的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="f5c11-146">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f5c11-147">对的设备时发出 GET 返回 ID 调用`/me/devices`，并执行 POST 时，则返回 ID 的命令对调用`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="f5c11-147">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f5c11-148">请求</span><span class="sxs-lookup"><span data-stu-id="f5c11-148">Request</span></span>

<span data-ttu-id="f5c11-149">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5c11-149">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f5c11-150">响应</span><span class="sxs-lookup"><span data-stu-id="f5c11-150">Response</span></span>

<span data-ttu-id="f5c11-151">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f5c11-151">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="f5c11-152">获取命令负载</span><span class="sxs-lookup"><span data-stu-id="f5c11-152">Get command payload</span></span>

<span data-ttu-id="f5c11-153">获取响应负载设备上的特定操作。</span><span class="sxs-lookup"><span data-stu-id="f5c11-153">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="f5c11-154">响应负载用于查询应用程序服务时返回带数据。</span><span class="sxs-lookup"><span data-stu-id="f5c11-154">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="f5c11-155">权限</span><span class="sxs-lookup"><span data-stu-id="f5c11-155">Permissions</span></span>

<span data-ttu-id="f5c11-p108">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5c11-p108">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5c11-158">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5c11-158">Permission type</span></span>      | <span data-ttu-id="f5c11-159">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5c11-159">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5c11-160">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5c11-160">Delegated (work or school account)</span></span> | <span data-ttu-id="f5c11-161">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5c11-161">Not supported.</span></span>    |
|<span data-ttu-id="f5c11-162">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5c11-162">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5c11-163">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f5c11-163">Device.Command</span></span>    |
|<span data-ttu-id="f5c11-164">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5c11-164">Application</span></span> | <span data-ttu-id="f5c11-165">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5c11-165">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="f5c11-166">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5c11-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="f5c11-167">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5c11-167">Request headers</span></span>

| <span data-ttu-id="f5c11-168">标头</span><span class="sxs-lookup"><span data-stu-id="f5c11-168">Header</span></span> |<span data-ttu-id="f5c11-169">值</span><span class="sxs-lookup"><span data-stu-id="f5c11-169">Value</span></span>
|:----|:------|
|<span data-ttu-id="f5c11-170">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5c11-170">Authorization</span></span>| <span data-ttu-id="f5c11-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5c11-p109">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f5c11-173">Accept</span><span class="sxs-lookup"><span data-stu-id="f5c11-173">Accept</span></span> | <span data-ttu-id="f5c11-174">application/json</span><span class="sxs-lookup"><span data-stu-id="f5c11-174">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="f5c11-175">响应</span><span class="sxs-lookup"><span data-stu-id="f5c11-175">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="f5c11-176">示例</span><span class="sxs-lookup"><span data-stu-id="f5c11-176">Example</span></span>

<span data-ttu-id="f5c11-177">本示例中，您需要的设备 ID 和的命令的已颁发的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="f5c11-177">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f5c11-178">在呼叫的设备时发出 GET 返回 ID `/me/devices`，并执行 POST 时，则返回 ID 的命令对调用`/me/devices/{id}/command`。</span><span class="sxs-lookup"><span data-stu-id="f5c11-178">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f5c11-179">请求</span><span class="sxs-lookup"><span data-stu-id="f5c11-179">Request</span></span>

<span data-ttu-id="f5c11-180">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5c11-180">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f5c11-181">响应</span><span class="sxs-lookup"><span data-stu-id="f5c11-181">Response</span></span>

<span data-ttu-id="f5c11-182">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f5c11-182">The following example shows the response.</span></span>

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
