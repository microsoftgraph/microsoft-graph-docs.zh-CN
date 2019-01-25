---
title: 发送设备命令
description: '此 API 支持 Project Rome 功能命令与 Microsoft 帐户关联的设备。 在执行 GET 呼叫后`me/devices`，向您的设备发出命令的设备 ID 中传递。 支持两种类型的命令： LaunchURI 和 AppServices。 如果您正在使用 LaunchURI，指定*类型*和*负载*参数。 对于 AppService 呼叫，指定 '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526240"
---
# <a name="send-device-command"></a><span data-ttu-id="d61f0-107">发送设备命令</span><span class="sxs-lookup"><span data-stu-id="d61f0-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61f0-108">此 API 支持 Project Rome 功能命令与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="d61f0-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="d61f0-109">在执行 GET 呼叫后`me/devices`，向您的设备发出命令的设备 ID 中传递。</span><span class="sxs-lookup"><span data-stu-id="d61f0-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="d61f0-110">支持两种类型的命令： LaunchURI 和 AppServices。</span><span class="sxs-lookup"><span data-stu-id="d61f0-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="d61f0-111">如果您正在使用 LaunchURI，指定*类型*和*负载*参数。</span><span class="sxs-lookup"><span data-stu-id="d61f0-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="d61f0-112">AppService 呼叫的指定*类型*、*负载*、 *packageFamilyName*和*appServiceName*参数。</span><span class="sxs-lookup"><span data-stu-id="d61f0-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="d61f0-113">权限</span><span class="sxs-lookup"><span data-stu-id="d61f0-113">Permissions</span></span>

<span data-ttu-id="d61f0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d61f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d61f0-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="d61f0-116">Permission type</span></span>      | <span data-ttu-id="d61f0-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d61f0-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d61f0-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d61f0-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d61f0-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d61f0-119">Not supported.</span></span>    |
|<span data-ttu-id="d61f0-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d61f0-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d61f0-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="d61f0-121">Device.Command</span></span>    |
|<span data-ttu-id="d61f0-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="d61f0-122">Application</span></span> | <span data-ttu-id="d61f0-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="d61f0-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d61f0-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d61f0-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="d61f0-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="d61f0-125">Request headers</span></span>


| <span data-ttu-id="d61f0-126">标头</span><span class="sxs-lookup"><span data-stu-id="d61f0-126">Header</span></span> |<span data-ttu-id="d61f0-127">值</span><span class="sxs-lookup"><span data-stu-id="d61f0-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="d61f0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d61f0-128">Authorization</span></span>| <span data-ttu-id="d61f0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d61f0-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d61f0-131">Accept</span><span class="sxs-lookup"><span data-stu-id="d61f0-131">Accept</span></span> | <span data-ttu-id="d61f0-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d61f0-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d61f0-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d61f0-133">Request body</span></span>

<span data-ttu-id="d61f0-134">在请求正文中，提供的命令属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d61f0-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="d61f0-135">响应</span><span class="sxs-lookup"><span data-stu-id="d61f0-135">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="d61f0-136">Command Properties</span><span class="sxs-lookup"><span data-stu-id="d61f0-136">Command properties</span></span> 

