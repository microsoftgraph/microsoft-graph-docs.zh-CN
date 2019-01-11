---
title: 发送设备命令
description: '此 API 支持 Project Rome 功能命令与 Microsoft 帐户关联的设备。 在执行 GET 呼叫后`me/devices`，向您的设备发出命令的设备 ID 中传递。 支持两种类型的命令： LaunchURI 和 AppServices。 如果您正在使用 LaunchURI，指定*类型*和*负载*参数。 对于 AppService 呼叫，指定 '
localization_priority: Normal
ms.openlocfilehash: 54349e2f43a776523614b0cd2abbc209e89305fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891985"
---
# <a name="send-device-command"></a><span data-ttu-id="d093c-107">发送设备命令</span><span class="sxs-lookup"><span data-stu-id="d093c-107">Send device command</span></span>

> <span data-ttu-id="d093c-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d093c-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d093c-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d093c-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d093c-110">此 API 支持 Project Rome 功能命令与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="d093c-110">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="d093c-111">在执行 GET 呼叫后`me/devices`，向您的设备发出命令的设备 ID 中传递。</span><span class="sxs-lookup"><span data-stu-id="d093c-111">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="d093c-112">支持两种类型的命令： LaunchURI 和 AppServices。</span><span class="sxs-lookup"><span data-stu-id="d093c-112">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="d093c-113">如果您正在使用 LaunchURI，指定*类型*和*负载*参数。</span><span class="sxs-lookup"><span data-stu-id="d093c-113">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="d093c-114">AppService 呼叫的指定*类型*、*负载*、 *packageFamilyName*和*appServiceName*参数。</span><span class="sxs-lookup"><span data-stu-id="d093c-114">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="d093c-115">权限</span><span class="sxs-lookup"><span data-stu-id="d093c-115">Permissions</span></span>

<span data-ttu-id="d093c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d093c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d093c-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="d093c-118">Permission type</span></span>      | <span data-ttu-id="d093c-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d093c-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d093c-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d093c-120">Delegated (work or school account)</span></span> | <span data-ttu-id="d093c-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d093c-121">Not supported.</span></span>    |
|<span data-ttu-id="d093c-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d093c-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d093c-123">Device.Command</span><span class="sxs-lookup"><span data-stu-id="d093c-123">Device.Command</span></span>    |
|<span data-ttu-id="d093c-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="d093c-124">Application</span></span> | <span data-ttu-id="d093c-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="d093c-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d093c-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d093c-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="d093c-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="d093c-127">Request headers</span></span>


| <span data-ttu-id="d093c-128">标头</span><span class="sxs-lookup"><span data-stu-id="d093c-128">Header</span></span> |<span data-ttu-id="d093c-129">值</span><span class="sxs-lookup"><span data-stu-id="d093c-129">Value</span></span>
|:----|:------|
|<span data-ttu-id="d093c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d093c-130">Authorization</span></span>| <span data-ttu-id="d093c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d093c-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d093c-133">Accept</span><span class="sxs-lookup"><span data-stu-id="d093c-133">Accept</span></span> | <span data-ttu-id="d093c-134">application/json</span><span class="sxs-lookup"><span data-stu-id="d093c-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d093c-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="d093c-135">Request body</span></span>

<span data-ttu-id="d093c-136">在请求正文中，提供的命令属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d093c-136">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="d093c-137">响应</span><span class="sxs-lookup"><span data-stu-id="d093c-137">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="d093c-138">Command 属性</span><span class="sxs-lookup"><span data-stu-id="d093c-138">Command properties</span></span> 

