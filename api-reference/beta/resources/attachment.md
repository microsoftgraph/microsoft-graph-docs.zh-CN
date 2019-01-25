---
title: attachment 资源类型
description: 您可以将相关的内容添加到事件，
localization_priority: Normal
ms.openlocfilehash: 59e1074cea9508af45cef0b6e61ea223a3ca851e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526940"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="5cfff-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cfff-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cfff-104">您可以将相关的内容添加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或附件的形式[发布](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="5cfff-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="5cfff-105">**附件**是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="5cfff-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="5cfff-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="5cfff-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="5cfff-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="5cfff-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="5cfff-108">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="5cfff-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="5cfff-109">方法</span><span class="sxs-lookup"><span data-stu-id="5cfff-109">Methods</span></span>

<span data-ttu-id="5cfff-110">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="5cfff-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="5cfff-111">方法</span><span class="sxs-lookup"><span data-stu-id="5cfff-111">Method</span></span>       | <span data-ttu-id="5cfff-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="5cfff-112">Return Type</span></span>  |<span data-ttu-id="5cfff-113">说明</span><span class="sxs-lookup"><span data-stu-id="5cfff-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cfff-114">获取附件</span><span class="sxs-lookup"><span data-stu-id="5cfff-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="5cfff-115">attachment</span><span class="sxs-lookup"><span data-stu-id="5cfff-115">attachment</span></span>](attachment.md) |<span data-ttu-id="5cfff-116">读取的属性和附件，附加到事件、 邮件、 Outlook 任务或公告的关系。</span><span class="sxs-lookup"><span data-stu-id="5cfff-116">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="5cfff-117">Add attachment to an event</span><span class="sxs-lookup"><span data-stu-id="5cfff-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="5cfff-118">attachment</span><span class="sxs-lookup"><span data-stu-id="5cfff-118">attachment</span></span>](attachment.md) |<span data-ttu-id="5cfff-119">将文件、项目或链接附件添加到事件中。</span><span class="sxs-lookup"><span data-stu-id="5cfff-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="5cfff-120">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="5cfff-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="5cfff-121">attachment</span><span class="sxs-lookup"><span data-stu-id="5cfff-121">attachment</span></span>](attachment.md) |<span data-ttu-id="5cfff-122">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="5cfff-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="5cfff-123">将附件添加到 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="5cfff-123">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="5cfff-124">attachment</span><span class="sxs-lookup"><span data-stu-id="5cfff-124">attachment</span></span>](attachment.md) |<span data-ttu-id="5cfff-125">添加文件、 项或 Outlook 任务链接附件。</span><span class="sxs-lookup"><span data-stu-id="5cfff-125">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="5cfff-126">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="5cfff-126">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="5cfff-127">附件</span><span class="sxs-lookup"><span data-stu-id="5cfff-127">attachment</span></span>](attachment.md) |<span data-ttu-id="5cfff-128">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="5cfff-128">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="5cfff-129">列出事件的附件</span><span class="sxs-lookup"><span data-stu-id="5cfff-129">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="5cfff-130">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cfff-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="5cfff-131">获取事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="5cfff-131">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="5cfff-132">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="5cfff-132">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="5cfff-133">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cfff-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="5cfff-134">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="5cfff-134">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="5cfff-135">Outlook 任务的列出附件</span><span class="sxs-lookup"><span data-stu-id="5cfff-135">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="5cfff-136">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cfff-136">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="5cfff-137">获取附件 Outlook 任务的列表。</span><span class="sxs-lookup"><span data-stu-id="5cfff-137">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="5cfff-138">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="5cfff-138">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="5cfff-139">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5cfff-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="5cfff-140">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="5cfff-140">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="5cfff-141">删除</span><span class="sxs-lookup"><span data-stu-id="5cfff-141">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="5cfff-142">无</span><span class="sxs-lookup"><span data-stu-id="5cfff-142">None</span></span> |<span data-ttu-id="5cfff-143">删除事件、 邮件、 Outlook 任务或公告上的附件。</span><span class="sxs-lookup"><span data-stu-id="5cfff-143">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cfff-144">属性</span><span class="sxs-lookup"><span data-stu-id="5cfff-144">Properties</span></span>

<span data-ttu-id="5cfff-p101">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="5cfff-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="5cfff-147">属性</span><span class="sxs-lookup"><span data-stu-id="5cfff-147">Property</span></span>     | <span data-ttu-id="5cfff-148">类型</span><span class="sxs-lookup"><span data-stu-id="5cfff-148">Type</span></span>   |<span data-ttu-id="5cfff-149">说明</span><span class="sxs-lookup"><span data-stu-id="5cfff-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cfff-150">contentType</span><span class="sxs-lookup"><span data-stu-id="5cfff-150">contentType</span></span>|<span data-ttu-id="5cfff-151">String</span><span class="sxs-lookup"><span data-stu-id="5cfff-151">String</span></span>|<span data-ttu-id="5cfff-152">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="5cfff-152">The MIME type.</span></span>|
|<span data-ttu-id="5cfff-153">id</span><span class="sxs-lookup"><span data-stu-id="5cfff-153">id</span></span>|<span data-ttu-id="5cfff-154">String</span><span class="sxs-lookup"><span data-stu-id="5cfff-154">String</span></span>| <span data-ttu-id="5cfff-155">只读。</span><span class="sxs-lookup"><span data-stu-id="5cfff-155">Read-only.</span></span>|
|<span data-ttu-id="5cfff-156">isInline</span><span class="sxs-lookup"><span data-stu-id="5cfff-156">isInline</span></span>|<span data-ttu-id="5cfff-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cfff-157">Boolean</span></span>|<span data-ttu-id="5cfff-158">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="5cfff-158">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="5cfff-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cfff-159">lastModifiedDateTime</span></span>|<span data-ttu-id="5cfff-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cfff-160">DateTimeOffset</span></span>|<span data-ttu-id="5cfff-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5cfff-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5cfff-163">名称</span><span class="sxs-lookup"><span data-stu-id="5cfff-163">name</span></span>|<span data-ttu-id="5cfff-164">String</span><span class="sxs-lookup"><span data-stu-id="5cfff-164">String</span></span>|<span data-ttu-id="5cfff-165">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5cfff-165">The display name of the attachment.</span></span> <span data-ttu-id="5cfff-166">这不需要是实际的文件名称。</span><span class="sxs-lookup"><span data-stu-id="5cfff-166">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="5cfff-167">size</span><span class="sxs-lookup"><span data-stu-id="5cfff-167">size</span></span>|<span data-ttu-id="5cfff-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5cfff-168">Int32</span></span>|<span data-ttu-id="5cfff-169">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="5cfff-169">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cfff-170">关系</span><span class="sxs-lookup"><span data-stu-id="5cfff-170">Relationships</span></span>
<span data-ttu-id="5cfff-171">无</span><span class="sxs-lookup"><span data-stu-id="5cfff-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cfff-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cfff-172">JSON representation</span></span>

<span data-ttu-id="5cfff-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cfff-173">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
