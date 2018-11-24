# <a name="list-joinedteams"></a><span data-ttu-id="31772-101">列表 joinedTeams</span><span class="sxs-lookup"><span data-stu-id="31772-101">List joinedTeams</span></span>



<span data-ttu-id="31772-102">获取用户已是直接成员的 Microsoft 团队中的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="31772-102">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="31772-103">权限</span><span class="sxs-lookup"><span data-stu-id="31772-103">Permissions</span></span>
<span data-ttu-id="31772-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="31772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31772-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="31772-106">Permission type</span></span>      | <span data-ttu-id="31772-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31772-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31772-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31772-108">Delegated (work or school account)</span></span> | <span data-ttu-id="31772-109">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31772-109">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="31772-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31772-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31772-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="31772-111">Not supported.</span></span>    |
|<span data-ttu-id="31772-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="31772-112">Application</span></span> | <span data-ttu-id="31772-113">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31772-113">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="31772-114">用户委派权限与此操作仅适用于 me 用户。</span><span class="sxs-lookup"><span data-stu-id="31772-114">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="31772-115">应用程序权限，它适用于所有用户通过指定的特定用户 id。（me 别名不支持应用程序权限）</span><span class="sxs-lookup"><span data-stu-id="31772-115">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="31772-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31772-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31772-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31772-117">Optional query parameters</span></span>
<span data-ttu-id="31772-118">目前不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="31772-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31772-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="31772-119">Request headers</span></span>
| <span data-ttu-id="31772-120">标头</span><span class="sxs-lookup"><span data-stu-id="31772-120">Header</span></span>       | <span data-ttu-id="31772-121">值</span><span class="sxs-lookup"><span data-stu-id="31772-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31772-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31772-122">Authorization</span></span>  | <span data-ttu-id="31772-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31772-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31772-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31772-125">Accept</span></span>  | <span data-ttu-id="31772-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31772-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31772-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31772-127">Request body</span></span>
<span data-ttu-id="31772-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31772-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31772-129">响应</span><span class="sxs-lookup"><span data-stu-id="31772-129">Response</span></span>

<span data-ttu-id="31772-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="31772-130">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31772-131">示例</span><span class="sxs-lookup"><span data-stu-id="31772-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31772-132">请求</span><span class="sxs-lookup"><span data-stu-id="31772-132">Request</span></span>
<span data-ttu-id="31772-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31772-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="31772-134">响应</span><span class="sxs-lookup"><span data-stu-id="31772-134">Response</span></span>
<span data-ttu-id="31772-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31772-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="31772-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="31772-138">See also</span></span>
[<span data-ttu-id="31772-139">列出所有团队</span><span class="sxs-lookup"><span data-stu-id="31772-139">List all teams</span></span>](../../../concepts/teams_list_all_teams.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
