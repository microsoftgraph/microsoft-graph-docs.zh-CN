# <a name="unarchive-team"></a><span data-ttu-id="7586e-101">Unarchive 团队</span><span class="sxs-lookup"><span data-stu-id="7586e-101">Unarchive team</span></span>



<span data-ttu-id="7586e-102">还原存档的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="7586e-102">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="7586e-103">这将还原发送消息和编辑团队，遵守租户和工作组设置用户的功能。</span><span class="sxs-lookup"><span data-stu-id="7586e-103">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="7586e-104">工作组已存档使用[存档](team_archive.md)API。</span><span class="sxs-lookup"><span data-stu-id="7586e-104">Teams are archived using the [archive](team_archive.md) API.</span></span>

<span data-ttu-id="7586e-105">Unarchiving 是异步操作。</span><span class="sxs-lookup"><span data-stu-id="7586e-105">Unarchiving is an async operation.</span></span> <span data-ttu-id="7586e-106">一旦异步操作已成功完成，此 API 响应后可能出现的团队未存档。</span><span class="sxs-lookup"><span data-stu-id="7586e-106">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="7586e-107">权限</span><span class="sxs-lookup"><span data-stu-id="7586e-107">Permissions</span></span>
<span data-ttu-id="7586e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7586e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7586e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7586e-110">Permission type</span></span>      | <span data-ttu-id="7586e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7586e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7586e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7586e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7586e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7586e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7586e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7586e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7586e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7586e-115">Not supported.</span></span>    |
|<span data-ttu-id="7586e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7586e-116">Application</span></span> | <span data-ttu-id="7586e-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7586e-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7586e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7586e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="7586e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7586e-119">Request headers</span></span>
| <span data-ttu-id="7586e-120">标头</span><span class="sxs-lookup"><span data-stu-id="7586e-120">Header</span></span>       | <span data-ttu-id="7586e-121">值</span><span class="sxs-lookup"><span data-stu-id="7586e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7586e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7586e-122">Authorization</span></span>  | <span data-ttu-id="7586e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7586e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7586e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7586e-125">Request body</span></span>
<span data-ttu-id="7586e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7586e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7586e-127">响应</span><span class="sxs-lookup"><span data-stu-id="7586e-127">Response</span></span>

<span data-ttu-id="7586e-128">如果 unarchiving 已成功启动，此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="7586e-128">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="7586e-129">响应还将包含`Location`标头，其中包含的[teamsAsyncOperation](../resources/teamsasyncoperation.md)创建处理 unarchiving 团队的位置。</span><span class="sxs-lookup"><span data-stu-id="7586e-129">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="7586e-130">通过对此位置进行 GET 请求检查 unarchiving 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7586e-130">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="7586e-131">示例</span><span class="sxs-lookup"><span data-stu-id="7586e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7586e-132">请求</span><span class="sxs-lookup"><span data-stu-id="7586e-132">Request</span></span>
<span data-ttu-id="7586e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7586e-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="7586e-134">响应</span><span class="sxs-lookup"><span data-stu-id="7586e-134">Response</span></span>
<span data-ttu-id="7586e-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="7586e-135">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
