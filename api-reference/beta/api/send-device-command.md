---
title: 发送设备命令
description: '此 API 使 Project 罗马功能能够命令与 Microsoft 帐户关联的设备。 在执行 GET 呼叫后 `me/devices` ，传入设备的 ID 以向设备发出命令。 支持两种类型的命令： LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请指定 *type* 和 *载荷* 参数。 对于 AppService 调用，请指定 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: 73f725dde241e5fc37ace2bc6b5ac92e5401a9fc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812560"
---
# <a name="send-device-command"></a><span data-ttu-id="48a8c-107">发送设备命令</span><span class="sxs-lookup"><span data-stu-id="48a8c-107">Send device command</span></span>

<span data-ttu-id="48a8c-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48a8c-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a8c-109">此 API 使 Project 罗马功能能够命令与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="48a8c-109">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="48a8c-110">在执行 GET 呼叫后 `me/devices` ，传入设备的 ID 以向设备发出命令。</span><span class="sxs-lookup"><span data-stu-id="48a8c-110">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="48a8c-111">支持两种类型的命令： LaunchURI 和 AppServices。</span><span class="sxs-lookup"><span data-stu-id="48a8c-111">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="48a8c-112">如果使用的是 LaunchURI，请指定 *type* 和 *载荷* 参数。</span><span class="sxs-lookup"><span data-stu-id="48a8c-112">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="48a8c-113">对于 AppService 调用，指定 *type*、 *载荷*、 *packageFamilyName*和 *appServiceName* 参数。</span><span class="sxs-lookup"><span data-stu-id="48a8c-113">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="48a8c-114">权限</span><span class="sxs-lookup"><span data-stu-id="48a8c-114">Permissions</span></span>

<span data-ttu-id="48a8c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48a8c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48a8c-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="48a8c-117">Permission type</span></span>      | <span data-ttu-id="48a8c-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48a8c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48a8c-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48a8c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="48a8c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="48a8c-120">Not supported.</span></span>    |
|<span data-ttu-id="48a8c-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48a8c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48a8c-122">Device.Command</span><span class="sxs-lookup"><span data-stu-id="48a8c-122">Device.Command</span></span>    |
|<span data-ttu-id="48a8c-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="48a8c-123">Application</span></span> | <span data-ttu-id="48a8c-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="48a8c-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48a8c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48a8c-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="48a8c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="48a8c-126">Request headers</span></span>


| <span data-ttu-id="48a8c-127">标头</span><span class="sxs-lookup"><span data-stu-id="48a8c-127">Header</span></span> |<span data-ttu-id="48a8c-128">值</span><span class="sxs-lookup"><span data-stu-id="48a8c-128">Value</span></span>
|:----|:------|
|<span data-ttu-id="48a8c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="48a8c-129">Authorization</span></span>| <span data-ttu-id="48a8c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48a8c-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="48a8c-132">接受</span><span class="sxs-lookup"><span data-stu-id="48a8c-132">Accept</span></span> | <span data-ttu-id="48a8c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="48a8c-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="48a8c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="48a8c-134">Request body</span></span>

<span data-ttu-id="48a8c-135">在请求正文中，提供命令属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48a8c-135">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="48a8c-136">响应</span><span class="sxs-lookup"><span data-stu-id="48a8c-136">Response</span></span>

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
### <a name="command-properties"></a><span data-ttu-id="48a8c-137">命令属性</span><span class="sxs-lookup"><span data-stu-id="48a8c-137">Command properties</span></span>

