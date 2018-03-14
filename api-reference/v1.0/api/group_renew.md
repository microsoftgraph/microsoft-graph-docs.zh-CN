# <a name="group-renew"></a><span data-ttu-id="b7c61-101">group: renew</span><span class="sxs-lookup"><span data-stu-id="b7c61-101">group: renew</span></span>

<span data-ttu-id="b7c61-102">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="b7c61-102">Renews a group's expiration.</span></span> <span data-ttu-id="b7c61-103">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="b7c61-103">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7c61-104">权限</span><span class="sxs-lookup"><span data-stu-id="b7c61-104">Permissions</span></span>

<span data-ttu-id="b7c61-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b7c61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="b7c61-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7c61-107">Permission type</span></span>      | <span data-ttu-id="b7c61-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7c61-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7c61-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7c61-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b7c61-110">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c61-110">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7c61-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7c61-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7c61-112">不支持</span><span class="sxs-lookup"><span data-stu-id="b7c61-112">Not supported</span></span> |
|<span data-ttu-id="b7c61-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7c61-113">Application</span></span> | <span data-ttu-id="b7c61-114">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c61-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7c61-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7c61-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/<id>/renew
```

## <a name="request-headers"></a><span data-ttu-id="b7c61-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7c61-116">Request headers</span></span>
| <span data-ttu-id="b7c61-117">名称</span><span class="sxs-lookup"><span data-stu-id="b7c61-117">Name</span></span>       | <span data-ttu-id="b7c61-118">说明</span><span class="sxs-lookup"><span data-stu-id="b7c61-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7c61-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c61-119">Authorization</span></span>  | <span data-ttu-id="b7c61-120">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b7c61-120">Bearer %token%</span></span> |


## <a name="request-body"></a><span data-ttu-id="b7c61-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7c61-121">Request body</span></span>

<span data-ttu-id="b7c61-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7c61-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7c61-123">响应</span><span class="sxs-lookup"><span data-stu-id="b7c61-123">Response</span></span>

<span data-ttu-id="b7c61-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b7c61-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c61-126">示例</span><span class="sxs-lookup"><span data-stu-id="b7c61-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b7c61-127">请求</span><span class="sxs-lookup"><span data-stu-id="b7c61-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/<id>/renew
```

##### <a name="response"></a><span data-ttu-id="b7c61-128">响应</span><span class="sxs-lookup"><span data-stu-id="b7c61-128">Response</span></span>
<span data-ttu-id="b7c61-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7c61-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->