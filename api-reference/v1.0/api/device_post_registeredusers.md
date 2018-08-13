# <a name="create-registereduser"></a><span data-ttu-id="66996-101">创建 registeredUser</span><span class="sxs-lookup"><span data-stu-id="66996-101">Create registeredUser</span></span>

<span data-ttu-id="66996-102">添加设备的已注册用户。</span><span class="sxs-lookup"><span data-stu-id="66996-102">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="66996-103">权限</span><span class="sxs-lookup"><span data-stu-id="66996-103">Permissions</span></span>
<span data-ttu-id="66996-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="66996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="66996-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="66996-106">Permission type</span></span>      | <span data-ttu-id="66996-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66996-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66996-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66996-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66996-109">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66996-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66996-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66996-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66996-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="66996-111">Not supported.</span></span>    |
|<span data-ttu-id="66996-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="66996-112">Application</span></span> | <span data-ttu-id="66996-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66996-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66996-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66996-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="66996-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="66996-115">Request headers</span></span>
| <span data-ttu-id="66996-116">名称</span><span class="sxs-lookup"><span data-stu-id="66996-116">Name</span></span>       | <span data-ttu-id="66996-117">类型</span><span class="sxs-lookup"><span data-stu-id="66996-117">Type</span></span> | <span data-ttu-id="66996-118">说明</span><span class="sxs-lookup"><span data-stu-id="66996-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66996-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="66996-119">Authorization</span></span>  | <span data-ttu-id="66996-120">string</span><span class="sxs-lookup"><span data-stu-id="66996-120">string</span></span>  | <span data-ttu-id="66996-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66996-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66996-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="66996-123">Request body</span></span>
<span data-ttu-id="66996-124">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66996-124">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66996-125">响应</span><span class="sxs-lookup"><span data-stu-id="66996-125">Response</span></span>

<span data-ttu-id="66996-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66996-126">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66996-127">示例</span><span class="sxs-lookup"><span data-stu-id="66996-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66996-128">请求</span><span class="sxs-lookup"><span data-stu-id="66996-128">Request</span></span>
<span data-ttu-id="66996-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66996-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="66996-130">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66996-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="66996-131">响应</span><span class="sxs-lookup"><span data-stu-id="66996-131">Response</span></span>
<span data-ttu-id="66996-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66996-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->