|<span data-ttu-id="d093c-139">**Name**</span><span class="sxs-lookup"><span data-stu-id="d093c-139">**Name**</span></span>|<span data-ttu-id="d093c-140">**类型**</span><span class="sxs-lookup"><span data-stu-id="d093c-140">**Type**</span></span>|<span data-ttu-id="d093c-141">**说明**</span><span class="sxs-lookup"><span data-stu-id="d093c-141">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="d093c-142">payload</span><span class="sxs-lookup"><span data-stu-id="d093c-142">payload</span></span> | <span data-ttu-id="d093c-143">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="d093c-143">microsoft.graph.json</span></span>| <span data-ttu-id="d093c-144">负载以将发送到应用程序服务或启动在设备上的 URI。</span><span class="sxs-lookup"><span data-stu-id="d093c-144">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="d093c-145">responsePayload</span><span class="sxs-lookup"><span data-stu-id="d093c-145">responsePayload</span></span> | <span data-ttu-id="d093c-146">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="d093c-146">microsoft.graph.json</span></span>| <span data-ttu-id="d093c-147">返回从目标设备的负载。</span><span class="sxs-lookup"><span data-stu-id="d093c-147">Payload returned from target device.</span></span> |
|<span data-ttu-id="d093c-148">postBackURI</span><span class="sxs-lookup"><span data-stu-id="d093c-148">postBackURI</span></span> | <span data-ttu-id="d093c-149">字符串</span><span class="sxs-lookup"><span data-stu-id="d093c-149">String</span></span> | <span data-ttu-id="d093c-150">回发 URI 发送更新的随后进行通知。</span><span class="sxs-lookup"><span data-stu-id="d093c-150">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="d093c-151">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="d093c-151">packageFamilyName</span></span> | <span data-ttu-id="d093c-152">字符串</span><span class="sxs-lookup"><span data-stu-id="d093c-152">String</span></span> | <span data-ttu-id="d093c-153">Windows 应用程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="d093c-153">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="d093c-154">appServiceName</span><span class="sxs-lookup"><span data-stu-id="d093c-154">appServiceName</span></span> | <span data-ttu-id="d093c-155">字符串</span><span class="sxs-lookup"><span data-stu-id="d093c-155">String</span></span> | <span data-ttu-id="d093c-156">由目标应用程序定义的应用程序服务的名称。</span><span class="sxs-lookup"><span data-stu-id="d093c-156">Name of app service defined by the target application.</span></span> <span data-ttu-id="d093c-157">所需如果启动应用程序服务。</span><span class="sxs-lookup"><span data-stu-id="d093c-157">Required if launching an app service.</span></span> |
|<span data-ttu-id="d093c-158">type</span><span class="sxs-lookup"><span data-stu-id="d093c-158">type</span></span>| <span data-ttu-id="d093c-159">字符串</span><span class="sxs-lookup"><span data-stu-id="d093c-159">String</span></span> | <span data-ttu-id="d093c-160">LaunchURI 或 AppService。</span><span class="sxs-lookup"><span data-stu-id="d093c-160">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="d093c-161">id</span><span class="sxs-lookup"><span data-stu-id="d093c-161">id</span></span>| <span data-ttu-id="d093c-162">字符串</span><span class="sxs-lookup"><span data-stu-id="d093c-162">String</span></span> | <span data-ttu-id="d093c-163">已向设备发送命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="d093c-163">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="d093c-164">actionStatus</span><span class="sxs-lookup"><span data-stu-id="d093c-164">actionStatus</span></span> | <span data-ttu-id="d093c-165">字符串</span><span class="sxs-lookup"><span data-stu-id="d093c-165">String</span></span> | <span data-ttu-id="d093c-166">命令的[状态](get-device-command-status.md)。</span><span class="sxs-lookup"><span data-stu-id="d093c-166">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="d093c-167">error</span><span class="sxs-lookup"><span data-stu-id="d093c-167">error</span></span>| <span data-ttu-id="d093c-168">字符串</span><span class="sxs-lookup"><span data-stu-id="d093c-168">String</span></span>| <span data-ttu-id="d093c-169">目标应用程序的请求相关联的任何错误。</span><span class="sxs-lookup"><span data-stu-id="d093c-169">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="d093c-170">启动 URI 示例</span><span class="sxs-lookup"><span data-stu-id="d093c-170">Launch URI example</span></span>

<span data-ttu-id="d093c-171">下面是 LaunchURI 请求; 的一个示例它将启动 URI 或目标设备上的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d093c-171">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="d093c-172">要启动 URI 或应用程序，发出公告使用的设备 ID (从上执行 GET 呼叫获取`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="d093c-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="d093c-173">*类型*参数设置为*LaunchURI*和提供 URI 值，如https://bing.com。</span><span class="sxs-lookup"><span data-stu-id="d093c-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="d093c-174">请求</span><span class="sxs-lookup"><span data-stu-id="d093c-174">Request</span></span>

<span data-ttu-id="d093c-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d093c-175">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d093c-176">响应</span><span class="sxs-lookup"><span data-stu-id="d093c-176">Response</span></span> 

<span data-ttu-id="d093c-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d093c-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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


## <a name="app-service-example"></a><span data-ttu-id="d093c-178">应用程序服务示例</span><span class="sxs-lookup"><span data-stu-id="d093c-178">App service example</span></span>

<span data-ttu-id="d093c-179">下面是查询应用程序服务在设备上的一个示例。</span><span class="sxs-lookup"><span data-stu-id="d093c-179">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="d093c-180">若要使用的应用程序服务必须执行 POST 呼叫使用的设备 id (从上执行 GET 呼叫获取`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="d093c-180">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="d093c-181">若要使用下面的示例，您必须目标设备上安装[Rome 应用程序](https://aka.ms/romanapp)。</span><span class="sxs-lookup"><span data-stu-id="d093c-181">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="d093c-182">必须在调用设置多个其他属性。</span><span class="sxs-lookup"><span data-stu-id="d093c-182">Several additional properties must be set in the call.</span></span> <span data-ttu-id="d093c-183">*类型*必须设置为*AppService* *AppServiceName*必须设置为应用程序服务应用程序中定义的名称、 *PackageFamilyName*必须设置为应用程序清单和*负载*中定义的程序包系列名称包含的键和值您正在呼叫的目标应用程序中的服务。</span><span class="sxs-lookup"><span data-stu-id="d093c-183">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="d093c-184">请求</span><span class="sxs-lookup"><span data-stu-id="d093c-184">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d093c-185">响应</span><span class="sxs-lookup"><span data-stu-id="d093c-185">Response</span></span>

<span data-ttu-id="d093c-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d093c-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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
