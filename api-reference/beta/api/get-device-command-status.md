---
title: 获取设备命令状态
description: 获取设备上命令的状态。 有关状态代码的完整列表, 请参阅 actionStatus 的列表。
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457149"
---
# <a name="get-device-command-status"></a><span data-ttu-id="91133-104">获取设备命令状态</span><span class="sxs-lookup"><span data-stu-id="91133-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91133-105">获取设备上命令的状态。</span><span class="sxs-lookup"><span data-stu-id="91133-105">Get the status of a command on a device.</span></span> <span data-ttu-id="91133-106">有关状态代码的完整列表, 请参阅[actionStatus 的列表](#list-of-actionstatus)。</span><span class="sxs-lookup"><span data-stu-id="91133-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="91133-107">权限</span><span class="sxs-lookup"><span data-stu-id="91133-107">Permissions</span></span>

<span data-ttu-id="91133-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91133-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91133-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="91133-110">Permission type</span></span>      | <span data-ttu-id="91133-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91133-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91133-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91133-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91133-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="91133-113">Not supported.</span></span>    |
|<span data-ttu-id="91133-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91133-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91133-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="91133-115">Device.Command</span></span>    |
|<span data-ttu-id="91133-116">Application</span><span class="sxs-lookup"><span data-stu-id="91133-116">Application</span></span> | <span data-ttu-id="91133-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="91133-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91133-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91133-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91133-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="91133-119">Request headers</span></span>

| <span data-ttu-id="91133-120">标头</span><span class="sxs-lookup"><span data-stu-id="91133-120">Header</span></span> |<span data-ttu-id="91133-121">值</span><span class="sxs-lookup"><span data-stu-id="91133-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="91133-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91133-122">Authorization</span></span>| <span data-ttu-id="91133-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91133-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="91133-125">接受</span><span class="sxs-lookup"><span data-stu-id="91133-125">Accept</span></span> | <span data-ttu-id="91133-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91133-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="91133-127">响应</span><span class="sxs-lookup"><span data-stu-id="91133-127">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="91133-128">actionStatus 列表</span><span class="sxs-lookup"><span data-stu-id="91133-128">List of actionStatus</span></span>

- <span data-ttu-id="91133-129">请求、//命令已创建, 正在等待处理</span><span class="sxs-lookup"><span data-stu-id="91133-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="91133-130">已将 sentToTarget、//命令发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="91133-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="91133-131">正在执行、//目标设备确认了命令的接收并正在执行该命令</span><span class="sxs-lookup"><span data-stu-id="91133-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="91133-132">已完成,//命令执行已完成</span><span class="sxs-lookup"><span data-stu-id="91133-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="91133-133">failedToSend,//服务无法将命令发送到目标设备</span><span class="sxs-lookup"><span data-stu-id="91133-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="91133-134">executionFailed,//命令执行失败</span><span class="sxs-lookup"><span data-stu-id="91133-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="91133-135">commandDropped、//设备处于 ConnectedStandby 状态时由客户端丢弃的命令</span><span class="sxs-lookup"><span data-stu-id="91133-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="91133-136">取消、//取消命令</span><span class="sxs-lookup"><span data-stu-id="91133-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="91133-137">取消、//取消命令</span><span class="sxs-lookup"><span data-stu-id="91133-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="91133-138">已取消,//命令已取消</span><span class="sxs-lookup"><span data-stu-id="91133-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="91133-139">重试,//服务正在重试将命令发送到目标</span><span class="sxs-lookup"><span data-stu-id="91133-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="91133-140">已过期,//命令处理超过了过期时间</span><span class="sxs-lookup"><span data-stu-id="91133-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="91133-141">处理命令时出现错误,//内部错误</span><span class="sxs-lookup"><span data-stu-id="91133-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="91133-142">自定义//自定义状态</span><span class="sxs-lookup"><span data-stu-id="91133-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="91133-143">示例</span><span class="sxs-lookup"><span data-stu-id="91133-143">Example</span></span>

