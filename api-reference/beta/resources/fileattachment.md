---
title: fileAttachment 资源类型
description: 附加到事件，文件 （如文本文件或 Word 文档中）
ms.openlocfilehash: 2a43ebbc78d831e907bfd19d647e4b7e398abe90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045671"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="8f0f5-103">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f0f5-103">fileAttachment resource type</span></span>

> <span data-ttu-id="8f0f5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f0f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f0f5-106">附加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)（如文本文件或 Word 文档） 的文件。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-106">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="8f0f5-107">**ContentBytes**属性将包含 base64 编码的文件的内容。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-107">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="8f0f5-108">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="8f0f5-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="8f0f5-109">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="8f0f5-110">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8f0f5-111">方法</span><span class="sxs-lookup"><span data-stu-id="8f0f5-111">Methods</span></span>

| <span data-ttu-id="8f0f5-112">方法</span><span class="sxs-lookup"><span data-stu-id="8f0f5-112">Method</span></span>       | <span data-ttu-id="8f0f5-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f0f5-113">Return Type</span></span>  |<span data-ttu-id="8f0f5-114">说明</span><span class="sxs-lookup"><span data-stu-id="8f0f5-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f0f5-115">Get</span><span class="sxs-lookup"><span data-stu-id="8f0f5-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="8f0f5-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="8f0f5-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="8f0f5-117">读取 fileattachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-117">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="8f0f5-118">删除</span><span class="sxs-lookup"><span data-stu-id="8f0f5-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="8f0f5-119">无</span><span class="sxs-lookup"><span data-stu-id="8f0f5-119">None</span></span> |<span data-ttu-id="8f0f5-120">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f0f5-121">属性</span><span class="sxs-lookup"><span data-stu-id="8f0f5-121">Properties</span></span>
| <span data-ttu-id="8f0f5-122">属性</span><span class="sxs-lookup"><span data-stu-id="8f0f5-122">Property</span></span>     | <span data-ttu-id="8f0f5-123">类型</span><span class="sxs-lookup"><span data-stu-id="8f0f5-123">Type</span></span>   |<span data-ttu-id="8f0f5-124">说明</span><span class="sxs-lookup"><span data-stu-id="8f0f5-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f0f5-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="8f0f5-125">contentBytes</span></span>|<span data-ttu-id="8f0f5-126">Binary</span><span class="sxs-lookup"><span data-stu-id="8f0f5-126">Binary</span></span>|<span data-ttu-id="8f0f5-127">文件的 Base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="8f0f5-128">contentId</span><span class="sxs-lookup"><span data-stu-id="8f0f5-128">contentId</span></span>|<span data-ttu-id="8f0f5-129">String</span><span class="sxs-lookup"><span data-stu-id="8f0f5-129">String</span></span>|<span data-ttu-id="8f0f5-130">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="8f0f5-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="8f0f5-131">contentLocation</span></span>|<span data-ttu-id="8f0f5-132">String</span><span class="sxs-lookup"><span data-stu-id="8f0f5-132">String</span></span>|<span data-ttu-id="8f0f5-133">对应于附件内容所在位置的统一资源标识符 (URI)。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-133">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="8f0f5-134">contentType</span><span class="sxs-lookup"><span data-stu-id="8f0f5-134">contentType</span></span>|<span data-ttu-id="8f0f5-135">String</span><span class="sxs-lookup"><span data-stu-id="8f0f5-135">String</span></span>|<span data-ttu-id="8f0f5-136">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="8f0f5-137">id</span><span class="sxs-lookup"><span data-stu-id="8f0f5-137">id</span></span>|<span data-ttu-id="8f0f5-138">String</span><span class="sxs-lookup"><span data-stu-id="8f0f5-138">String</span></span>|<span data-ttu-id="8f0f5-139">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-139">The attachment ID.</span></span>|
|<span data-ttu-id="8f0f5-140">isInline</span><span class="sxs-lookup"><span data-stu-id="8f0f5-140">isInline</span></span>|<span data-ttu-id="8f0f5-141">布尔</span><span class="sxs-lookup"><span data-stu-id="8f0f5-141">Boolean</span></span>|<span data-ttu-id="8f0f5-142">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="8f0f5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f0f5-143">lastModifiedDateTime</span></span>|<span data-ttu-id="8f0f5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f0f5-144">DateTimeOffset</span></span>|<span data-ttu-id="8f0f5-145">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="8f0f5-146">name</span><span class="sxs-lookup"><span data-stu-id="8f0f5-146">name</span></span>|<span data-ttu-id="8f0f5-147">String</span><span class="sxs-lookup"><span data-stu-id="8f0f5-147">String</span></span>|<span data-ttu-id="8f0f5-148">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="8f0f5-149">size</span><span class="sxs-lookup"><span data-stu-id="8f0f5-149">size</span></span>|<span data-ttu-id="8f0f5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8f0f5-150">Int32</span></span>|<span data-ttu-id="8f0f5-151">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f0f5-152">Relationships</span><span class="sxs-lookup"><span data-stu-id="8f0f5-152">Relationships</span></span>
<span data-ttu-id="8f0f5-153">无</span><span class="sxs-lookup"><span data-stu-id="8f0f5-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f0f5-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f0f5-154">JSON representation</span></span>

<span data-ttu-id="8f0f5-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f0f5-155">Here is a JSON representation of the resource</span></span>

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
