# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="5776c-101">笔记本：getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="5776c-101">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="5776c-102">获取登录用户访问的 [recentNotebook](../resources/recentnotebook.md) 实例列表。</span><span class="sxs-lookup"><span data-stu-id="5776c-102">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5776c-103">权限</span><span class="sxs-lookup"><span data-stu-id="5776c-103">Permissions</span></span>
<span data-ttu-id="5776c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5776c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5776c-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="5776c-106">Permission type</span></span>      | <span data-ttu-id="5776c-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5776c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5776c-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5776c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5776c-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5776c-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="5776c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5776c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5776c-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5776c-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="5776c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="5776c-112">Application</span></span> | <span data-ttu-id="5776c-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5776c-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5776c-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5776c-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="5776c-115">用户的 `<id | userPrincipalName>` 必须与用于发出请求的授权令牌中编码的用户一致。</span><span class="sxs-lookup"><span data-stu-id="5776c-115">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="5776c-116">函数参数</span><span class="sxs-lookup"><span data-stu-id="5776c-116">Function parameters</span></span>

| <span data-ttu-id="5776c-117">参数</span><span class="sxs-lookup"><span data-stu-id="5776c-117">Parameter</span></span>    | <span data-ttu-id="5776c-118">类型</span><span class="sxs-lookup"><span data-stu-id="5776c-118">Type</span></span>   |<span data-ttu-id="5776c-119">说明</span><span class="sxs-lookup"><span data-stu-id="5776c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5776c-120">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="5776c-120">includePersonalNotebooks</span></span>|<span data-ttu-id="5776c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5776c-121">Boolean</span></span>|<span data-ttu-id="5776c-122">添加用户拥有的笔记本。</span><span class="sxs-lookup"><span data-stu-id="5776c-122">Include notebooks owned by the user.</span></span> <span data-ttu-id="5776c-123">若要添加用户拥有的笔记本，请设置为 `true`；否则，设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="5776c-123">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="5776c-124">如果不添加 `includePersonalNotebooks` 参数，请求会返回 `400` 错误响应。</span><span class="sxs-lookup"><span data-stu-id="5776c-124">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5776c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="5776c-125">Request headers</span></span>
| <span data-ttu-id="5776c-126">名称</span><span class="sxs-lookup"><span data-stu-id="5776c-126">Name</span></span>       | <span data-ttu-id="5776c-127">说明</span><span class="sxs-lookup"><span data-stu-id="5776c-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5776c-128">授权</span><span class="sxs-lookup"><span data-stu-id="5776c-128">Authorization</span></span>  | <span data-ttu-id="5776c-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5776c-129">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5776c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5776c-130">Request body</span></span>
<span data-ttu-id="5776c-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5776c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5776c-132">响应</span><span class="sxs-lookup"><span data-stu-id="5776c-132">Response</span></span>
<span data-ttu-id="5776c-133">如果成功响应，则返回 `200 OK`，其中包含 **recentNotebooks** 的 JSON 集合。</span><span class="sxs-lookup"><span data-stu-id="5776c-133">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="5776c-134">示例</span><span class="sxs-lookup"><span data-stu-id="5776c-134">Example</span></span>
<span data-ttu-id="5776c-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5776c-135">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5776c-136">请求</span><span class="sxs-lookup"><span data-stu-id="5776c-136">Request</span></span>
<span data-ttu-id="5776c-137">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="5776c-137">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="5776c-138">响应</span><span class="sxs-lookup"><span data-stu-id="5776c-138">Response</span></span>
<span data-ttu-id="5776c-139">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="5776c-139">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
