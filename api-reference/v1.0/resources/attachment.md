# <a name="attachment-resource-type"></a><span data-ttu-id="fcf84-101">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcf84-101">attachment resource type</span></span>

<span data-ttu-id="fcf84-102">可以附件形式向[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)添加相关内容。</span><span class="sxs-lookup"><span data-stu-id="fcf84-102">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="fcf84-103">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="fcf84-103">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="fcf84-104">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="fcf84-104">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="fcf84-105">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="fcf84-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="fcf84-106">文件链接（[referenceAttachment](../resources/referenceAttachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="fcf84-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="fcf84-107">方法</span><span class="sxs-lookup"><span data-stu-id="fcf84-107">Methods</span></span>

<span data-ttu-id="fcf84-108">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="fcf84-108">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="fcf84-109">方法</span><span class="sxs-lookup"><span data-stu-id="fcf84-109">Method</span></span>       | <span data-ttu-id="fcf84-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="fcf84-110">Return Type</span></span>  |<span data-ttu-id="fcf84-111">说明</span><span class="sxs-lookup"><span data-stu-id="fcf84-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fcf84-112">获取附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-112">Get attachment</span></span>](../api/attachment_get.md) | [<span data-ttu-id="fcf84-113">附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-113">attachment</span></span>](attachment.md) |<span data-ttu-id="fcf84-114">读取附加到事件、邮件或帖子的附件的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fcf84-114">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="fcf84-115">向一个事件添加附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-115">Add attachment to an event</span></span>](../api/event_post_attachments.md) | [<span data-ttu-id="fcf84-116">附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-116">attachment</span></span>](attachment.md) |<span data-ttu-id="fcf84-117">将文件、项目或链接附件添加到事件中。</span><span class="sxs-lookup"><span data-stu-id="fcf84-117">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="fcf84-118">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="fcf84-118">Add attachment to a message</span></span>](../api/message_post_attachments.md) | [<span data-ttu-id="fcf84-119">附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-119">attachment</span></span>](attachment.md) |<span data-ttu-id="fcf84-120">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="fcf84-120">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="fcf84-121">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="fcf84-121">Add attachment to a post</span></span>](../api/post_post_attachments.md) | [<span data-ttu-id="fcf84-122">附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-122">attachment</span></span>](attachment.md) |<span data-ttu-id="fcf84-123">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="fcf84-123">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="fcf84-124">列出事件的附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-124">List attachments of an event</span></span>](../api/event_list_attachments.md) | <span data-ttu-id="fcf84-125">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fcf84-125">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="fcf84-126">获取事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="fcf84-126">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="fcf84-127">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-127">List attachments of a message</span></span>](../api/message_list_attachments.md) | <span data-ttu-id="fcf84-128">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fcf84-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="fcf84-129">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="fcf84-129">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="fcf84-130">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="fcf84-130">List attachments of a post</span></span>](../api/post_list_attachments.md) | <span data-ttu-id="fcf84-131">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fcf84-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="fcf84-132">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="fcf84-132">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="fcf84-133">删除</span><span class="sxs-lookup"><span data-stu-id="fcf84-133">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="fcf84-134">无</span><span class="sxs-lookup"><span data-stu-id="fcf84-134">None</span></span> |<span data-ttu-id="fcf84-135">删除事件、邮件或帖子的附件。</span><span class="sxs-lookup"><span data-stu-id="fcf84-135">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="fcf84-136">属性</span><span class="sxs-lookup"><span data-stu-id="fcf84-136">Properties</span></span>

<span data-ttu-id="fcf84-p101">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceAttachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="fcf84-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md)) for additional properties.</span></span>

| <span data-ttu-id="fcf84-139">属性</span><span class="sxs-lookup"><span data-stu-id="fcf84-139">Property</span></span>     | <span data-ttu-id="fcf84-140">类型</span><span class="sxs-lookup"><span data-stu-id="fcf84-140">Type</span></span>   |<span data-ttu-id="fcf84-141">说明</span><span class="sxs-lookup"><span data-stu-id="fcf84-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcf84-142">contentType</span><span class="sxs-lookup"><span data-stu-id="fcf84-142">contentType</span></span>|<span data-ttu-id="fcf84-143">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf84-143">String</span></span>|<span data-ttu-id="fcf84-144">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="fcf84-144">The MIME type.</span></span>|
|<span data-ttu-id="fcf84-145">id</span><span class="sxs-lookup"><span data-stu-id="fcf84-145">id</span></span>|<span data-ttu-id="fcf84-146">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf84-146">String</span></span>| <span data-ttu-id="fcf84-147">只读。</span><span class="sxs-lookup"><span data-stu-id="fcf84-147">Read-only.</span></span>|
|<span data-ttu-id="fcf84-148">isInline</span><span class="sxs-lookup"><span data-stu-id="fcf84-148">isInline</span></span>|<span data-ttu-id="fcf84-149">布尔</span><span class="sxs-lookup"><span data-stu-id="fcf84-149">Boolean</span></span>|<span data-ttu-id="fcf84-150">`true` 如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="fcf84-150">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="fcf84-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcf84-151">lastModifiedDateTime</span></span>|<span data-ttu-id="fcf84-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcf84-152">DateTimeOffset</span></span>|<span data-ttu-id="fcf84-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fcf84-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fcf84-155">名称</span><span class="sxs-lookup"><span data-stu-id="fcf84-155">name</span></span>|<span data-ttu-id="fcf84-156">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf84-156">String</span></span>|<span data-ttu-id="fcf84-157">附件的文件名。</span><span class="sxs-lookup"><span data-stu-id="fcf84-157">The attachment's file name.</span></span>|
|<span data-ttu-id="fcf84-158">size</span><span class="sxs-lookup"><span data-stu-id="fcf84-158">size</span></span>|<span data-ttu-id="fcf84-159">Int32</span><span class="sxs-lookup"><span data-stu-id="fcf84-159">Int32</span></span>|<span data-ttu-id="fcf84-160">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="fcf84-160">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcf84-161">关系</span><span class="sxs-lookup"><span data-stu-id="fcf84-161">Relationships</span></span>
<span data-ttu-id="fcf84-162">无</span><span class="sxs-lookup"><span data-stu-id="fcf84-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcf84-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcf84-163">JSON representation</span></span>

<span data-ttu-id="fcf84-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcf84-164">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
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
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
