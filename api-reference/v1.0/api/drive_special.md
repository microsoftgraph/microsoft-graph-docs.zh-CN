# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="7a92d-101">按名称获取特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="7a92d-101">Get a special folder by name</span></span>

<span data-ttu-id="7a92d-102">使用特殊集合可以按名称访问特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="7a92d-102">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="7a92d-p101">特殊文件夹可以提供简单别名来访问 OneDrive 中的已知文件夹，无需按路径查找（需要本地化）或通过 ID 引用文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续查找该文件夹。</span><span class="sxs-lookup"><span data-stu-id="7a92d-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="7a92d-p102">应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="7a92d-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

><span data-ttu-id="7a92d-107">**注意：**如果你拥有只读权限并且请求不存在的特殊文件夹，将收到 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="7a92d-107">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a92d-108">权限</span><span class="sxs-lookup"><span data-stu-id="7a92d-108">Permissions</span></span>

<span data-ttu-id="7a92d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7a92d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7a92d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a92d-111">Permission type</span></span>                        | <span data-ttu-id="7a92d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a92d-112">Permissions (from least to most privileged)</span></span>                                                           |
|:--------------------------------------|:------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="7a92d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a92d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a92d-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a92d-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="7a92d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a92d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a92d-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Files.ReadWrite.AppFolder</span><span class="sxs-lookup"><span data-stu-id="7a92d-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span></span>           |
|<span data-ttu-id="7a92d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a92d-117">Application</span></span>                            | <span data-ttu-id="7a92d-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a92d-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="7a92d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a92d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a92d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7a92d-120">Optional query parameters</span></span>

<span data-ttu-id="7a92d-121">此方法支持使用 `$expand` 和 `$select` [OData 查询参数](../../../concepts/query_parameters.md)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7a92d-121">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a92d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a92d-122">Request headers</span></span>

| <span data-ttu-id="7a92d-123">名称</span><span class="sxs-lookup"><span data-stu-id="7a92d-123">Name</span></span>          | <span data-ttu-id="7a92d-124">类型</span><span class="sxs-lookup"><span data-stu-id="7a92d-124">Type</span></span>   | <span data-ttu-id="7a92d-125">说明</span><span class="sxs-lookup"><span data-stu-id="7a92d-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="7a92d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a92d-126">Authorization</span></span> | <span data-ttu-id="7a92d-127">string</span><span class="sxs-lookup"><span data-stu-id="7a92d-127">string</span></span> | <span data-ttu-id="7a92d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a92d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a92d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a92d-130">Request body</span></span>

<span data-ttu-id="7a92d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a92d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a92d-132">响应</span><span class="sxs-lookup"><span data-stu-id="7a92d-132">Response</span></span>

<span data-ttu-id="7a92d-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a92d-133">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a92d-134">示例</span><span class="sxs-lookup"><span data-stu-id="7a92d-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7a92d-135">请求</span><span class="sxs-lookup"><span data-stu-id="7a92d-135">Request</span></span>

<span data-ttu-id="7a92d-136">下面是一个请求用户驱动器的示例。</span><span class="sxs-lookup"><span data-stu-id="7a92d-136">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="7a92d-137">响应</span><span class="sxs-lookup"><span data-stu-id="7a92d-137">Response</span></span>
<span data-ttu-id="7a92d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7a92d-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="7a92d-139">注解</span><span class="sxs-lookup"><span data-stu-id="7a92d-139">Remarks</span></span>

<span data-ttu-id="7a92d-140">若要请求特殊文件夹的子文件夹，则可以请求 `children` 集合，或使用 [$expand](../../../concepts/query_parameters.md) 选项展开子集合。</span><span class="sxs-lookup"><span data-stu-id="7a92d-140">To request the children of a special folder, you can request the `children` collection or use the [expand](../../../concepts/query_parameters.md) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
