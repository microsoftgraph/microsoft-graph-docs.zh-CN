# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="a5d95-101">为 DriveItem 创建共享链接</span><span class="sxs-lookup"><span data-stu-id="a5d95-101">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="a5d95-102">可以使用 **createLink** 操作通过共享链接共享 [DriveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a5d95-102">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="a5d95-p101">如果调用应用程序指定的链接类型尚不存在，**CreateLink** 操作将创建新的共享链接。如果应用程序指定的共享链接类型已存在，则返回现有的共享链接。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="a5d95-105">DriveItem 资源从其上级继承权限。</span><span class="sxs-lookup"><span data-stu-id="a5d95-105">DriveItem resources inherit permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5d95-106">权限</span><span class="sxs-lookup"><span data-stu-id="a5d95-106">Permissions</span></span>
<span data-ttu-id="a5d95-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5d95-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5d95-109">Permission type</span></span>      | <span data-ttu-id="a5d95-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5d95-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="a5d95-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5d95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5d95-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d95-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="a5d95-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5d95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5d95-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d95-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="a5d95-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5d95-115">Application</span></span> | <span data-ttu-id="a5d95-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d95-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a5d95-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5d95-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a><span data-ttu-id="a5d95-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5d95-118">Request body</span></span>
<span data-ttu-id="a5d95-p103">请求正文定义应用程序正在查找的共享链接的类型。请求应是具有此属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p103">The body of the request defines the type of sharing link your application is looking for. The request should be a JSON object with this property.</span></span>

| <span data-ttu-id="a5d95-121">名称</span><span class="sxs-lookup"><span data-stu-id="a5d95-121">Name</span></span>      | <span data-ttu-id="a5d95-122">类型</span><span class="sxs-lookup"><span data-stu-id="a5d95-122">Type</span></span>   | <span data-ttu-id="a5d95-123">说明</span><span class="sxs-lookup"><span data-stu-id="a5d95-123">Description</span></span>                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| <span data-ttu-id="a5d95-124">**类型**</span><span class="sxs-lookup"><span data-stu-id="a5d95-124">**type**</span></span>  | <span data-ttu-id="a5d95-125">string</span><span class="sxs-lookup"><span data-stu-id="a5d95-125">string</span></span> | <span data-ttu-id="a5d95-p104">要创建的共享链接的类型。`view`、`edit` 或 `embed`。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="a5d95-128">**scope**</span><span class="sxs-lookup"><span data-stu-id="a5d95-128">**scope**</span></span> | <span data-ttu-id="a5d95-129">string</span><span class="sxs-lookup"><span data-stu-id="a5d95-129">string</span></span> | <span data-ttu-id="a5d95-p105">要创建的链接的范围。`anonymous` 或 `organization`。可选。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p105">The scope of link to create. Either `anonymous` or `organization`. Optional.</span></span> |

## <a name="link-types"></a><span data-ttu-id="a5d95-133">链接类型</span><span class="sxs-lookup"><span data-stu-id="a5d95-133">Link types</span></span>
<span data-ttu-id="a5d95-134">**type** 参数允许使用以下值：</span><span class="sxs-lookup"><span data-stu-id="a5d95-134">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="a5d95-135">类型值</span><span class="sxs-lookup"><span data-stu-id="a5d95-135">Type value</span></span> | <span data-ttu-id="a5d95-136">说明</span><span class="sxs-lookup"><span data-stu-id="a5d95-136">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="a5d95-137">创建到项目的只读链接。</span><span class="sxs-lookup"><span data-stu-id="a5d95-137">Creates a read-only link to the item.</span></span>                                                        |
| `edit`     | <span data-ttu-id="a5d95-138">创建到项目的读写链接。</span><span class="sxs-lookup"><span data-stu-id="a5d95-138">Creates a read-write link to the item.</span></span>                                                       |
| `embed`    | <span data-ttu-id="a5d95-p106">创建到项目的可嵌入链接。此选项仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p106">Creates an embeddable link to the item. This option is only available for OneDrive Personal.</span></span> |

## <a name="scope-types"></a><span data-ttu-id="a5d95-141">范围类型</span><span class="sxs-lookup"><span data-stu-id="a5d95-141">Scope types</span></span>
<span data-ttu-id="a5d95-p107">**scope** 参数允许使用以下值。这是一个可选参数。如果未指定 **scope** 参数，则将创建最大可用权限的链接。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p107">The following values are allowed for the **scope** parameter. This is an optional parameter. If the **scope** parameter is not specified, the most permissive link available will be created.</span></span>

