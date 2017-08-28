# <a name="referenceattachment-resource-type"></a><span data-ttu-id="3c572-101">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c572-101">referenceAttachment resource type</span></span>

<span data-ttu-id="3c572-102">到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。</span><span class="sxs-lookup"><span data-stu-id="3c572-102">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="3c572-103">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="3c572-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3c572-104">方法</span><span class="sxs-lookup"><span data-stu-id="3c572-104">Methods</span></span>

| <span data-ttu-id="3c572-105">方法</span><span class="sxs-lookup"><span data-stu-id="3c572-105">Method</span></span>       | <span data-ttu-id="3c572-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c572-106">Return Type</span></span>  |<span data-ttu-id="3c572-107">说明</span><span class="sxs-lookup"><span data-stu-id="3c572-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c572-108">Get</span><span class="sxs-lookup"><span data-stu-id="3c572-108">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="3c572-109">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="3c572-109">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="3c572-110">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c572-110">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="3c572-111">删除</span><span class="sxs-lookup"><span data-stu-id="3c572-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="3c572-112">无</span><span class="sxs-lookup"><span data-stu-id="3c572-112">None</span></span> |<span data-ttu-id="3c572-113">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="3c572-113">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3c572-114">属性</span><span class="sxs-lookup"><span data-stu-id="3c572-114">Properties</span></span>
| <span data-ttu-id="3c572-115">属性</span><span class="sxs-lookup"><span data-stu-id="3c572-115">Property</span></span>     | <span data-ttu-id="3c572-116">类型</span><span class="sxs-lookup"><span data-stu-id="3c572-116">Type</span></span>   |<span data-ttu-id="3c572-117">说明</span><span class="sxs-lookup"><span data-stu-id="3c572-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c572-118">contentType</span><span class="sxs-lookup"><span data-stu-id="3c572-118">contentType</span></span>|<span data-ttu-id="3c572-119">String</span><span class="sxs-lookup"><span data-stu-id="3c572-119">String</span></span>|<span data-ttu-id="3c572-120">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="3c572-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="3c572-121">id</span><span class="sxs-lookup"><span data-stu-id="3c572-121">id</span></span>|<span data-ttu-id="3c572-122">String</span><span class="sxs-lookup"><span data-stu-id="3c572-122">String</span></span>|<span data-ttu-id="3c572-p101">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="3c572-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="3c572-125">isInline</span><span class="sxs-lookup"><span data-stu-id="3c572-125">isInline</span></span>|<span data-ttu-id="3c572-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c572-126">Boolean</span></span>|<span data-ttu-id="3c572-127">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3c572-127">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="3c572-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c572-128">lastModifiedDateTime</span></span>|<span data-ttu-id="3c572-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c572-129">DateTimeOffset</span></span>|<span data-ttu-id="3c572-p102">上次修改附件的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3c572-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3c572-133">名称</span><span class="sxs-lookup"><span data-stu-id="3c572-133">name</span></span>|<span data-ttu-id="3c572-134">String</span><span class="sxs-lookup"><span data-stu-id="3c572-134">String</span></span>|<span data-ttu-id="3c572-p103">显示在用于表示嵌入附件的图标下方的文本。这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="3c572-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="3c572-137">size</span><span class="sxs-lookup"><span data-stu-id="3c572-137">size</span></span>|<span data-ttu-id="3c572-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3c572-138">Int32</span></span>|<span data-ttu-id="3c572-139">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="3c572-139">The size of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c572-140">关系</span><span class="sxs-lookup"><span data-stu-id="3c572-140">Relationships</span></span>
<span data-ttu-id="3c572-141">无</span><span class="sxs-lookup"><span data-stu-id="3c572-141">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="3c572-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c572-142">JSON representation</span></span>

<span data-ttu-id="3c572-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c572-143">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
