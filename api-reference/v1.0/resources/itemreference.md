# <a name="itemreference-resource-type"></a><span data-ttu-id="43be1-101">ItemReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="43be1-101">ItemReference resource type</span></span>

<span data-ttu-id="43be1-102">**ItemReference** 资源提供了通过 API 查找 [DriveItem](driveitem.md) 的必要信息。</span><span class="sxs-lookup"><span data-stu-id="43be1-102">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="43be1-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43be1-103">JSON representation</span></span>

<span data-ttu-id="43be1-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43be1-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="43be1-105">属性</span><span class="sxs-lookup"><span data-stu-id="43be1-105">Properties</span></span>

| <span data-ttu-id="43be1-106">属性</span><span class="sxs-lookup"><span data-stu-id="43be1-106">Property</span></span>      | <span data-ttu-id="43be1-107">类型</span><span class="sxs-lookup"><span data-stu-id="43be1-107">Type</span></span>                              | <span data-ttu-id="43be1-108">说明</span><span class="sxs-lookup"><span data-stu-id="43be1-108">Description</span></span>                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="43be1-109">driveId</span><span class="sxs-lookup"><span data-stu-id="43be1-109">driveId</span></span>       | <span data-ttu-id="43be1-110">字符串</span><span class="sxs-lookup"><span data-stu-id="43be1-110">String</span></span>                            | <span data-ttu-id="43be1-p101">包含项的驱动器实例的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="43be1-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>                                 |
| <span data-ttu-id="43be1-113">id</span><span class="sxs-lookup"><span data-stu-id="43be1-113">id</span></span>            | <span data-ttu-id="43be1-114">String</span><span class="sxs-lookup"><span data-stu-id="43be1-114">String</span></span>                            | <span data-ttu-id="43be1-p102">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="43be1-p102">Unique identifier of the item in the drive. Read-only.</span></span>                                                     |
| <span data-ttu-id="43be1-117">name</span><span class="sxs-lookup"><span data-stu-id="43be1-117">name</span></span>          | <span data-ttu-id="43be1-118">字符串</span><span class="sxs-lookup"><span data-stu-id="43be1-118">String</span></span>                            | <span data-ttu-id="43be1-p103">所引用的项的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="43be1-p103">The name of the item being referenced. Read-only.</span></span>                                                          |
| <span data-ttu-id="43be1-121">路径</span><span class="sxs-lookup"><span data-stu-id="43be1-121">path</span></span>          | <span data-ttu-id="43be1-122">String</span><span class="sxs-lookup"><span data-stu-id="43be1-122">String</span></span>                            | <span data-ttu-id="43be1-p104">可用于导航到该项的路径。只读。</span><span class="sxs-lookup"><span data-stu-id="43be1-p104">Path that can be used to navigate to the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="43be1-125">shareId</span><span class="sxs-lookup"><span data-stu-id="43be1-125">shareId</span></span>       | <span data-ttu-id="43be1-126">String</span><span class="sxs-lookup"><span data-stu-id="43be1-126">String</span></span>                            | <span data-ttu-id="43be1-127">可通过 [Shares](../api/shares_get.md) API 访问共享资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="43be1-127">A unique identifier for a shared resource that can be accessed via the [Shares](../api/shares_get.md) API.</span></span> |
| <span data-ttu-id="43be1-128">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="43be1-128">sharepointIds</span></span> | [<span data-ttu-id="43be1-129">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="43be1-129">sharepointIds</span></span>](sharepointids.md) | <span data-ttu-id="43be1-p105">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="43be1-p105">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                   |

## <a name="remarks"></a><span data-ttu-id="43be1-132">注解</span><span class="sxs-lookup"><span data-stu-id="43be1-132">Remarks</span></span>

<span data-ttu-id="43be1-133">为了从 **itemReference** 资源中找到 **driveItem**，请构建以下格式的 URL：</span><span class="sxs-lookup"><span data-stu-id="43be1-133">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="43be1-134">**path** 值是相对于目标驱动器的 API 路径，例如：`/drive/root:/Documents/myfile.docx`。</span><span class="sxs-lookup"><span data-stu-id="43be1-134">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="43be1-135">要检索人工可读路径中的痕迹，可以放心地忽略路径字符串中的第一个 `:` 之前的所有内容。</span><span class="sxs-lookup"><span data-stu-id="43be1-135">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