| <span data-ttu-id="a5d95-145">类型值</span><span class="sxs-lookup"><span data-stu-id="a5d95-145">Type value</span></span>     | <span data-ttu-id="a5d95-146">说明</span><span class="sxs-lookup"><span data-stu-id="a5d95-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="a5d95-p108">创建到任意用户都可访问的项目的链接。租户管理员可禁用匿名链接。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p108">Creates a link to the item accessible to anyone. Anonymous links may be disabled by the tenant administrator.</span></span>                 |
| `organization` | <span data-ttu-id="a5d95-p109">创建到组织内部人员都可访问的项目的链接。组织连接范围不适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p109">Creates a link to the item accessible within an organization. Organization link scope is not available for OneDrive Personal.</span></span> |

## <a name="response"></a><span data-ttu-id="a5d95-151">响应</span><span class="sxs-lookup"><span data-stu-id="a5d95-151">Response</span></span>

<span data-ttu-id="a5d95-152">如果成功，此方法将在响应正文中返回单个 [Permission](../resources/permission.md) 资源，此响应正文表示请求的共享链接的权限。</span><span class="sxs-lookup"><span data-stu-id="a5d95-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing link permission.</span></span>

<span data-ttu-id="a5d95-153">本服务首先查看当前权限，并检查是否已存在与调用应用程序**类型**相同的链接。</span><span class="sxs-lookup"><span data-stu-id="a5d95-153">The service will first look at the current permissions and check if one already exists that has the same **type** for the calling application.</span></span>

<span data-ttu-id="a5d95-154">如果已经为此项目创建新的共享链接，响应为 `201 Created`；如果返回现有链接，则为 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="a5d95-154">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="a5d95-155">示例</span><span class="sxs-lookup"><span data-stu-id="a5d95-155">Example</span></span>
<span data-ttu-id="a5d95-156">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a5d95-156">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a5d95-157">请求</span><span class="sxs-lookup"><span data-stu-id="a5d95-157">Request</span></span>
<span data-ttu-id="a5d95-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5d95-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a><span data-ttu-id="a5d95-159">响应</span><span class="sxs-lookup"><span data-stu-id="a5d95-159">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="a5d95-160">创建公司可共享的链接</span><span class="sxs-lookup"><span data-stu-id="a5d95-160">Creating company sharable links</span></span>

<span data-ttu-id="a5d95-p110">OneDrive for Business 和 SharePoint 都支持公司可共享的链接。此类链接与匿名链接类似，但仅适用于拥有租户的成员。若要创建公司可共享的链接，请使用值为 `organization` 的 **scope** 参数。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p110">OneDrive for Business and SharePoint support company sharable links. These are similar to anonymous links, except they only work for members of the owning tenant. To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

## <a name="http-request"></a><span data-ttu-id="a5d95-164">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5d95-164">HTTP request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a><span data-ttu-id="a5d95-165">HTTP 响应</span><span class="sxs-lookup"><span data-stu-id="a5d95-165">HTTP response</span></span>

<span data-ttu-id="a5d95-166">如果已经为此项目创建新的共享链接，响应为 `201 Created`；如果返回现有链接，则为 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="a5d95-166">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a><span data-ttu-id="a5d95-167">可嵌入的链接</span><span class="sxs-lookup"><span data-stu-id="a5d95-167">Embeddable links</span></span>

<span data-ttu-id="a5d95-p111">使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。</span><span class="sxs-lookup"><span data-stu-id="a5d95-p111">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="a5d95-170">**注意：**仅 **driveType** 为 `personal` 的 [驱动器](../resources/drive.md) 支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="a5d95-170">**Note:** Embed links are only supported in [Drives](../resources/drive.md) where the **driveType** is `personal`.</span></span>

## <a name="remarks"></a><span data-ttu-id="a5d95-171">注释</span><span class="sxs-lookup"><span data-stu-id="a5d95-171">Remarks</span></span>

* <span data-ttu-id="a5d95-172">使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。</span><span class="sxs-lookup"><span data-stu-id="a5d95-172">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="a5d95-173">链接在项的共享权限中可见，可以由该项的所有者删除。</span><span class="sxs-lookup"><span data-stu-id="a5d95-173">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="a5d95-174">除非项已被签出，否则链接始终指向该项的最新版本（仅限 SharePoint）。</span><span class="sxs-lookup"><span data-stu-id="a5d95-174">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
