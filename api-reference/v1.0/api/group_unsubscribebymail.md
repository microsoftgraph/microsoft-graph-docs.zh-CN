# <a name="group-unsubscribebymail"></a><span data-ttu-id="b4623-101">组：unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="b4623-101">group: unsubscribeByMail</span></span>

<span data-ttu-id="b4623-p101">调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="b4623-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 
## <a name="permissions"></a><span data-ttu-id="b4623-104">权限</span><span class="sxs-lookup"><span data-stu-id="b4623-104">Permissions</span></span>
<span data-ttu-id="b4623-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b4623-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b4623-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4623-107">Permission type</span></span>      | <span data-ttu-id="b4623-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4623-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b4623-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4623-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b4623-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4623-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b4623-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4623-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4623-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4623-112">Not supported.</span></span>    | 
|<span data-ttu-id="b4623-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4623-113">Application</span></span> | <span data-ttu-id="b4623-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4623-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b4623-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4623-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="b4623-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4623-116">Request headers</span></span>
| <span data-ttu-id="b4623-117">标头</span><span class="sxs-lookup"><span data-stu-id="b4623-117">Header</span></span>       | <span data-ttu-id="b4623-118">值</span><span class="sxs-lookup"><span data-stu-id="b4623-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4623-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4623-119">Authorization</span></span>  | <span data-ttu-id="b4623-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4623-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4623-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4623-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b4623-123">响应</span><span class="sxs-lookup"><span data-stu-id="b4623-123">Response</span></span>
<span data-ttu-id="b4623-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4623-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4623-126">示例</span><span class="sxs-lookup"><span data-stu-id="b4623-126">Example</span></span>
<span data-ttu-id="b4623-127">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b4623-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b4623-128">请求</span><span class="sxs-lookup"><span data-stu-id="b4623-128">Request</span></span>
<span data-ttu-id="b4623-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4623-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

##### <a name="response"></a><span data-ttu-id="b4623-130">响应</span><span class="sxs-lookup"><span data-stu-id="b4623-130">Response</span></span>
<span data-ttu-id="b4623-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4623-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
