# <a name="get-team"></a><span data-ttu-id="3b45a-101">获取工作组</span><span class="sxs-lookup"><span data-stu-id="3b45a-101">Get team</span></span>



<span data-ttu-id="3b45a-102">检索的属性和指定[团队](../resources/team.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="3b45a-102">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b45a-103">权限</span><span class="sxs-lookup"><span data-stu-id="3b45a-103">Permissions</span></span>
<span data-ttu-id="3b45a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3b45a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b45a-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b45a-106">Permission type</span></span>      | <span data-ttu-id="3b45a-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b45a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b45a-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b45a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3b45a-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b45a-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b45a-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b45a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b45a-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b45a-111">Not supported.</span></span>    |
|<span data-ttu-id="3b45a-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b45a-112">Application</span></span> | <span data-ttu-id="3b45a-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b45a-113">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="3b45a-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b45a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b45a-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3b45a-115">Optional query parameters</span></span>
<span data-ttu-id="3b45a-116">此方法支持 $select 和 $expand [OData 查询参数](../../../concepts/query_parameters.md)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="3b45a-116">This method supports the $select and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b45a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b45a-117">Request headers</span></span>
| <span data-ttu-id="3b45a-118">标头</span><span class="sxs-lookup"><span data-stu-id="3b45a-118">Header</span></span>       | <span data-ttu-id="3b45a-119">值</span><span class="sxs-lookup"><span data-stu-id="3b45a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b45a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b45a-120">Authorization</span></span>  | <span data-ttu-id="3b45a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b45a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b45a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b45a-123">Request body</span></span>
<span data-ttu-id="3b45a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b45a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b45a-125">响应</span><span class="sxs-lookup"><span data-stu-id="3b45a-125">Response</span></span>

<span data-ttu-id="3b45a-126">如果成功，此方法返回`200 OK`响应代码和响应正文中的[团队](../resources/team.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b45a-126">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b45a-127">示例</span><span class="sxs-lookup"><span data-stu-id="3b45a-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3b45a-128">请求</span><span class="sxs-lookup"><span data-stu-id="3b45a-128">Request</span></span>
<span data-ttu-id="3b45a-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3b45a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="3b45a-130">响应</span><span class="sxs-lookup"><span data-stu-id="3b45a-130">Response</span></span>
<span data-ttu-id="3b45a-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3b45a-131">The following is an example of the response.</span></span> 

><span data-ttu-id="3b45a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3b45a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
