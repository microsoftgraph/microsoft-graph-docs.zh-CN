---
title: 获取设备命令状态
description: 获取设备上命令的状态。 有关状态代码的完整列表，请参阅 actionStatus 列表。
localization_priority: Normal
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: c0747438a9921f2ed6f3ccf1ee551f4aced70fcb
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515962"
---
# <a name="get-device-command-status"></a><span data-ttu-id="6eb4a-104">获取设备命令状态</span><span class="sxs-lookup"><span data-stu-id="6eb4a-104">Get device command status</span></span>

<span data-ttu-id="6eb4a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eb4a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb4a-106">获取设备上命令的状态。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-106">Get the status of a command on a device.</span></span> <span data-ttu-id="6eb4a-107">有关状态代码的完整列表，请参阅 [actionStatus 列表](#list-of-actionstatus)。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-107">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="6eb4a-108">权限</span><span class="sxs-lookup"><span data-stu-id="6eb4a-108">Permissions</span></span>

<span data-ttu-id="6eb4a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb4a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eb4a-111">Permission type</span></span>      | <span data-ttu-id="6eb4a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6eb4a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6eb4a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb4a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6eb4a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-114">Not supported.</span></span>    |
|<span data-ttu-id="6eb4a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb4a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eb4a-116">Device.Command</span><span class="sxs-lookup"><span data-stu-id="6eb4a-116">Device.Command</span></span>    |
|<span data-ttu-id="6eb4a-117">Application</span><span class="sxs-lookup"><span data-stu-id="6eb4a-117">Application</span></span> | <span data-ttu-id="6eb4a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6eb4a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eb4a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6eb4a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eb4a-120">Request headers</span></span>

| <span data-ttu-id="6eb4a-121">标头</span><span class="sxs-lookup"><span data-stu-id="6eb4a-121">Header</span></span> |<span data-ttu-id="6eb4a-122">值</span><span class="sxs-lookup"><span data-stu-id="6eb4a-122">Value</span></span>
|:----|:------|
|<span data-ttu-id="6eb4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eb4a-123">Authorization</span></span>| <span data-ttu-id="6eb4a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="6eb4a-126">接受</span><span class="sxs-lookup"><span data-stu-id="6eb4a-126">Accept</span></span> | <span data-ttu-id="6eb4a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6eb4a-127">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="6eb4a-128">响应</span><span class="sxs-lookup"><span data-stu-id="6eb4a-128">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="6eb4a-129">actionStatus 列表</span><span class="sxs-lookup"><span data-stu-id="6eb4a-129">List of actionStatus</span></span>

- <span data-ttu-id="6eb4a-130">requesting， // Command has been created and is waiting to be processed</span><span class="sxs-lookup"><span data-stu-id="6eb4a-130">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="6eb4a-131">sentToTarget，// 命令已发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="6eb4a-131">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="6eb4a-132">执行，// 目标设备确认收到命令并正在执行该命令</span><span class="sxs-lookup"><span data-stu-id="6eb4a-132">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="6eb4a-133">已完成，// 命令执行已完成</span><span class="sxs-lookup"><span data-stu-id="6eb4a-133">completed, // Command execution completed</span></span>
- <span data-ttu-id="6eb4a-134">failedToSend， // Service 未能将命令发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="6eb4a-134">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="6eb4a-135">executionFailed， // 命令执行失败</span><span class="sxs-lookup"><span data-stu-id="6eb4a-135">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="6eb4a-136">commandDropped， // 如果设备位于 ConnectedStandby 状态，则客户端丢弃的命令</span><span class="sxs-lookup"><span data-stu-id="6eb4a-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="6eb4a-137">cancel， // Cancel the command</span><span class="sxs-lookup"><span data-stu-id="6eb4a-137">cancel, // Cancel the command</span></span>
- <span data-ttu-id="6eb4a-138">取消，// 取消命令</span><span class="sxs-lookup"><span data-stu-id="6eb4a-138">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="6eb4a-139">已取消，// 命令已取消</span><span class="sxs-lookup"><span data-stu-id="6eb4a-139">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="6eb4a-140">retry， // Service 正在重试以将命令发送到目标</span><span class="sxs-lookup"><span data-stu-id="6eb4a-140">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="6eb4a-141">已过期，// 命令处理超出过期时间</span><span class="sxs-lookup"><span data-stu-id="6eb4a-141">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="6eb4a-142">错误，// 处理命令时出现内部错误</span><span class="sxs-lookup"><span data-stu-id="6eb4a-142">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="6eb4a-143">自定义 // 自定义状态</span><span class="sxs-lookup"><span data-stu-id="6eb4a-143">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="6eb4a-144">示例</span><span class="sxs-lookup"><span data-stu-id="6eb4a-144">Example</span></span>

