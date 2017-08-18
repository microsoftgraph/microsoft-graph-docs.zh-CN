# <a name="remove-member"></a><span data-ttu-id="fb7d3-101">删除成员</span><span class="sxs-lookup"><span data-stu-id="fb7d3-101">Remove member</span></span>

<span data-ttu-id="fb7d3-p101">使用此 API 可以通过 **members** 导航属性删除 Office 365 组、安全组或已启用邮件的安全组中的成员。你可以删除用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="fb7d3-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb7d3-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb7d3-104">Prerequisites</span></span>
<span data-ttu-id="fb7d3-105">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All* 或 *Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="fb7d3-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="fb7d3-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb7d3-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fb7d3-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb7d3-107">Request headers</span></span>
| <span data-ttu-id="fb7d3-108">名称</span><span class="sxs-lookup"><span data-stu-id="fb7d3-108">Name</span></span>       | <span data-ttu-id="fb7d3-109">类型</span><span class="sxs-lookup"><span data-stu-id="fb7d3-109">Type</span></span> | <span data-ttu-id="fb7d3-110">说明</span><span class="sxs-lookup"><span data-stu-id="fb7d3-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fb7d3-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb7d3-111">Authorization</span></span>  | <span data-ttu-id="fb7d3-112">string</span><span class="sxs-lookup"><span data-stu-id="fb7d3-112">string</span></span>  | <span data-ttu-id="fb7d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb7d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb7d3-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb7d3-115">Request body</span></span>
<span data-ttu-id="fb7d3-116">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb7d3-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb7d3-117">响应</span><span class="sxs-lookup"><span data-stu-id="fb7d3-117">Response</span></span>

<span data-ttu-id="fb7d3-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fb7d3-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb7d3-120">示例</span><span class="sxs-lookup"><span data-stu-id="fb7d3-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb7d3-121">请求</span><span class="sxs-lookup"><span data-stu-id="fb7d3-121">Request</span></span>
<span data-ttu-id="fb7d3-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb7d3-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="fb7d3-123">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="fb7d3-123">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="fb7d3-124">响应</span><span class="sxs-lookup"><span data-stu-id="fb7d3-124">Response</span></span>
<span data-ttu-id="fb7d3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb7d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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