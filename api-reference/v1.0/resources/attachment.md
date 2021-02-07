---
title: attachment 资源类型
description: 可向事件添加相关的内容，
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a965c7cb7afc2961b15b24af3acf3c6597910754
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135784"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="96df2-103">attachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="96df2-103">attachment resource type</span></span>

<span data-ttu-id="96df2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96df2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96df2-105">可以附件形式向用户[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)添加相关内容。</span><span class="sxs-lookup"><span data-stu-id="96df2-105">You can add related content to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="96df2-106">**附件** 是以下附件派生类型的基础资源：</span><span class="sxs-lookup"><span data-stu-id="96df2-106">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="96df2-107">文件（[fileAttachment](../resources/fileattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="96df2-107">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="96df2-108">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）</span><span class="sxs-lookup"><span data-stu-id="96df2-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="96df2-109">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）</span><span class="sxs-lookup"><span data-stu-id="96df2-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

<span data-ttu-id="96df2-110">组日历中的事件不支持附件。</span><span class="sxs-lookup"><span data-stu-id="96df2-110">Events in group calendars do not support attachments.</span></span>

## <a name="methods"></a><span data-ttu-id="96df2-111">方法</span><span class="sxs-lookup"><span data-stu-id="96df2-111">Methods</span></span>

<span data-ttu-id="96df2-112">以下方法适用于所有附件派生类型（**fileAttachment**、**itemAttachment** 或 **referenceAttachment**）。</span><span class="sxs-lookup"><span data-stu-id="96df2-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="96df2-113">方法</span><span class="sxs-lookup"><span data-stu-id="96df2-113">Method</span></span>       | <span data-ttu-id="96df2-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="96df2-114">Return Type</span></span>  |<span data-ttu-id="96df2-115">说明</span><span class="sxs-lookup"><span data-stu-id="96df2-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96df2-116">获取附件</span><span class="sxs-lookup"><span data-stu-id="96df2-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="96df2-117">attachment</span><span class="sxs-lookup"><span data-stu-id="96df2-117">attachment</span></span>](attachment.md) |<span data-ttu-id="96df2-118">读取附加到事件、邮件或帖子的附件的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="96df2-118">Read the properties, relationships, or raw contents of an attachment, attached to a user event, message, or post.</span></span>|
|[<span data-ttu-id="96df2-119">将附件添加到用户事件中</span><span class="sxs-lookup"><span data-stu-id="96df2-119">Add attachment to a user event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="96df2-120">附件</span><span class="sxs-lookup"><span data-stu-id="96df2-120">attachment</span></span>](attachment.md) |<span data-ttu-id="96df2-121">将文件、项目或链接附件添加到用户日历中的事件中。</span><span class="sxs-lookup"><span data-stu-id="96df2-121">Add a file, item, or link attachment to an event in a user calendar.</span></span>|
|[<span data-ttu-id="96df2-122">将附件添加到邮件中</span><span class="sxs-lookup"><span data-stu-id="96df2-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="96df2-123">附件</span><span class="sxs-lookup"><span data-stu-id="96df2-123">attachment</span></span>](attachment.md) |<span data-ttu-id="96df2-124">将文件、项目或将附件链接添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="96df2-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="96df2-125">将附件添加到帖子中</span><span class="sxs-lookup"><span data-stu-id="96df2-125">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="96df2-126">附件</span><span class="sxs-lookup"><span data-stu-id="96df2-126">attachment</span></span>](attachment.md) |<span data-ttu-id="96df2-127">将文件、项目或将附件链接添加到帖子中。</span><span class="sxs-lookup"><span data-stu-id="96df2-127">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="96df2-128">列出用户事件的附件</span><span class="sxs-lookup"><span data-stu-id="96df2-128">List attachments of a user event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="96df2-129">[附件](attachment.md)集合</span><span class="sxs-lookup"><span data-stu-id="96df2-129">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="96df2-130">获取用户日历中事件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="96df2-130">Get a list of attachments for an event in a user calendar.</span></span> |
|[<span data-ttu-id="96df2-131">列出邮件的附件</span><span class="sxs-lookup"><span data-stu-id="96df2-131">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="96df2-132">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96df2-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="96df2-133">获取邮件的附件列表。</span><span class="sxs-lookup"><span data-stu-id="96df2-133">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="96df2-134">列出帖子的附件</span><span class="sxs-lookup"><span data-stu-id="96df2-134">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="96df2-135">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96df2-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="96df2-136">获取帖子的附件列表。</span><span class="sxs-lookup"><span data-stu-id="96df2-136">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="96df2-137">删除</span><span class="sxs-lookup"><span data-stu-id="96df2-137">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="96df2-138">无</span><span class="sxs-lookup"><span data-stu-id="96df2-138">None</span></span> |<span data-ttu-id="96df2-139">删除事件、邮件或帖子的附件。</span><span class="sxs-lookup"><span data-stu-id="96df2-139">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="96df2-140">属性</span><span class="sxs-lookup"><span data-stu-id="96df2-140">Properties</span></span>

<span data-ttu-id="96df2-p101">下面介绍了任意 attachment 资源的基础属性。有关其他属性，请参阅具体附件类型（[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)）。</span><span class="sxs-lookup"><span data-stu-id="96df2-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="96df2-143">属性</span><span class="sxs-lookup"><span data-stu-id="96df2-143">Property</span></span>     | <span data-ttu-id="96df2-144">类型</span><span class="sxs-lookup"><span data-stu-id="96df2-144">Type</span></span>   |<span data-ttu-id="96df2-145">说明</span><span class="sxs-lookup"><span data-stu-id="96df2-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96df2-146">contentType</span><span class="sxs-lookup"><span data-stu-id="96df2-146">contentType</span></span>|<span data-ttu-id="96df2-147">String</span><span class="sxs-lookup"><span data-stu-id="96df2-147">String</span></span>|<span data-ttu-id="96df2-148">MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="96df2-148">The MIME type.</span></span>|
|<span data-ttu-id="96df2-149">id</span><span class="sxs-lookup"><span data-stu-id="96df2-149">id</span></span>|<span data-ttu-id="96df2-150">String</span><span class="sxs-lookup"><span data-stu-id="96df2-150">String</span></span>| <span data-ttu-id="96df2-151">只读。</span><span class="sxs-lookup"><span data-stu-id="96df2-151">Read-only.</span></span>|
|<span data-ttu-id="96df2-152">isInline</span><span class="sxs-lookup"><span data-stu-id="96df2-152">isInline</span></span>|<span data-ttu-id="96df2-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="96df2-153">Boolean</span></span>|<span data-ttu-id="96df2-154">如果附件是内嵌附件，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="96df2-154">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="96df2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96df2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="96df2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96df2-156">DateTimeOffset</span></span>|<span data-ttu-id="96df2-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96df2-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96df2-159">名称</span><span class="sxs-lookup"><span data-stu-id="96df2-159">name</span></span>|<span data-ttu-id="96df2-160">String</span><span class="sxs-lookup"><span data-stu-id="96df2-160">String</span></span>|<span data-ttu-id="96df2-161">附件的文件名。</span><span class="sxs-lookup"><span data-stu-id="96df2-161">The attachment's file name.</span></span>|
|<span data-ttu-id="96df2-162">size</span><span class="sxs-lookup"><span data-stu-id="96df2-162">size</span></span>|<span data-ttu-id="96df2-163">Int32</span><span class="sxs-lookup"><span data-stu-id="96df2-163">Int32</span></span>|<span data-ttu-id="96df2-164">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="96df2-164">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96df2-165">关系</span><span class="sxs-lookup"><span data-stu-id="96df2-165">Relationships</span></span>
<span data-ttu-id="96df2-166">无</span><span class="sxs-lookup"><span data-stu-id="96df2-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96df2-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96df2-167">JSON representation</span></span>

<span data-ttu-id="96df2-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96df2-168">Here is a JSON representation of the resource</span></span>

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

