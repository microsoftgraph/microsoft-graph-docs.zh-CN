# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="1c21a-101">升级团队中应用程序</span><span class="sxs-lookup"><span data-stu-id="1c21a-101">Upgrade an app in a team</span></span>



<span data-ttu-id="1c21a-102">升级[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1c21a-102">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c21a-103">权限</span><span class="sxs-lookup"><span data-stu-id="1c21a-103">Permissions</span></span>

<span data-ttu-id="1c21a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1c21a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c21a-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c21a-106">Permission type</span></span>      | <span data-ttu-id="1c21a-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c21a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c21a-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c21a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1c21a-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c21a-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1c21a-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c21a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c21a-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c21a-111">Not supported.</span></span>    |
|<span data-ttu-id="1c21a-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c21a-112">Application</span></span> | <span data-ttu-id="1c21a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c21a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c21a-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c21a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="1c21a-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c21a-115">Request headers</span></span>
| <span data-ttu-id="1c21a-116">标头</span><span class="sxs-lookup"><span data-stu-id="1c21a-116">Header</span></span>       | <span data-ttu-id="1c21a-117">值</span><span class="sxs-lookup"><span data-stu-id="1c21a-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c21a-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c21a-118">Authorization</span></span>  | <span data-ttu-id="1c21a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c21a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c21a-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c21a-121">Request body</span></span>
<span data-ttu-id="1c21a-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1c21a-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c21a-123">响应</span><span class="sxs-lookup"><span data-stu-id="1c21a-123">Response</span></span>

<span data-ttu-id="1c21a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1c21a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c21a-126">示例</span><span class="sxs-lookup"><span data-stu-id="1c21a-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1c21a-127">请求</span><span class="sxs-lookup"><span data-stu-id="1c21a-127">Request</span></span>
<span data-ttu-id="1c21a-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c21a-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="1c21a-129">响应</span><span class="sxs-lookup"><span data-stu-id="1c21a-129">Response</span></span>
<span data-ttu-id="1c21a-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1c21a-130">The following is an example of the response.</span></span> 

><span data-ttu-id="1c21a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c21a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