<span data-ttu-id="91133-144">在此示例中, 将需要设备的 id 以及已颁发给设备的命令的 id。</span><span class="sxs-lookup"><span data-stu-id="91133-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="91133-145">在发出对`/me/devices`的 GET 呼叫时, 将返回设备 ID, 并且在对`/me/devices/{id}/command`进行开机自检呼叫时返回命令 id。</span><span class="sxs-lookup"><span data-stu-id="91133-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="91133-146">请求</span><span class="sxs-lookup"><span data-stu-id="91133-146">Request</span></span>

<span data-ttu-id="91133-147">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="91133-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="91133-148">响应</span><span class="sxs-lookup"><span data-stu-id="91133-148">Response</span></span>

<span data-ttu-id="91133-149">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="91133-149">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="91133-150">获取命令有效负载</span><span class="sxs-lookup"><span data-stu-id="91133-150">Get command payload</span></span>

<span data-ttu-id="91133-151">获取设备上特定操作的响应负载。</span><span class="sxs-lookup"><span data-stu-id="91133-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="91133-152">在查询应用程序服务以传送数据时, 将使用响应负载。</span><span class="sxs-lookup"><span data-stu-id="91133-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="91133-153">权限</span><span class="sxs-lookup"><span data-stu-id="91133-153">Permissions</span></span>

<span data-ttu-id="91133-p107">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91133-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91133-156">权限类型</span><span class="sxs-lookup"><span data-stu-id="91133-156">Permission type</span></span>      | <span data-ttu-id="91133-157">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91133-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91133-158">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91133-158">Delegated (work or school account)</span></span> | <span data-ttu-id="91133-159">不支持。</span><span class="sxs-lookup"><span data-stu-id="91133-159">Not supported.</span></span>    |
|<span data-ttu-id="91133-160">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91133-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91133-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="91133-161">Device.Command</span></span>    |
|<span data-ttu-id="91133-162">Application</span><span class="sxs-lookup"><span data-stu-id="91133-162">Application</span></span> | <span data-ttu-id="91133-163">不支持。</span><span class="sxs-lookup"><span data-stu-id="91133-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="91133-164">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91133-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="91133-165">请求标头</span><span class="sxs-lookup"><span data-stu-id="91133-165">Request headers</span></span>

| <span data-ttu-id="91133-166">标头</span><span class="sxs-lookup"><span data-stu-id="91133-166">Header</span></span> |<span data-ttu-id="91133-167">值</span><span class="sxs-lookup"><span data-stu-id="91133-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="91133-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="91133-168">Authorization</span></span>| <span data-ttu-id="91133-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91133-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="91133-171">接受</span><span class="sxs-lookup"><span data-stu-id="91133-171">Accept</span></span> | <span data-ttu-id="91133-172">application/json</span><span class="sxs-lookup"><span data-stu-id="91133-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="91133-173">响应</span><span class="sxs-lookup"><span data-stu-id="91133-173">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="91133-174">示例</span><span class="sxs-lookup"><span data-stu-id="91133-174">Example</span></span>

<span data-ttu-id="91133-175">在此示例中, 将需要设备的 id 以及已颁发给设备的命令的 id。</span><span class="sxs-lookup"><span data-stu-id="91133-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="91133-176">在`/me/devices`发出 GET 呼叫时, 将返回设备 ID, 并在对`/me/devices/{id}/command`进行开机自检呼叫时返回命令 id。</span><span class="sxs-lookup"><span data-stu-id="91133-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="91133-177">请求</span><span class="sxs-lookup"><span data-stu-id="91133-177">Request</span></span>

<span data-ttu-id="91133-178">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="91133-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="91133-179">响应</span><span class="sxs-lookup"><span data-stu-id="91133-179">Response</span></span>

<span data-ttu-id="91133-180">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="91133-180">The following example shows the response.</span></span>

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
