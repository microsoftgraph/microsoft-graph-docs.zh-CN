# <a name="patch-channel"></a><span data-ttu-id="2c44b-101">修补程序通道</span><span class="sxs-lookup"><span data-stu-id="2c44b-101">Patch channel</span></span>



<span data-ttu-id="2c44b-102">更新指定的[频道](../resources/channel.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="2c44b-102">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="2c44b-103">**注意**： 没有应用程序权限和此 API 的已知的问题。</span><span class="sxs-lookup"><span data-stu-id="2c44b-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="2c44b-104">有关详细信息，请参阅[已知问题列表](../../../concepts/known_issues.md#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="2c44b-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c44b-105">权限</span><span class="sxs-lookup"><span data-stu-id="2c44b-105">Permissions</span></span>
<span data-ttu-id="2c44b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2c44b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2c44b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c44b-108">Permission type</span></span>      | <span data-ttu-id="2c44b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c44b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c44b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c44b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c44b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c44b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c44b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c44b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c44b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c44b-113">Not supported.</span></span>    |
|<span data-ttu-id="2c44b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c44b-114">Application</span></span> | <span data-ttu-id="2c44b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c44b-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c44b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c44b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2c44b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c44b-117">Request headers</span></span>
| <span data-ttu-id="2c44b-118">标头</span><span class="sxs-lookup"><span data-stu-id="2c44b-118">Header</span></span>       | <span data-ttu-id="2c44b-119">值</span><span class="sxs-lookup"><span data-stu-id="2c44b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c44b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c44b-120">Authorization</span></span>  | <span data-ttu-id="2c44b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c44b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c44b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c44b-123">Content-Type</span></span>  | <span data-ttu-id="2c44b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2c44b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c44b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c44b-125">Request body</span></span>
<span data-ttu-id="2c44b-126">在请求正文中，提供[信道](../resources/channel.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c44b-126">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2c44b-127">响应</span><span class="sxs-lookup"><span data-stu-id="2c44b-127">Response</span></span>

<span data-ttu-id="2c44b-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2c44b-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c44b-129">示例</span><span class="sxs-lookup"><span data-stu-id="2c44b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c44b-130">请求</span><span class="sxs-lookup"><span data-stu-id="2c44b-130">Request</span></span>
<span data-ttu-id="2c44b-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c44b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="2c44b-132">响应</span><span class="sxs-lookup"><span data-stu-id="2c44b-132">Response</span></span>
<span data-ttu-id="2c44b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c44b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
