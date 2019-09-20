---
title: 发送设备命令
description: '此 API 使 Project 罗马功能能够命令与 Microsoft 帐户关联的设备。 在`me/devices`执行 GET 呼叫后，传入设备的 ID 以向设备发出命令。 支持两种类型的命令： LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请指定*type*和*载荷*参数。 对于 AppService 调用，请指定 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f112c7d3253a0a0801b7542f492c6f3f1f675c81
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053940"
---
# <a name="send-device-command"></a><span data-ttu-id="1c5f6-107">发送设备命令</span><span class="sxs-lookup"><span data-stu-id="1c5f6-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c5f6-108">此 API 使 Project 罗马功能能够命令与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="1c5f6-109">在`me/devices`执行 GET 呼叫后，传入设备的 ID 以向设备发出命令。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="1c5f6-110">支持两种类型的命令： LaunchURI 和 AppServices。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="1c5f6-111">如果使用的是 LaunchURI，请指定*type*和*载荷*参数。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="1c5f6-112">对于 AppService 调用，指定*type*、*载荷*、 *packageFamilyName*和*appServiceName*参数。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c5f6-113">权限</span><span class="sxs-lookup"><span data-stu-id="1c5f6-113">Permissions</span></span>

<span data-ttu-id="1c5f6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1c5f6-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c5f6-116">Permission type</span></span>      | <span data-ttu-id="1c5f6-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c5f6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c5f6-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c5f6-118">Delegated (work or school account)</span></span> | <span data-ttu-id="1c5f6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-119">Not supported.</span></span>    |
|<span data-ttu-id="1c5f6-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c5f6-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c5f6-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="1c5f6-121">Device.Command</span></span>    |
|<span data-ttu-id="1c5f6-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c5f6-122">Application</span></span> | <span data-ttu-id="1c5f6-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c5f6-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c5f6-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="1c5f6-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c5f6-125">Request headers</span></span>


| <span data-ttu-id="1c5f6-126">标头</span><span class="sxs-lookup"><span data-stu-id="1c5f6-126">Header</span></span> |<span data-ttu-id="1c5f6-127">值</span><span class="sxs-lookup"><span data-stu-id="1c5f6-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="1c5f6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c5f6-128">Authorization</span></span>| <span data-ttu-id="1c5f6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1c5f6-131">接受</span><span class="sxs-lookup"><span data-stu-id="1c5f6-131">Accept</span></span> | <span data-ttu-id="1c5f6-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1c5f6-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c5f6-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c5f6-133">Request body</span></span>

<span data-ttu-id="1c5f6-134">在请求正文中，提供命令属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="1c5f6-135">响应</span><span class="sxs-lookup"><span data-stu-id="1c5f6-135">Response</span></span>

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
### <a name="command-properties"></a><span data-ttu-id="1c5f6-136">命令属性</span><span class="sxs-lookup"><span data-stu-id="1c5f6-136">Command properties</span></span> 