|<span data-ttu-id="48a8c-138">**名称**</span><span class="sxs-lookup"><span data-stu-id="48a8c-138">**Name**</span></span>|<span data-ttu-id="48a8c-139">**类型**</span><span class="sxs-lookup"><span data-stu-id="48a8c-139">**Type**</span></span>|<span data-ttu-id="48a8c-140">**说明**</span><span class="sxs-lookup"><span data-stu-id="48a8c-140">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="48a8c-141">payload</span><span class="sxs-lookup"><span data-stu-id="48a8c-141">payload</span></span> | <span data-ttu-id="48a8c-142">microsoft.graph.js</span><span class="sxs-lookup"><span data-stu-id="48a8c-142">microsoft.graph.json</span></span>| <span data-ttu-id="48a8c-143">要发送到应用程序服务或启动设备上的 URI 的有效负载。</span><span class="sxs-lookup"><span data-stu-id="48a8c-143">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="48a8c-144">responsePayload</span><span class="sxs-lookup"><span data-stu-id="48a8c-144">responsePayload</span></span> | <span data-ttu-id="48a8c-145">microsoft.graph.js</span><span class="sxs-lookup"><span data-stu-id="48a8c-145">microsoft.graph.json</span></span>| <span data-ttu-id="48a8c-146">从目标设备返回的有效负载。</span><span class="sxs-lookup"><span data-stu-id="48a8c-146">Payload returned from target device.</span></span> |
|<span data-ttu-id="48a8c-147">postBackURI</span><span class="sxs-lookup"><span data-stu-id="48a8c-147">postBackURI</span></span> | <span data-ttu-id="48a8c-148">String</span><span class="sxs-lookup"><span data-stu-id="48a8c-148">String</span></span> | <span data-ttu-id="48a8c-149">回发 URI 以发送后续的更新通知。</span><span class="sxs-lookup"><span data-stu-id="48a8c-149">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="48a8c-150">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="48a8c-150">packageFamilyName</span></span> | <span data-ttu-id="48a8c-151">String</span><span class="sxs-lookup"><span data-stu-id="48a8c-151">String</span></span> | <span data-ttu-id="48a8c-152">Windows 程序包系列应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="48a8c-152">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="48a8c-153">appServiceName</span><span class="sxs-lookup"><span data-stu-id="48a8c-153">appServiceName</span></span> | <span data-ttu-id="48a8c-154">String</span><span class="sxs-lookup"><span data-stu-id="48a8c-154">String</span></span> | <span data-ttu-id="48a8c-155">由目标应用程序定义的应用服务的名称。</span><span class="sxs-lookup"><span data-stu-id="48a8c-155">Name of app service defined by the target application.</span></span> <span data-ttu-id="48a8c-156">如果启动应用服务，则为必需。</span><span class="sxs-lookup"><span data-stu-id="48a8c-156">Required if launching an app service.</span></span> |
|<span data-ttu-id="48a8c-157">type</span><span class="sxs-lookup"><span data-stu-id="48a8c-157">type</span></span>| <span data-ttu-id="48a8c-158">String</span><span class="sxs-lookup"><span data-stu-id="48a8c-158">String</span></span> | <span data-ttu-id="48a8c-159">LaunchURI 或 AppService。</span><span class="sxs-lookup"><span data-stu-id="48a8c-159">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="48a8c-160">id</span><span class="sxs-lookup"><span data-stu-id="48a8c-160">id</span></span>| <span data-ttu-id="48a8c-161">String</span><span class="sxs-lookup"><span data-stu-id="48a8c-161">String</span></span> | <span data-ttu-id="48a8c-162">已发送到设备的命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="48a8c-162">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="48a8c-163">actionStatus</span><span class="sxs-lookup"><span data-stu-id="48a8c-163">actionStatus</span></span> | <span data-ttu-id="48a8c-164">String</span><span class="sxs-lookup"><span data-stu-id="48a8c-164">String</span></span> | <span data-ttu-id="48a8c-165">命令的 [状态](get-device-command-status.md) 。</span><span class="sxs-lookup"><span data-stu-id="48a8c-165">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="48a8c-166">error</span><span class="sxs-lookup"><span data-stu-id="48a8c-166">error</span></span>| <span data-ttu-id="48a8c-167">String</span><span class="sxs-lookup"><span data-stu-id="48a8c-167">String</span></span>| <span data-ttu-id="48a8c-168">与目标应用程序中的请求关联的任何错误。</span><span class="sxs-lookup"><span data-stu-id="48a8c-168">Any errors associated with the request from the target application.</span></span> |

## <a name="examples"></a><span data-ttu-id="48a8c-169">示例</span><span class="sxs-lookup"><span data-stu-id="48a8c-169">Examples</span></span>

### <a name="example-1-launch-uri"></a><span data-ttu-id="48a8c-170">示例1：启动 URI</span><span class="sxs-lookup"><span data-stu-id="48a8c-170">Example 1: Launch URI</span></span>

<span data-ttu-id="48a8c-171">以下是 LaunchURI 请求的示例;它会启动一个 URI 或目标设备上的应用程序。</span><span class="sxs-lookup"><span data-stu-id="48a8c-171">The following is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="48a8c-172">若要启动 URI 或应用，请使用从) 上的 GET 调用获取的设备的 ID 发出 POST (`me/devices` 。</span><span class="sxs-lookup"><span data-stu-id="48a8c-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="48a8c-173">将 *类型* 参数设置为 *LaunchURI* ，并提供 URI 值（如） https://bing.com 。</span><span class="sxs-lookup"><span data-stu-id="48a8c-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="48a8c-174">请求</span><span class="sxs-lookup"><span data-stu-id="48a8c-174">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```
#### <a name="response"></a><span data-ttu-id="48a8c-175">响应</span><span class="sxs-lookup"><span data-stu-id="48a8c-175">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


### <a name="example-2-app-service"></a><span data-ttu-id="48a8c-176">示例2： App service</span><span class="sxs-lookup"><span data-stu-id="48a8c-176">Example 2: App service</span></span>

<span data-ttu-id="48a8c-177">下面的示例演示如何在设备上查询应用服务。</span><span class="sxs-lookup"><span data-stu-id="48a8c-177">The following example shows how to query an app service on a device.</span></span> <span data-ttu-id="48a8c-178">若要使用应用服务，您必须使用从) 上的 GET 呼叫获取的设备的 ID 执行 POST 调用 (`me/devices` 。</span><span class="sxs-lookup"><span data-stu-id="48a8c-178">To use an app service, you must do a POST call using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="48a8c-179">若要使用以下示例，必须在目标设备上安装 [罗马应用程序](https://aka.ms/romanapp) 。</span><span class="sxs-lookup"><span data-stu-id="48a8c-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="48a8c-180">必须在调用中设置多个附加属性。</span><span class="sxs-lookup"><span data-stu-id="48a8c-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="48a8c-181">*Type* 必须设置为 *AppService*， *AppServiceName* 必须设置为应用程序中定义的应用服务的名称， *PackageFamilyName* 必须设置为应用程序清单中定义的程序包系列名称， *有效负载* 将保留您在目标应用程序中调用的服务的键和值。</span><span class="sxs-lookup"><span data-stu-id="48a8c-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="48a8c-182">请求</span><span class="sxs-lookup"><span data-stu-id="48a8c-182">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a><span data-ttu-id="48a8c-183">响应</span><span class="sxs-lookup"><span data-stu-id="48a8c-183">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
