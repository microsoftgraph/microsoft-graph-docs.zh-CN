---
title: 获取设备命令状态
description: 获取设备上命令的状态。 有关状态代码的完整列表, 请参阅 actionStatus 的列表。
localization_priority: Normal
ms.openlocfilehash: 9b914cdfde78ce50df812acb09dc034c978c7e08
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324995"
---
# <a name="get-device-command-status"></a><span data-ttu-id="1a697-104">获取设备命令状态</span><span class="sxs-lookup"><span data-stu-id="1a697-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a697-105">获取设备上命令的状态。</span><span class="sxs-lookup"><span data-stu-id="1a697-105">Get the status of a command on a device.</span></span> <span data-ttu-id="1a697-106">有关状态代码的完整列表, 请参阅[actionStatus 的列表](#list-of-actionstatus)。</span><span class="sxs-lookup"><span data-stu-id="1a697-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a697-107">权限</span><span class="sxs-lookup"><span data-stu-id="1a697-107">Permissions</span></span>

<span data-ttu-id="1a697-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a697-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a697-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a697-110">Permission type</span></span>      | <span data-ttu-id="1a697-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a697-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a697-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a697-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a697-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a697-113">Not supported.</span></span>    |
|<span data-ttu-id="1a697-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a697-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a697-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="1a697-115">Device.Command</span></span>    |
|<span data-ttu-id="1a697-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a697-116">Application</span></span> | <span data-ttu-id="1a697-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a697-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a697-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a697-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a697-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a697-119">Request headers</span></span>

| <span data-ttu-id="1a697-120">标头</span><span class="sxs-lookup"><span data-stu-id="1a697-120">Header</span></span> |<span data-ttu-id="1a697-121">值</span><span class="sxs-lookup"><span data-stu-id="1a697-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="1a697-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a697-122">Authorization</span></span>| <span data-ttu-id="1a697-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a697-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1a697-125">接受</span><span class="sxs-lookup"><span data-stu-id="1a697-125">Accept</span></span> | <span data-ttu-id="1a697-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a697-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="1a697-127">响应</span><span class="sxs-lookup"><span data-stu-id="1a697-127">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="1a697-128">actionStatus 列表</span><span class="sxs-lookup"><span data-stu-id="1a697-128">List of actionStatus</span></span>

- <span data-ttu-id="1a697-129">请求、//命令已创建, 正在等待处理</span><span class="sxs-lookup"><span data-stu-id="1a697-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="1a697-130">已将 sentToTarget、//命令发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="1a697-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="1a697-131">正在执行、//目标设备确认了命令的接收并正在执行该命令</span><span class="sxs-lookup"><span data-stu-id="1a697-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="1a697-132">已完成,//命令执行已完成</span><span class="sxs-lookup"><span data-stu-id="1a697-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="1a697-133">failedToSend,//服务无法将命令发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="1a697-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="1a697-134">executionFailed,//命令执行失败</span><span class="sxs-lookup"><span data-stu-id="1a697-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="1a697-135">commandDropped、//设备处于 ConnectedStandby 状态时由客户端丢弃的命令</span><span class="sxs-lookup"><span data-stu-id="1a697-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="1a697-136">取消、//取消命令</span><span class="sxs-lookup"><span data-stu-id="1a697-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="1a697-137">取消、//取消命令</span><span class="sxs-lookup"><span data-stu-id="1a697-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="1a697-138">已取消,//命令已取消</span><span class="sxs-lookup"><span data-stu-id="1a697-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="1a697-139">重试,//服务正在重试将命令发送到目标</span><span class="sxs-lookup"><span data-stu-id="1a697-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="1a697-140">已过期,//命令处理超过了过期时间</span><span class="sxs-lookup"><span data-stu-id="1a697-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="1a697-141">处理命令时出现错误,//内部错误</span><span class="sxs-lookup"><span data-stu-id="1a697-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="1a697-142">自定义//自定义状态</span><span class="sxs-lookup"><span data-stu-id="1a697-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="1a697-143">示例</span><span class="sxs-lookup"><span data-stu-id="1a697-143">Example</span></span>

<span data-ttu-id="1a697-144">在此示例中, 将需要设备的 id 以及已颁发给设备的命令的 id。</span><span class="sxs-lookup"><span data-stu-id="1a697-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="1a697-145">在发出对`/me/devices`的 GET 呼叫时, 将返回设备 ID, 并且在对`/me/devices/{id}/command`进行开机自检呼叫时返回命令 id。</span><span class="sxs-lookup"><span data-stu-id="1a697-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="1a697-146">请求</span><span class="sxs-lookup"><span data-stu-id="1a697-146">Request</span></span>

<span data-ttu-id="1a697-147">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a697-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="1a697-148">响应</span><span class="sxs-lookup"><span data-stu-id="1a697-148">Response</span></span>

<span data-ttu-id="1a697-149">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="1a697-149">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="1a697-150">获取命令有效负载</span><span class="sxs-lookup"><span data-stu-id="1a697-150">Get command payload</span></span>

<span data-ttu-id="1a697-151">获取设备上特定操作的响应负载。</span><span class="sxs-lookup"><span data-stu-id="1a697-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="1a697-152">在查询应用程序服务以传送数据时, 将使用响应负载。</span><span class="sxs-lookup"><span data-stu-id="1a697-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="1a697-153">权限</span><span class="sxs-lookup"><span data-stu-id="1a697-153">Permissions</span></span>

<span data-ttu-id="1a697-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a697-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a697-156">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a697-156">Permission type</span></span>      | <span data-ttu-id="1a697-157">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a697-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a697-158">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a697-158">Delegated (work or school account)</span></span> | <span data-ttu-id="1a697-159">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a697-159">Not supported.</span></span>    |
|<span data-ttu-id="1a697-160">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a697-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a697-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="1a697-161">Device.Command</span></span>    |
|<span data-ttu-id="1a697-162">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a697-162">Application</span></span> | <span data-ttu-id="1a697-163">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a697-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="1a697-164">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a697-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="1a697-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a697-165">Request headers</span></span>

| <span data-ttu-id="1a697-166">标头</span><span class="sxs-lookup"><span data-stu-id="1a697-166">Header</span></span> |<span data-ttu-id="1a697-167">值</span><span class="sxs-lookup"><span data-stu-id="1a697-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="1a697-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a697-168">Authorization</span></span>| <span data-ttu-id="1a697-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a697-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1a697-171">接受</span><span class="sxs-lookup"><span data-stu-id="1a697-171">Accept</span></span> | <span data-ttu-id="1a697-172">application/json</span><span class="sxs-lookup"><span data-stu-id="1a697-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="1a697-173">响应</span><span class="sxs-lookup"><span data-stu-id="1a697-173">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="1a697-174">示例</span><span class="sxs-lookup"><span data-stu-id="1a697-174">Example</span></span>

<span data-ttu-id="1a697-175">在此示例中, 将需要设备的 id 以及已颁发给设备的命令的 id。</span><span class="sxs-lookup"><span data-stu-id="1a697-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="1a697-176">在`/me/devices`发出 GET 呼叫时, 将返回设备 ID, 并在对`/me/devices/{id}/command`进行开机自检呼叫时返回命令 id。</span><span class="sxs-lookup"><span data-stu-id="1a697-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="1a697-177">请求</span><span class="sxs-lookup"><span data-stu-id="1a697-177">Request</span></span>

<span data-ttu-id="1a697-178">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a697-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="1a697-179">响应</span><span class="sxs-lookup"><span data-stu-id="1a697-179">Response</span></span>

<span data-ttu-id="1a697-180">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="1a697-180">The following example shows the response.</span></span>

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
