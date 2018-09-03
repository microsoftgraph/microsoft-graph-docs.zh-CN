# <a name="itemattachment-resource-type"></a><span data-ttu-id="c01d6-101">itemAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c01d6-101">itemAttachment resource type</span></span>

<span data-ttu-id="c01d6-102">附加到另一个事件、邮件或帖子的联系人、事件或邮件。</span><span class="sxs-lookup"><span data-stu-id="c01d6-102">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="c01d6-103">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="c01d6-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c01d6-104">方法</span><span class="sxs-lookup"><span data-stu-id="c01d6-104">Methods</span></span>

| <span data-ttu-id="c01d6-105">方法</span><span class="sxs-lookup"><span data-stu-id="c01d6-105">Method</span></span>       | <span data-ttu-id="c01d6-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="c01d6-106">Return Type</span></span>  |<span data-ttu-id="c01d6-107">说明</span><span class="sxs-lookup"><span data-stu-id="c01d6-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c01d6-108">获取</span><span class="sxs-lookup"><span data-stu-id="c01d6-108">Get</span></span>](../api/attachment_get.md) | <span data-ttu-id="c01d6-109">[itemAttachment](itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="c01d6-109">[itemAttachment](itemattachment.md),</span></span> |<span data-ttu-id="c01d6-110">读取 itemAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c01d6-110">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="c01d6-111">删除</span><span class="sxs-lookup"><span data-stu-id="c01d6-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="c01d6-112">无</span><span class="sxs-lookup"><span data-stu-id="c01d6-112">None</span></span> |<span data-ttu-id="c01d6-113">删除 itemAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="c01d6-113">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c01d6-114">属性</span><span class="sxs-lookup"><span data-stu-id="c01d6-114">Properties</span></span>
| <span data-ttu-id="c01d6-115">属性</span><span class="sxs-lookup"><span data-stu-id="c01d6-115">Property</span></span>     | <span data-ttu-id="c01d6-116">类型</span><span class="sxs-lookup"><span data-stu-id="c01d6-116">Type</span></span>   |<span data-ttu-id="c01d6-117">说明</span><span class="sxs-lookup"><span data-stu-id="c01d6-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c01d6-118">contentType</span><span class="sxs-lookup"><span data-stu-id="c01d6-118">contentType</span></span>|<span data-ttu-id="c01d6-119">字符串</span><span class="sxs-lookup"><span data-stu-id="c01d6-119">String</span></span>|<span data-ttu-id="c01d6-120">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="c01d6-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="c01d6-121">ID</span><span class="sxs-lookup"><span data-stu-id="c01d6-121">id</span></span>|<span data-ttu-id="c01d6-122">字符串</span><span class="sxs-lookup"><span data-stu-id="c01d6-122">String</span></span>| <span data-ttu-id="c01d6-123">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="c01d6-123">The attachment ID.</span></span>|
|<span data-ttu-id="c01d6-124">isInline</span><span class="sxs-lookup"><span data-stu-id="c01d6-124">isInline</span></span>|<span data-ttu-id="c01d6-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="c01d6-125">Boolean</span></span>|<span data-ttu-id="c01d6-126">如果附件是内联的（例如嵌入到项目正文中的图像），请设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c01d6-126">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="c01d6-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c01d6-127">lastModifiedDateTime</span></span>|<span data-ttu-id="c01d6-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c01d6-128">DateTimeOffset</span></span>|<span data-ttu-id="c01d6-129">上次修改附件的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="c01d6-129">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="c01d6-130">名称</span><span class="sxs-lookup"><span data-stu-id="c01d6-130">name</span></span>|<span data-ttu-id="c01d6-131">字符串</span><span class="sxs-lookup"><span data-stu-id="c01d6-131">String</span></span>|<span data-ttu-id="c01d6-132">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c01d6-132">The display name of the attachment.</span></span>|
|<span data-ttu-id="c01d6-133">大小</span><span class="sxs-lookup"><span data-stu-id="c01d6-133">size</span></span>|<span data-ttu-id="c01d6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c01d6-134">Int32</span></span>|<span data-ttu-id="c01d6-135">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="c01d6-135">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c01d6-136">关系</span><span class="sxs-lookup"><span data-stu-id="c01d6-136">Relationships</span></span>
| <span data-ttu-id="c01d6-137">关系</span><span class="sxs-lookup"><span data-stu-id="c01d6-137">Relationship</span></span> | <span data-ttu-id="c01d6-138">类型</span><span class="sxs-lookup"><span data-stu-id="c01d6-138">Type</span></span>   |<span data-ttu-id="c01d6-139">说明</span><span class="sxs-lookup"><span data-stu-id="c01d6-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c01d6-140">项</span><span class="sxs-lookup"><span data-stu-id="c01d6-140">item</span></span>|[<span data-ttu-id="c01d6-141">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="c01d6-141">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="c01d6-p101">附加的消息或事件。导航属性。</span><span class="sxs-lookup"><span data-stu-id="c01d6-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c01d6-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c01d6-144">JSON representation</span></span>

<span data-ttu-id="c01d6-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c01d6-145">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