<span data-ttu-id="6eb4a-145">在此例中，你将需要设备的 ID 和已颁发给设备的命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-145">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="6eb4a-146">发出 GET 调用时，将返回设备 ID，对 .进行 POST 调用时 `/me/devices` 将返回命令 `/me/devices/{id}/command` ID。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-146">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="6eb4a-147">请求</span><span class="sxs-lookup"><span data-stu-id="6eb4a-147">Request</span></span>

<span data-ttu-id="6eb4a-148">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="6eb4a-149">响应</span><span class="sxs-lookup"><span data-stu-id="6eb4a-149">Response</span></span>

<span data-ttu-id="6eb4a-150">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-150">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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


## <a name="get-command-payload"></a><span data-ttu-id="6eb4a-151">获取命令有效负载</span><span class="sxs-lookup"><span data-stu-id="6eb4a-151">Get command payload</span></span>

<span data-ttu-id="6eb4a-152">获取设备上特定操作的响应负载。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-152">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="6eb4a-153">查询应用服务以返回数据时，使用响应有效负载。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-153">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="6eb4a-154">权限</span><span class="sxs-lookup"><span data-stu-id="6eb4a-154">Permissions</span></span>

<span data-ttu-id="6eb4a-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb4a-157">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eb4a-157">Permission type</span></span>      | <span data-ttu-id="6eb4a-158">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6eb4a-158">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6eb4a-159">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb4a-159">Delegated (work or school account)</span></span> | <span data-ttu-id="6eb4a-160">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-160">Not supported.</span></span>    |
|<span data-ttu-id="6eb4a-161">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb4a-161">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eb4a-162">Device.Command</span><span class="sxs-lookup"><span data-stu-id="6eb4a-162">Device.Command</span></span>    |
|<span data-ttu-id="6eb4a-163">Application</span><span class="sxs-lookup"><span data-stu-id="6eb4a-163">Application</span></span> | <span data-ttu-id="6eb4a-164">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-164">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="6eb4a-165">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eb4a-165">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="6eb4a-166">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eb4a-166">Request headers</span></span>

| <span data-ttu-id="6eb4a-167">标头</span><span class="sxs-lookup"><span data-stu-id="6eb4a-167">Header</span></span> |<span data-ttu-id="6eb4a-168">值</span><span class="sxs-lookup"><span data-stu-id="6eb4a-168">Value</span></span>
|:----|:------|
|<span data-ttu-id="6eb4a-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eb4a-169">Authorization</span></span>| <span data-ttu-id="6eb4a-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="6eb4a-172">接受</span><span class="sxs-lookup"><span data-stu-id="6eb4a-172">Accept</span></span> | <span data-ttu-id="6eb4a-173">application/json</span><span class="sxs-lookup"><span data-stu-id="6eb4a-173">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="6eb4a-174">响应</span><span class="sxs-lookup"><span data-stu-id="6eb4a-174">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="6eb4a-175">示例</span><span class="sxs-lookup"><span data-stu-id="6eb4a-175">Example</span></span>

<span data-ttu-id="6eb4a-176">在此例中，你将需要设备的 ID 和已颁发给设备的命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-176">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="6eb4a-177">发出 GET 调用时，将返回设备 ID，对 设备 ID 执行 POST 调用时 `/me/devices` ，将返回命令 `/me/devices/{id}/command` ID。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-177">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="6eb4a-178">请求</span><span class="sxs-lookup"><span data-stu-id="6eb4a-178">Request</span></span>

<span data-ttu-id="6eb4a-179">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-179">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="6eb4a-180">响应</span><span class="sxs-lookup"><span data-stu-id="6eb4a-180">Response</span></span>

<span data-ttu-id="6eb4a-181">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="6eb4a-181">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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