|<span data-ttu-id="1c5f6-137">**名称**</span><span class="sxs-lookup"><span data-stu-id="1c5f6-137">**Name**</span></span>|<span data-ttu-id="1c5f6-138">**Type**</span><span class="sxs-lookup"><span data-stu-id="1c5f6-138">**Type**</span></span>|<span data-ttu-id="1c5f6-139">**说明**</span><span class="sxs-lookup"><span data-stu-id="1c5f6-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="1c5f6-140">payload</span><span class="sxs-lookup"><span data-stu-id="1c5f6-140">payload</span></span> | <span data-ttu-id="1c5f6-141">microsoft. json</span><span class="sxs-lookup"><span data-stu-id="1c5f6-141">microsoft.graph.json</span></span>| <span data-ttu-id="1c5f6-142">要发送到应用程序服务或启动设备上的 URI 的有效负载。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="1c5f6-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="1c5f6-143">responsePayload</span></span> | <span data-ttu-id="1c5f6-144">microsoft. json</span><span class="sxs-lookup"><span data-stu-id="1c5f6-144">microsoft.graph.json</span></span>| <span data-ttu-id="1c5f6-145">从目标设备返回的有效负载。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="1c5f6-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="1c5f6-146">postBackURI</span></span> | <span data-ttu-id="1c5f6-147">String</span><span class="sxs-lookup"><span data-stu-id="1c5f6-147">String</span></span> | <span data-ttu-id="1c5f6-148">回发 URI 以发送后续的更新通知。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="1c5f6-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="1c5f6-149">packageFamilyName</span></span> | <span data-ttu-id="1c5f6-150">String</span><span class="sxs-lookup"><span data-stu-id="1c5f6-150">String</span></span> | <span data-ttu-id="1c5f6-151">Windows 程序包系列应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="1c5f6-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="1c5f6-152">appServiceName</span></span> | <span data-ttu-id="1c5f6-153">String</span><span class="sxs-lookup"><span data-stu-id="1c5f6-153">String</span></span> | <span data-ttu-id="1c5f6-154">由目标应用程序定义的应用服务的名称。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="1c5f6-155">如果启动应用服务，则为必需。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="1c5f6-156">type</span><span class="sxs-lookup"><span data-stu-id="1c5f6-156">type</span></span>| <span data-ttu-id="1c5f6-157">String</span><span class="sxs-lookup"><span data-stu-id="1c5f6-157">String</span></span> | <span data-ttu-id="1c5f6-158">LaunchURI 或 AppService。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="1c5f6-159">id</span><span class="sxs-lookup"><span data-stu-id="1c5f6-159">id</span></span>| <span data-ttu-id="1c5f6-160">String</span><span class="sxs-lookup"><span data-stu-id="1c5f6-160">String</span></span> | <span data-ttu-id="1c5f6-161">已发送到设备的命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="1c5f6-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="1c5f6-162">actionStatus</span></span> | <span data-ttu-id="1c5f6-163">String</span><span class="sxs-lookup"><span data-stu-id="1c5f6-163">String</span></span> | <span data-ttu-id="1c5f6-164">命令的[状态](get-device-command-status.md)。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="1c5f6-165">error</span><span class="sxs-lookup"><span data-stu-id="1c5f6-165">error</span></span>| <span data-ttu-id="1c5f6-166">String</span><span class="sxs-lookup"><span data-stu-id="1c5f6-166">String</span></span>| <span data-ttu-id="1c5f6-167">与目标应用程序中的请求关联的任何错误。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-167">Any errors associated with the request from the target application.</span></span> |

## <a name="examples"></a><span data-ttu-id="1c5f6-168">示例</span><span class="sxs-lookup"><span data-stu-id="1c5f6-168">Examples</span></span>

### <a name="example-1-launch-uri"></a><span data-ttu-id="1c5f6-169">示例1：启动 URI</span><span class="sxs-lookup"><span data-stu-id="1c5f6-169">Example 1: Launch URI</span></span> 

<span data-ttu-id="1c5f6-170">以下是 LaunchURI 请求的示例;它会启动一个 URI 或目标设备上的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-170">The following is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="1c5f6-171">若要启动 URI 或应用，请使用设备 ID 发出 POST （通过执行 GET 呼叫获取`me/devices`）。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-171">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="1c5f6-172">将*类型*参数设置为*LaunchURI* ，并提供 URI 值（如https://bing.com）。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-172">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="1c5f6-173">请求</span><span class="sxs-lookup"><span data-stu-id="1c5f6-173">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="1c5f6-174">响应</span><span class="sxs-lookup"><span data-stu-id="1c5f6-174">Response</span></span> 

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


### <a name="example-2-app-service"></a><span data-ttu-id="1c5f6-175">示例2： App service</span><span class="sxs-lookup"><span data-stu-id="1c5f6-175">Example 2: App service</span></span>

<span data-ttu-id="1c5f6-176">下面的示例演示如何在设备上查询应用服务。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-176">The following example shows how to query an app service on a device.</span></span> <span data-ttu-id="1c5f6-177">若要使用应用服务，必须使用设备 ID （通过执行 GET 呼叫获取`me/devices`）执行 POST 调用。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-177">To use an app service, you must do a POST call using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="1c5f6-178">若要使用以下示例，必须在目标设备上安装[罗马应用程序](https://aka.ms/romanapp)。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-178">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="1c5f6-179">必须在调用中设置多个附加属性。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-179">Several additional properties must be set in the call.</span></span> <span data-ttu-id="1c5f6-180">*Type*必须设置为*AppService*， *AppServiceName*必须设置为应用程序中定义的应用服务的名称， *PackageFamilyName*必须设置为应用程序清单中定义的程序包系列名称和*有效负载*保留您在目标应用程序中调用的服务的键和值。</span><span class="sxs-lookup"><span data-stu-id="1c5f6-180">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="1c5f6-181">请求</span><span class="sxs-lookup"><span data-stu-id="1c5f6-181">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="1c5f6-182">响应</span><span class="sxs-lookup"><span data-stu-id="1c5f6-182">Response</span></span>

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
