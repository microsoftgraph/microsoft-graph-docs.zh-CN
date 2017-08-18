# <a name="add-member"></a><span data-ttu-id="8ca11-101">添加成员</span><span class="sxs-lookup"><span data-stu-id="8ca11-101">Add member</span></span>

<span data-ttu-id="8ca11-p101">通过 **members** 导航属性，使用此 API 将成员添加到 Office 365 组、安全组或已启用邮件的安全组中。你可以添加用户或其他组。重要说明：仅能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="8ca11-p101">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ca11-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ca11-105">Prerequisites</span></span>
<span data-ttu-id="8ca11-106">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All* 或 *Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="8ca11-106">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="8ca11-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ca11-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8ca11-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ca11-108">Request headers</span></span>
| <span data-ttu-id="8ca11-109">名称</span><span class="sxs-lookup"><span data-stu-id="8ca11-109">Name</span></span>       | <span data-ttu-id="8ca11-110">类型</span><span class="sxs-lookup"><span data-stu-id="8ca11-110">Type</span></span> | <span data-ttu-id="8ca11-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ca11-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ca11-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ca11-112">Authorization</span></span>  | <span data-ttu-id="8ca11-113">string</span><span class="sxs-lookup"><span data-stu-id="8ca11-113">string</span></span>  | <span data-ttu-id="8ca11-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ca11-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ca11-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ca11-116">Request body</span></span>
<span data-ttu-id="8ca11-117">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ca11-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8ca11-118">响应</span><span class="sxs-lookup"><span data-stu-id="8ca11-118">Response</span></span>

<span data-ttu-id="8ca11-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8ca11-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ca11-121">示例</span><span class="sxs-lookup"><span data-stu-id="8ca11-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ca11-122">请求</span><span class="sxs-lookup"><span data-stu-id="8ca11-122">Request</span></span>
<span data-ttu-id="8ca11-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ca11-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="8ca11-124">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 `id` 的JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ca11-124">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>
##### <a name="response"></a><span data-ttu-id="8ca11-125">响应</span><span class="sxs-lookup"><span data-stu-id="8ca11-125">Response</span></span>
<span data-ttu-id="8ca11-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ca11-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->