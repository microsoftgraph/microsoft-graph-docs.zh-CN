# <a name="get-tab"></a><span data-ttu-id="61141-101">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="61141-101">Get tab</span></span>



<span data-ttu-id="61141-102">检索的属性和指定的[选项卡](../resources/teamstab.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="61141-102">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="61141-103">权限</span><span class="sxs-lookup"><span data-stu-id="61141-103">Permissions</span></span>
<span data-ttu-id="61141-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="61141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61141-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="61141-106">Permission type</span></span>      | <span data-ttu-id="61141-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61141-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61141-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61141-108">Delegated (work or school account)</span></span> | <span data-ttu-id="61141-109">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61141-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="61141-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61141-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61141-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="61141-111">Not supported.</span></span>    |
|<span data-ttu-id="61141-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="61141-112">Application</span></span> | <span data-ttu-id="61141-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61141-113">Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="61141-114">目前，仅[委派权限](../../../concepts/permissions_reference.md)支持此操作。</span><span class="sxs-lookup"><span data-stu-id="61141-114">Currently, only [delegated permissions](../../../concepts/permissions_reference.md) are supported for this operation.</span></span>

## <a name="http-request"></a><span data-ttu-id="61141-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61141-115">HTTP request</span></span>
```http
GET /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61141-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="61141-116">Optional query parameters</span></span>

<span data-ttu-id="61141-117">此方法支持 $select，和 $expand [OData 查询参数](../../../concepts/query_parameters.md)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="61141-117">This method supports the $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61141-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="61141-118">Request headers</span></span>
| <span data-ttu-id="61141-119">标头</span><span class="sxs-lookup"><span data-stu-id="61141-119">Header</span></span>       | <span data-ttu-id="61141-120">值</span><span class="sxs-lookup"><span data-stu-id="61141-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61141-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="61141-121">Authorization</span></span>  | <span data-ttu-id="61141-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61141-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61141-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="61141-124">Request body</span></span>
<span data-ttu-id="61141-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61141-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61141-126">响应</span><span class="sxs-lookup"><span data-stu-id="61141-126">Response</span></span>

<span data-ttu-id="61141-127">如果成功，此方法返回`200 OK`响应代码和响应正文中的[选项卡](../resources/teamstab.md)对象。</span><span class="sxs-lookup"><span data-stu-id="61141-127">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61141-128">示例</span><span class="sxs-lookup"><span data-stu-id="61141-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="61141-129">请求</span><span class="sxs-lookup"><span data-stu-id="61141-129">Request</span></span>
<span data-ttu-id="61141-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61141-130">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="61141-131">响应</span><span class="sxs-lookup"><span data-stu-id="61141-131">Response</span></span>
<span data-ttu-id="61141-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61141-132">The following is an example of the response.</span></span> 

><span data-ttu-id="61141-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="61141-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
