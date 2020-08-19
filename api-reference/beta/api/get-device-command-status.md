---
title: 获取设备命令状态
description: 获取设备上命令的状态。 有关状态代码的完整列表，请参阅 actionStatus 的列表。
localization_priority: Normal
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: 33470cb5aceb402d6a37749fa8c2ebcfcd0bce75
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807330"
---
# <a name="get-device-command-status"></a><span data-ttu-id="8a965-104">获取设备命令状态</span><span class="sxs-lookup"><span data-stu-id="8a965-104">Get device command status</span></span>

<span data-ttu-id="8a965-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a965-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a965-106">获取设备上命令的状态。</span><span class="sxs-lookup"><span data-stu-id="8a965-106">Get the status of a command on a device.</span></span> <span data-ttu-id="8a965-107">有关状态代码的完整列表，请参阅 [actionStatus 的列表](#list-of-actionstatus)。</span><span class="sxs-lookup"><span data-stu-id="8a965-107">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a965-108">权限</span><span class="sxs-lookup"><span data-stu-id="8a965-108">Permissions</span></span>

<span data-ttu-id="8a965-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a965-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a965-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a965-111">Permission type</span></span>      | <span data-ttu-id="8a965-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a965-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a965-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a965-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8a965-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a965-114">Not supported.</span></span>    |
|<span data-ttu-id="8a965-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a965-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a965-116">Device.Command</span><span class="sxs-lookup"><span data-stu-id="8a965-116">Device.Command</span></span>    |
|<span data-ttu-id="8a965-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a965-117">Application</span></span> | <span data-ttu-id="8a965-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a965-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a965-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a965-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a965-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a965-120">Request headers</span></span>

| <span data-ttu-id="8a965-121">标头</span><span class="sxs-lookup"><span data-stu-id="8a965-121">Header</span></span> |<span data-ttu-id="8a965-122">值</span><span class="sxs-lookup"><span data-stu-id="8a965-122">Value</span></span>
|:----|:------|
|<span data-ttu-id="8a965-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a965-123">Authorization</span></span>| <span data-ttu-id="8a965-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a965-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8a965-126">接受</span><span class="sxs-lookup"><span data-stu-id="8a965-126">Accept</span></span> | <span data-ttu-id="8a965-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8a965-127">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="8a965-128">响应</span><span class="sxs-lookup"><span data-stu-id="8a965-128">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="8a965-129">ActionStatus 列表</span><span class="sxs-lookup"><span data-stu-id="8a965-129">List of actionStatus</span></span>

- <span data-ttu-id="8a965-130">请求、//命令已创建，正在等待处理</span><span class="sxs-lookup"><span data-stu-id="8a965-130">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="8a965-131">已将 sentToTarget、//命令发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="8a965-131">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="8a965-132">正在执行、//目标设备确认了命令的接收并正在执行该命令</span><span class="sxs-lookup"><span data-stu-id="8a965-132">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="8a965-133">已完成，//命令执行已完成</span><span class="sxs-lookup"><span data-stu-id="8a965-133">completed, // Command execution completed</span></span>
- <span data-ttu-id="8a965-134">failedToSend，//服务无法将命令发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="8a965-134">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="8a965-135">executionFailed，//命令执行失败</span><span class="sxs-lookup"><span data-stu-id="8a965-135">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="8a965-136">commandDropped、//设备处于 ConnectedStandby 状态时由客户端丢弃的命令</span><span class="sxs-lookup"><span data-stu-id="8a965-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="8a965-137">取消、//取消命令</span><span class="sxs-lookup"><span data-stu-id="8a965-137">cancel, // Cancel the command</span></span>
- <span data-ttu-id="8a965-138">取消、//取消命令</span><span class="sxs-lookup"><span data-stu-id="8a965-138">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="8a965-139">已取消，//命令已取消</span><span class="sxs-lookup"><span data-stu-id="8a965-139">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="8a965-140">重试，//服务正在重试将命令发送到目标</span><span class="sxs-lookup"><span data-stu-id="8a965-140">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="8a965-141">已过期，//命令处理超过了过期时间</span><span class="sxs-lookup"><span data-stu-id="8a965-141">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="8a965-142">处理命令时出现错误，//内部错误</span><span class="sxs-lookup"><span data-stu-id="8a965-142">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="8a965-143">自定义//自定义状态</span><span class="sxs-lookup"><span data-stu-id="8a965-143">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="8a965-144">示例</span><span class="sxs-lookup"><span data-stu-id="8a965-144">Example</span></span>

<span data-ttu-id="8a965-145">在此示例中，将需要设备的 ID 以及已颁发给设备的命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="8a965-145">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="8a965-146">在发出对的 GET 呼叫时，将返回设备 ID `/me/devices` ，并且在对进行开机自检呼叫时返回命令 id `/me/devices/{id}/command` 。</span><span class="sxs-lookup"><span data-stu-id="8a965-146">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="8a965-147">请求</span><span class="sxs-lookup"><span data-stu-id="8a965-147">Request</span></span>

<span data-ttu-id="8a965-148">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a965-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="8a965-149">响应</span><span class="sxs-lookup"><span data-stu-id="8a965-149">Response</span></span>

<span data-ttu-id="8a965-150">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="8a965-150">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="8a965-151">获取命令有效负载</span><span class="sxs-lookup"><span data-stu-id="8a965-151">Get command payload</span></span>

<span data-ttu-id="8a965-152">获取设备上特定操作的响应负载。</span><span class="sxs-lookup"><span data-stu-id="8a965-152">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="8a965-153">在查询应用程序服务以传送数据时，将使用响应负载。</span><span class="sxs-lookup"><span data-stu-id="8a965-153">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="8a965-154">权限</span><span class="sxs-lookup"><span data-stu-id="8a965-154">Permissions</span></span>

<span data-ttu-id="8a965-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a965-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a965-157">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a965-157">Permission type</span></span>      | <span data-ttu-id="8a965-158">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a965-158">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a965-159">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a965-159">Delegated (work or school account)</span></span> | <span data-ttu-id="8a965-160">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a965-160">Not supported.</span></span>    |
|<span data-ttu-id="8a965-161">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a965-161">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a965-162">Device.Command</span><span class="sxs-lookup"><span data-stu-id="8a965-162">Device.Command</span></span>    |
|<span data-ttu-id="8a965-163">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a965-163">Application</span></span> | <span data-ttu-id="8a965-164">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a965-164">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="8a965-165">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a965-165">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="8a965-166">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a965-166">Request headers</span></span>

| <span data-ttu-id="8a965-167">标头</span><span class="sxs-lookup"><span data-stu-id="8a965-167">Header</span></span> |<span data-ttu-id="8a965-168">值</span><span class="sxs-lookup"><span data-stu-id="8a965-168">Value</span></span>
|:----|:------|
|<span data-ttu-id="8a965-169">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a965-169">Authorization</span></span>| <span data-ttu-id="8a965-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a965-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8a965-172">接受</span><span class="sxs-lookup"><span data-stu-id="8a965-172">Accept</span></span> | <span data-ttu-id="8a965-173">application/json</span><span class="sxs-lookup"><span data-stu-id="8a965-173">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="8a965-174">响应</span><span class="sxs-lookup"><span data-stu-id="8a965-174">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="8a965-175">示例</span><span class="sxs-lookup"><span data-stu-id="8a965-175">Example</span></span>

<span data-ttu-id="8a965-176">在此示例中，将需要设备的 ID 以及已颁发给设备的命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="8a965-176">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="8a965-177">在发出 GET 呼叫时，将返回设备 ID `/me/devices` ，并在对进行开机自检呼叫时返回命令 id `/me/devices/{id}/command` 。</span><span class="sxs-lookup"><span data-stu-id="8a965-177">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="8a965-178">请求</span><span class="sxs-lookup"><span data-stu-id="8a965-178">Request</span></span>

<span data-ttu-id="8a965-179">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a965-179">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="8a965-180">响应</span><span class="sxs-lookup"><span data-stu-id="8a965-180">Response</span></span>

<span data-ttu-id="8a965-181">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="8a965-181">The following example shows the response.</span></span>

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
