# <a name="add-app-to-team"></a><span data-ttu-id="422d3-101">将应用程序添加到团队</span><span class="sxs-lookup"><span data-stu-id="422d3-101">Add app to team</span></span>



<span data-ttu-id="422d3-102">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="422d3-102">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="422d3-103">权限</span><span class="sxs-lookup"><span data-stu-id="422d3-103">Permissions</span></span>
<span data-ttu-id="422d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="422d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="422d3-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="422d3-106">Permission type</span></span>      | <span data-ttu-id="422d3-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="422d3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="422d3-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="422d3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="422d3-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422d3-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="422d3-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="422d3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="422d3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="422d3-111">Not supported.</span></span>    |
|<span data-ttu-id="422d3-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="422d3-112">Application</span></span> | <span data-ttu-id="422d3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="422d3-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="422d3-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="422d3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="422d3-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="422d3-115">Request headers</span></span>
| <span data-ttu-id="422d3-116">标头</span><span class="sxs-lookup"><span data-stu-id="422d3-116">Header</span></span>       | <span data-ttu-id="422d3-117">值</span><span class="sxs-lookup"><span data-stu-id="422d3-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="422d3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="422d3-118">Authorization</span></span>  | <span data-ttu-id="422d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="422d3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="422d3-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="422d3-121">Request body</span></span>

| <span data-ttu-id="422d3-122">属性</span><span class="sxs-lookup"><span data-stu-id="422d3-122">Property</span></span>     | <span data-ttu-id="422d3-123">类型</span><span class="sxs-lookup"><span data-stu-id="422d3-123">Type</span></span>   |<span data-ttu-id="422d3-124">说明</span><span class="sxs-lookup"><span data-stu-id="422d3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="422d3-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="422d3-125">teamsApp</span></span>| [<span data-ttu-id="422d3-126">teamsApp</span><span class="sxs-lookup"><span data-stu-id="422d3-126">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="422d3-127">添加应用程序。</span><span class="sxs-lookup"><span data-stu-id="422d3-127">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="422d3-128">响应</span><span class="sxs-lookup"><span data-stu-id="422d3-128">Response</span></span>

<span data-ttu-id="422d3-129">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="422d3-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="422d3-130">示例</span><span class="sxs-lookup"><span data-stu-id="422d3-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="422d3-131">请求</span><span class="sxs-lookup"><span data-stu-id="422d3-131">Request</span></span>
<span data-ttu-id="422d3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="422d3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="422d3-133">响应</span><span class="sxs-lookup"><span data-stu-id="422d3-133">Response</span></span>
<span data-ttu-id="422d3-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="422d3-134">The following is an example of the response.</span></span> <span data-ttu-id="422d3-135">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="422d3-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="422d3-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="422d3-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
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

## <a name="see-also"></a><span data-ttu-id="422d3-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="422d3-137">See also</span></span>

