# <a name="fileattachment-resource-type"></a><span data-ttu-id="07ae9-101">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="07ae9-101">fileAttachment resource type</span></span>

<span data-ttu-id="07ae9-p101">事件、邮件或帖子中附加的文件（例如文本文件或 Word 文档）。**contentBytes** 属性包含文件的 base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="07ae9-p101">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="07ae9-104">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="07ae9-104">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="07ae9-105">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="07ae9-105">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="07ae9-106">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="07ae9-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="07ae9-107">方法</span><span class="sxs-lookup"><span data-stu-id="07ae9-107">Methods</span></span>

| <span data-ttu-id="07ae9-108">方法</span><span class="sxs-lookup"><span data-stu-id="07ae9-108">Method</span></span>       | <span data-ttu-id="07ae9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="07ae9-109">Return Type</span></span>  |<span data-ttu-id="07ae9-110">说明</span><span class="sxs-lookup"><span data-stu-id="07ae9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07ae9-111">Get</span><span class="sxs-lookup"><span data-stu-id="07ae9-111">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="07ae9-112">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="07ae9-112">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="07ae9-113">读取 fileattachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07ae9-113">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="07ae9-114">删除</span><span class="sxs-lookup"><span data-stu-id="07ae9-114">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="07ae9-115">无</span><span class="sxs-lookup"><span data-stu-id="07ae9-115">None</span></span> |<span data-ttu-id="07ae9-116">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="07ae9-116">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="07ae9-117">属性</span><span class="sxs-lookup"><span data-stu-id="07ae9-117">Properties</span></span>
| <span data-ttu-id="07ae9-118">属性</span><span class="sxs-lookup"><span data-stu-id="07ae9-118">Property</span></span>     | <span data-ttu-id="07ae9-119">类型</span><span class="sxs-lookup"><span data-stu-id="07ae9-119">Type</span></span>   |<span data-ttu-id="07ae9-120">说明</span><span class="sxs-lookup"><span data-stu-id="07ae9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07ae9-121">contentBytes</span><span class="sxs-lookup"><span data-stu-id="07ae9-121">contentBytes</span></span>|<span data-ttu-id="07ae9-122">Binary</span><span class="sxs-lookup"><span data-stu-id="07ae9-122">Binary</span></span>|<span data-ttu-id="07ae9-123">文件的二进制内容。</span><span class="sxs-lookup"><span data-stu-id="07ae9-123">The binary contents of the file.</span></span>|
|<span data-ttu-id="07ae9-124">contentId</span><span class="sxs-lookup"><span data-stu-id="07ae9-124">contentId</span></span>|<span data-ttu-id="07ae9-125">String</span><span class="sxs-lookup"><span data-stu-id="07ae9-125">String</span></span>|<span data-ttu-id="07ae9-126">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="07ae9-126">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="07ae9-127">contentLocation</span><span class="sxs-lookup"><span data-stu-id="07ae9-127">contentLocation</span></span>|<span data-ttu-id="07ae9-128">String</span><span class="sxs-lookup"><span data-stu-id="07ae9-128">String</span></span>|<span data-ttu-id="07ae9-129">对应于附件内容所在位置的统一资源标识符 (URI)。</span><span class="sxs-lookup"><span data-stu-id="07ae9-129">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="07ae9-130">contentType</span><span class="sxs-lookup"><span data-stu-id="07ae9-130">contentType</span></span>|<span data-ttu-id="07ae9-131">String</span><span class="sxs-lookup"><span data-stu-id="07ae9-131">String</span></span>|<span data-ttu-id="07ae9-132">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="07ae9-132">The content type of the attachment.</span></span>|
|<span data-ttu-id="07ae9-133">id</span><span class="sxs-lookup"><span data-stu-id="07ae9-133">id</span></span>|<span data-ttu-id="07ae9-134">String</span><span class="sxs-lookup"><span data-stu-id="07ae9-134">String</span></span>|<span data-ttu-id="07ae9-135">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="07ae9-135">The attachment ID.</span></span>|
|<span data-ttu-id="07ae9-136">isInline</span><span class="sxs-lookup"><span data-stu-id="07ae9-136">isInline</span></span>|<span data-ttu-id="07ae9-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="07ae9-137">Boolean</span></span>|<span data-ttu-id="07ae9-138">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="07ae9-138">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="07ae9-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07ae9-139">lastModifiedDateTime</span></span>|<span data-ttu-id="07ae9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07ae9-140">DateTimeOffset</span></span>|<span data-ttu-id="07ae9-141">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07ae9-141">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="07ae9-142">name</span><span class="sxs-lookup"><span data-stu-id="07ae9-142">name</span></span>|<span data-ttu-id="07ae9-143">String</span><span class="sxs-lookup"><span data-stu-id="07ae9-143">String</span></span>|<span data-ttu-id="07ae9-144">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="07ae9-144">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="07ae9-145">size</span><span class="sxs-lookup"><span data-stu-id="07ae9-145">size</span></span>|<span data-ttu-id="07ae9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="07ae9-146">Int32</span></span>|<span data-ttu-id="07ae9-147">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="07ae9-147">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07ae9-148">关系</span><span class="sxs-lookup"><span data-stu-id="07ae9-148">Relationships</span></span>
<span data-ttu-id="07ae9-149">无</span><span class="sxs-lookup"><span data-stu-id="07ae9-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="07ae9-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07ae9-150">JSON representation</span></span>

<span data-ttu-id="07ae9-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07ae9-151">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
