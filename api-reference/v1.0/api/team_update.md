# <a name="update-team"></a><span data-ttu-id="2e6c7-101">更新团队</span><span class="sxs-lookup"><span data-stu-id="2e6c7-101">Update team</span></span>



<span data-ttu-id="2e6c7-102">更新指定的[团队](../resources/team.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="2e6c7-102">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e6c7-103">权限</span><span class="sxs-lookup"><span data-stu-id="2e6c7-103">Permissions</span></span>
<span data-ttu-id="2e6c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2e6c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="2e6c7-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e6c7-106">Permission type</span></span>      | <span data-ttu-id="2e6c7-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e6c7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e6c7-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e6c7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2e6c7-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e6c7-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e6c7-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e6c7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e6c7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e6c7-111">Not supported.</span></span>    |
|<span data-ttu-id="2e6c7-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e6c7-112">Application</span></span> | <span data-ttu-id="2e6c7-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e6c7-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="2e6c7-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e6c7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e6c7-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e6c7-115">Request headers</span></span>
| <span data-ttu-id="2e6c7-116">标头</span><span class="sxs-lookup"><span data-stu-id="2e6c7-116">Header</span></span>       | <span data-ttu-id="2e6c7-117">值</span><span class="sxs-lookup"><span data-stu-id="2e6c7-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e6c7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e6c7-118">Authorization</span></span>  | <span data-ttu-id="2e6c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e6c7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2e6c7-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e6c7-121">Content-Type</span></span>  | <span data-ttu-id="2e6c7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2e6c7-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e6c7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e6c7-123">Request body</span></span>
<span data-ttu-id="2e6c7-124">在请求正文中，提供[团队](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e6c7-124">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2e6c7-125">响应</span><span class="sxs-lookup"><span data-stu-id="2e6c7-125">Response</span></span>

<span data-ttu-id="2e6c7-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2e6c7-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2e6c7-127">示例</span><span class="sxs-lookup"><span data-stu-id="2e6c7-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2e6c7-128">请求</span><span class="sxs-lookup"><span data-stu-id="2e6c7-128">Request</span></span>
<span data-ttu-id="2e6c7-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2e6c7-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="2e6c7-130">响应</span><span class="sxs-lookup"><span data-stu-id="2e6c7-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
