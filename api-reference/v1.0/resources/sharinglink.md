# <a name="sharinglink-resource-type"></a><span data-ttu-id="802b0-101">SharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="802b0-101">SharingLink resource type</span></span>

<span data-ttu-id="802b0-102">**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="802b0-102">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="802b0-103">如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。</span><span class="sxs-lookup"><span data-stu-id="802b0-103">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="802b0-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="802b0-104">JSON representation</span></span>

<span data-ttu-id="802b0-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="802b0-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="802b0-106">属性</span><span class="sxs-lookup"><span data-stu-id="802b0-106">Properties</span></span>

| <span data-ttu-id="802b0-107">属性</span><span class="sxs-lookup"><span data-stu-id="802b0-107">Property</span></span>    | <span data-ttu-id="802b0-108">类型</span><span class="sxs-lookup"><span data-stu-id="802b0-108">Type</span></span>                    | <span data-ttu-id="802b0-109">说明</span><span class="sxs-lookup"><span data-stu-id="802b0-109">Description</span></span>                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="802b0-110">application</span><span class="sxs-lookup"><span data-stu-id="802b0-110">application</span></span> | [<span data-ttu-id="802b0-111">标识</span><span class="sxs-lookup"><span data-stu-id="802b0-111">identity</span></span>](identity.md) | <span data-ttu-id="802b0-112">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="802b0-112">The app the link is associated with.</span></span>                                                                                                                                                                    |
| <span data-ttu-id="802b0-113">type</span><span class="sxs-lookup"><span data-stu-id="802b0-113">type</span></span>        | <span data-ttu-id="802b0-114">String</span><span class="sxs-lookup"><span data-stu-id="802b0-114">String</span></span>                  | <span data-ttu-id="802b0-115">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="802b0-115">The type of the link created.</span></span>                                                                                                                                                                           |
| <span data-ttu-id="802b0-116">scope</span><span class="sxs-lookup"><span data-stu-id="802b0-116">scope</span></span>       | <span data-ttu-id="802b0-117">String</span><span class="sxs-lookup"><span data-stu-id="802b0-117">String</span></span>                  | <span data-ttu-id="802b0-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="802b0-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span> |
| <span data-ttu-id="802b0-120">webUrl</span><span class="sxs-lookup"><span data-stu-id="802b0-120">webUrl</span></span>      | <span data-ttu-id="802b0-121">String</span><span class="sxs-lookup"><span data-stu-id="802b0-121">String</span></span>                  | <span data-ttu-id="802b0-122">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="802b0-122">A URL that opens the item in the browser on the OneDrive website.</span></span>                                                                                                                                       |

## <a name="type-enumeration"></a><span data-ttu-id="802b0-123">类型枚举</span><span class="sxs-lookup"><span data-stu-id="802b0-123">Type enumeration</span></span>

<span data-ttu-id="802b0-124">此表定义了 **type** 属性的可能值：</span><span class="sxs-lookup"><span data-stu-id="802b0-124">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="802b0-125">值</span><span class="sxs-lookup"><span data-stu-id="802b0-125">Value</span></span>   | <span data-ttu-id="802b0-126">角色</span><span class="sxs-lookup"><span data-stu-id="802b0-126">Role</span></span>    | <span data-ttu-id="802b0-127">说明</span><span class="sxs-lookup"><span data-stu-id="802b0-127">Description</span></span>                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | <span data-ttu-id="802b0-128">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="802b0-128">A view-only sharing link, allowing read-only access.</span></span>                            |
| `edit`  | `write` | <span data-ttu-id="802b0-129">编辑共享链接，允许读写访问。</span><span class="sxs-lookup"><span data-stu-id="802b0-129">An edit sharing link, allowing read-write access.</span></span>                               |

## <a name="scope-enumeration"></a><span data-ttu-id="802b0-130">范围枚举</span><span class="sxs-lookup"><span data-stu-id="802b0-130">Scope enumeration</span></span>

| <span data-ttu-id="802b0-131">值</span><span class="sxs-lookup"><span data-stu-id="802b0-131">Value</span></span>          | <span data-ttu-id="802b0-132">说明</span><span class="sxs-lookup"><span data-stu-id="802b0-132">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="802b0-133">任何人均可使用共享链接。</span><span class="sxs-lookup"><span data-stu-id="802b0-133">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="802b0-p102">同一组织（租户）中的任何人均可使用共享链接。不适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="802b0-p102">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
