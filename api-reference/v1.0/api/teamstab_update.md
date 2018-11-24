# <a name="update-tab"></a><span data-ttu-id="5ae7e-101">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="5ae7e-101">Update tab</span></span>



<span data-ttu-id="5ae7e-102">更新指定的[选项卡上](../resources/teamstab.md)的属性。可以使用此配置的选项卡的内容。</span><span class="sxs-lookup"><span data-stu-id="5ae7e-102">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ae7e-103">权限</span><span class="sxs-lookup"><span data-stu-id="5ae7e-103">Permissions</span></span>
<span data-ttu-id="5ae7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5ae7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5ae7e-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ae7e-106">Permission type</span></span>      | <span data-ttu-id="5ae7e-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ae7e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ae7e-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ae7e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5ae7e-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae7e-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ae7e-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ae7e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ae7e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ae7e-111">Not supported.</span></span>    |
|<span data-ttu-id="5ae7e-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ae7e-112">Application</span></span>                            | <span data-ttu-id="5ae7e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae7e-113">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5ae7e-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ae7e-114">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5ae7e-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ae7e-115">Request headers</span></span>
| <span data-ttu-id="5ae7e-116">标头</span><span class="sxs-lookup"><span data-stu-id="5ae7e-116">Header</span></span>       | <span data-ttu-id="5ae7e-117">值</span><span class="sxs-lookup"><span data-stu-id="5ae7e-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ae7e-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ae7e-118">Authorization</span></span>  | <span data-ttu-id="5ae7e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ae7e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5ae7e-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ae7e-121">Content-Type</span></span>  | <span data-ttu-id="5ae7e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5ae7e-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ae7e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ae7e-123">Request body</span></span>
<span data-ttu-id="5ae7e-124">在请求正文中，提供[tab](../resources/teamstab.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ae7e-124">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5ae7e-125">响应</span><span class="sxs-lookup"><span data-stu-id="5ae7e-125">Response</span></span>

<span data-ttu-id="5ae7e-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5ae7e-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5ae7e-127">示例</span><span class="sxs-lookup"><span data-stu-id="5ae7e-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5ae7e-128">请求</span><span class="sxs-lookup"><span data-stu-id="5ae7e-128">Request</span></span>
<span data-ttu-id="5ae7e-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5ae7e-129">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="5ae7e-130">响应</span><span class="sxs-lookup"><span data-stu-id="5ae7e-130">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

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

## <a name="see-also"></a><span data-ttu-id="5ae7e-131">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5ae7e-131">See also</span></span>

[<span data-ttu-id="5ae7e-132">配置到内置选项卡的类型</span><span class="sxs-lookup"><span data-stu-id="5ae7e-132">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