|<span data-ttu-id="d61f0-137">**Name**</span><span class="sxs-lookup"><span data-stu-id="d61f0-137">**Name**</span></span>|<span data-ttu-id="d61f0-138">**类型**</span><span class="sxs-lookup"><span data-stu-id="d61f0-138">**Type**</span></span>|<span data-ttu-id="d61f0-139">**说明**</span><span class="sxs-lookup"><span data-stu-id="d61f0-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="d61f0-140">payload</span><span class="sxs-lookup"><span data-stu-id="d61f0-140">payload</span></span> | <span data-ttu-id="d61f0-141">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="d61f0-141">microsoft.graph.json</span></span>| <span data-ttu-id="d61f0-142">负载以将发送到应用程序服务或启动在设备上的 URI。</span><span class="sxs-lookup"><span data-stu-id="d61f0-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="d61f0-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="d61f0-143">responsePayload</span></span> | <span data-ttu-id="d61f0-144">microsoft.graph.json</span><span class="sxs-lookup"><span data-stu-id="d61f0-144">microsoft.graph.json</span></span>| <span data-ttu-id="d61f0-145">返回从目标设备的负载。</span><span class="sxs-lookup"><span data-stu-id="d61f0-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="d61f0-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="d61f0-146">postBackURI</span></span> | <span data-ttu-id="d61f0-147">String</span><span class="sxs-lookup"><span data-stu-id="d61f0-147">String</span></span> | <span data-ttu-id="d61f0-148">回发 URI 发送更新的随后进行通知。</span><span class="sxs-lookup"><span data-stu-id="d61f0-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="d61f0-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="d61f0-149">packageFamilyName</span></span> | <span data-ttu-id="d61f0-150">String</span><span class="sxs-lookup"><span data-stu-id="d61f0-150">String</span></span> | <span data-ttu-id="d61f0-151">Windows 应用程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="d61f0-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="d61f0-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="d61f0-152">appServiceName</span></span> | <span data-ttu-id="d61f0-153">String</span><span class="sxs-lookup"><span data-stu-id="d61f0-153">String</span></span> | <span data-ttu-id="d61f0-154">由目标应用程序定义的应用程序服务的名称。</span><span class="sxs-lookup"><span data-stu-id="d61f0-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="d61f0-155">所需如果启动应用程序服务。</span><span class="sxs-lookup"><span data-stu-id="d61f0-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="d61f0-156">type</span><span class="sxs-lookup"><span data-stu-id="d61f0-156">type</span></span>| <span data-ttu-id="d61f0-157">String</span><span class="sxs-lookup"><span data-stu-id="d61f0-157">String</span></span> | <span data-ttu-id="d61f0-158">LaunchURI 或 AppService。</span><span class="sxs-lookup"><span data-stu-id="d61f0-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="d61f0-159">id</span><span class="sxs-lookup"><span data-stu-id="d61f0-159">id</span></span>| <span data-ttu-id="d61f0-160">字串符号</span><span class="sxs-lookup"><span data-stu-id="d61f0-160">String</span></span> | <span data-ttu-id="d61f0-161">已向设备发送命令的 ID。</span><span class="sxs-lookup"><span data-stu-id="d61f0-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="d61f0-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="d61f0-162">actionStatus</span></span> | <span data-ttu-id="d61f0-163">String</span><span class="sxs-lookup"><span data-stu-id="d61f0-163">String</span></span> | <span data-ttu-id="d61f0-164">命令的[状态](get-device-command-status.md)。</span><span class="sxs-lookup"><span data-stu-id="d61f0-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="d61f0-165">error</span><span class="sxs-lookup"><span data-stu-id="d61f0-165">error</span></span>| <span data-ttu-id="d61f0-166">String</span><span class="sxs-lookup"><span data-stu-id="d61f0-166">String</span></span>| <span data-ttu-id="d61f0-167">目标应用程序的请求相关联的任何错误。</span><span class="sxs-lookup"><span data-stu-id="d61f0-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="d61f0-168">启动 URI 示例</span><span class="sxs-lookup"><span data-stu-id="d61f0-168">Launch URI example</span></span>

<span data-ttu-id="d61f0-169">下面是 LaunchURI 请求; 的一个示例它将启动 URI 或目标设备上的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d61f0-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="d61f0-170">要启动 URI 或应用程序，发出公告使用的设备 ID (从上执行 GET 呼叫获取`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="d61f0-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="d61f0-171">*类型*参数设置为*LaunchURI*和提供 URI 值，如https://bing.com。</span><span class="sxs-lookup"><span data-stu-id="d61f0-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="d61f0-172">请求</span><span class="sxs-lookup"><span data-stu-id="d61f0-172">Request</span></span>

<span data-ttu-id="d61f0-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d61f0-173">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d61f0-174">响应</span><span class="sxs-lookup"><span data-stu-id="d61f0-174">Response</span></span> 

<span data-ttu-id="d61f0-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d61f0-175">The following is an example of the response.</span></span>

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


## <a name="app-service-example"></a><span data-ttu-id="d61f0-176">应用程序服务示例</span><span class="sxs-lookup"><span data-stu-id="d61f0-176">App service example</span></span>

<span data-ttu-id="d61f0-177">下面是查询应用程序服务在设备上的一个示例。</span><span class="sxs-lookup"><span data-stu-id="d61f0-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="d61f0-178">若要使用的应用程序服务必须执行 POST 呼叫使用的设备 id (从上执行 GET 呼叫获取`me/devices`)。</span><span class="sxs-lookup"><span data-stu-id="d61f0-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="d61f0-179">若要使用下面的示例，您必须目标设备上安装[Rome 应用程序](https://aka.ms/romanapp)。</span><span class="sxs-lookup"><span data-stu-id="d61f0-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="d61f0-180">必须在调用设置多个其他属性。</span><span class="sxs-lookup"><span data-stu-id="d61f0-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="d61f0-181">*类型*必须设置为*AppService* *AppServiceName*必须设置为应用程序服务应用程序中定义的名称、 *PackageFamilyName*必须设置为应用程序清单和*负载*中定义的程序包系列名称包含的键和值您正在呼叫的目标应用程序中的服务。</span><span class="sxs-lookup"><span data-stu-id="d61f0-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="d61f0-182">请求</span><span class="sxs-lookup"><span data-stu-id="d61f0-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d61f0-183">响应</span><span class="sxs-lookup"><span data-stu-id="d61f0-183">Response</span></span>

<span data-ttu-id="d61f0-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d61f0-184">The following is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
