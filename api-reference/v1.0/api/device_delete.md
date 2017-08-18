# <a name="delete-device"></a><span data-ttu-id="0208d-101">删除设备</span><span class="sxs-lookup"><span data-stu-id="0208d-101">Delete device</span></span>

<span data-ttu-id="0208d-102">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="0208d-102">Delete a registered device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0208d-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="0208d-103">Prerequisites</span></span>
<span data-ttu-id="0208d-104">要执行此 API，需要以下**范围**之一：*Directory.AccessAsUser.All*、*Device.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="0208d-104">One of the following **scopes** is required to execute this API: *Directory.AccessAsUser.All*, *Device.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="0208d-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0208d-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="0208d-106">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="0208d-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0208d-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="0208d-107">Request headers</span></span>
| <span data-ttu-id="0208d-108">名称</span><span class="sxs-lookup"><span data-stu-id="0208d-108">Name</span></span>       | <span data-ttu-id="0208d-109">类型</span><span class="sxs-lookup"><span data-stu-id="0208d-109">Type</span></span> | <span data-ttu-id="0208d-110">说明</span><span class="sxs-lookup"><span data-stu-id="0208d-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0208d-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="0208d-111">Authorization</span></span>  | <span data-ttu-id="0208d-112">string</span><span class="sxs-lookup"><span data-stu-id="0208d-112">string</span></span>  | <span data-ttu-id="0208d-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0208d-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0208d-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="0208d-115">Request body</span></span>
<span data-ttu-id="0208d-116">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0208d-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0208d-117">响应</span><span class="sxs-lookup"><span data-stu-id="0208d-117">Response</span></span>

<span data-ttu-id="0208d-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0208d-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0208d-120">示例</span><span class="sxs-lookup"><span data-stu-id="0208d-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0208d-121">请求</span><span class="sxs-lookup"><span data-stu-id="0208d-121">Request</span></span>
<span data-ttu-id="0208d-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0208d-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="0208d-123">响应</span><span class="sxs-lookup"><span data-stu-id="0208d-123">Response</span></span>
<span data-ttu-id="0208d-124">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0208d-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
