# <a name="delete-device"></a><span data-ttu-id="3e092-101">删除设备</span><span class="sxs-lookup"><span data-stu-id="3e092-101">Delete device</span></span>

<span data-ttu-id="3e092-102">删除已注册的设备。</span><span class="sxs-lookup"><span data-stu-id="3e092-102">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e092-103">权限</span><span class="sxs-lookup"><span data-stu-id="3e092-103">Permissions</span></span>
<span data-ttu-id="3e092-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3e092-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="3e092-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e092-106">Permission type</span></span>      | <span data-ttu-id="3e092-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e092-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e092-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e092-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3e092-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e092-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e092-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e092-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e092-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e092-111">Not supported.</span></span>    |
|<span data-ttu-id="3e092-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e092-112">Application</span></span> | <span data-ttu-id="3e092-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e092-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e092-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e092-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="3e092-115">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="3e092-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e092-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e092-116">Request headers</span></span>
| <span data-ttu-id="3e092-117">名称</span><span class="sxs-lookup"><span data-stu-id="3e092-117">Name</span></span>       | <span data-ttu-id="3e092-118">类型</span><span class="sxs-lookup"><span data-stu-id="3e092-118">Type</span></span> | <span data-ttu-id="3e092-119">说明</span><span class="sxs-lookup"><span data-stu-id="3e092-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e092-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e092-120">Authorization</span></span>  | <span data-ttu-id="3e092-121">string</span><span class="sxs-lookup"><span data-stu-id="3e092-121">string</span></span>  | <span data-ttu-id="3e092-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e092-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e092-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e092-124">Request body</span></span>
<span data-ttu-id="3e092-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e092-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e092-126">响应</span><span class="sxs-lookup"><span data-stu-id="3e092-126">Response</span></span>

<span data-ttu-id="3e092-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3e092-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e092-129">示例</span><span class="sxs-lookup"><span data-stu-id="3e092-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e092-130">请求</span><span class="sxs-lookup"><span data-stu-id="3e092-130">Request</span></span>
<span data-ttu-id="3e092-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e092-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="3e092-132">响应</span><span class="sxs-lookup"><span data-stu-id="3e092-132">Response</span></span>
<span data-ttu-id="3e092-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3e092-133">Here is an example of the response.</span></span>
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
