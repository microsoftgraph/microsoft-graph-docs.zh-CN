# <a name="add-tab-to-channel"></a><span data-ttu-id="179aa-101">选项卡添加到频道</span><span class="sxs-lookup"><span data-stu-id="179aa-101">Add tab to channel</span></span>



<span data-ttu-id="179aa-102">将 (pin) 添加到[团队](../resources/team.md)中指定的[频道](../resources/channel.md)一个[选项卡](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="179aa-102">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="179aa-103">相应的应用程序已必须[安装在工作组中](../api/teamsappinstallation_add.md)。</span><span class="sxs-lookup"><span data-stu-id="179aa-103">The corresponding app must already be [installed in the team](../api/teamsappinstallation_add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="179aa-104">权限</span><span class="sxs-lookup"><span data-stu-id="179aa-104">Permissions</span></span>
<span data-ttu-id="179aa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="179aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="179aa-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="179aa-107">Permission type</span></span>      | <span data-ttu-id="179aa-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="179aa-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="179aa-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="179aa-109">Delegated (work or school account)</span></span> | <span data-ttu-id="179aa-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="179aa-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="179aa-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="179aa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="179aa-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="179aa-112">Not supported.</span></span>    |
| <span data-ttu-id="179aa-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="179aa-113">Application</span></span>                            | <span data-ttu-id="179aa-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="179aa-114">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="179aa-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="179aa-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="179aa-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="179aa-116">Request headers</span></span>
| <span data-ttu-id="179aa-117">标头</span><span class="sxs-lookup"><span data-stu-id="179aa-117">Header</span></span>       | <span data-ttu-id="179aa-118">值</span><span class="sxs-lookup"><span data-stu-id="179aa-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="179aa-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="179aa-119">Authorization</span></span>  | <span data-ttu-id="179aa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="179aa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="179aa-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="179aa-122">Request body</span></span>

<span data-ttu-id="179aa-123">[TeamsTab](../resources/teamstab.md)。</span><span class="sxs-lookup"><span data-stu-id="179aa-123">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="179aa-124">响应</span><span class="sxs-lookup"><span data-stu-id="179aa-124">Response</span></span>

<span data-ttu-id="179aa-125">如果成功，此方法返回 `201 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="179aa-125">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="179aa-126">示例</span><span class="sxs-lookup"><span data-stu-id="179aa-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="179aa-127">请求</span><span class="sxs-lookup"><span data-stu-id="179aa-127">Request</span></span>

<span data-ttu-id="179aa-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="179aa-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="179aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="179aa-129">Response</span></span>

<span data-ttu-id="179aa-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="179aa-130">The following is an example of the response.</span></span> <span data-ttu-id="179aa-131">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="179aa-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="179aa-132">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="179aa-132">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "name": "My Contoso Tab",
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

## <a name="see-also"></a><span data-ttu-id="179aa-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="179aa-133">See also</span></span>

[<span data-ttu-id="179aa-134">配置到内置选项卡的类型</span><span class="sxs-lookup"><span data-stu-id="179aa-134">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
