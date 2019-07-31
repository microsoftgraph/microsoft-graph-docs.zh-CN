---
title: fileAttachment 资源类型
description: 附加到事件的文件 (如文本文件或 Word 文档)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 966de812c8b0507c3d757d42fba5624c0b82ce4f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972038"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="b1596-103">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1596-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1596-104">附加到[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[公告](../resources/post.md)的文件 (如文本文件或 Word 文档)。</span><span class="sxs-lookup"><span data-stu-id="b1596-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="b1596-105">**ContentBytes**属性包含文件的 base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="b1596-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="b1596-106">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="b1596-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="b1596-107">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="b1596-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="b1596-108">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="b1596-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b1596-109">方法</span><span class="sxs-lookup"><span data-stu-id="b1596-109">Methods</span></span>

| <span data-ttu-id="b1596-110">方法</span><span class="sxs-lookup"><span data-stu-id="b1596-110">Method</span></span>       | <span data-ttu-id="b1596-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1596-111">Return Type</span></span>  |<span data-ttu-id="b1596-112">说明</span><span class="sxs-lookup"><span data-stu-id="b1596-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1596-113">Get</span><span class="sxs-lookup"><span data-stu-id="b1596-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="b1596-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="b1596-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="b1596-115">读取 fileattachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1596-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="b1596-116">删除</span><span class="sxs-lookup"><span data-stu-id="b1596-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="b1596-117">无</span><span class="sxs-lookup"><span data-stu-id="b1596-117">None</span></span> |<span data-ttu-id="b1596-118">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="b1596-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b1596-119">属性</span><span class="sxs-lookup"><span data-stu-id="b1596-119">Properties</span></span>
| <span data-ttu-id="b1596-120">属性</span><span class="sxs-lookup"><span data-stu-id="b1596-120">Property</span></span>     | <span data-ttu-id="b1596-121">类型</span><span class="sxs-lookup"><span data-stu-id="b1596-121">Type</span></span>   |<span data-ttu-id="b1596-122">说明</span><span class="sxs-lookup"><span data-stu-id="b1596-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1596-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="b1596-123">contentBytes</span></span>|<span data-ttu-id="b1596-124">Binary</span><span class="sxs-lookup"><span data-stu-id="b1596-124">Binary</span></span>|<span data-ttu-id="b1596-125">文件的 Base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="b1596-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="b1596-126">contentId</span><span class="sxs-lookup"><span data-stu-id="b1596-126">contentId</span></span>|<span data-ttu-id="b1596-127">String</span><span class="sxs-lookup"><span data-stu-id="b1596-127">String</span></span>|<span data-ttu-id="b1596-128">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="b1596-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="b1596-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="b1596-129">contentLocation</span></span>|<span data-ttu-id="b1596-130">String</span><span class="sxs-lookup"><span data-stu-id="b1596-130">String</span></span>|<span data-ttu-id="b1596-131">请勿使用此属性，因为它不受支持。</span><span class="sxs-lookup"><span data-stu-id="b1596-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="b1596-132">contentType</span><span class="sxs-lookup"><span data-stu-id="b1596-132">contentType</span></span>|<span data-ttu-id="b1596-133">String</span><span class="sxs-lookup"><span data-stu-id="b1596-133">String</span></span>|<span data-ttu-id="b1596-134">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="b1596-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="b1596-135">id</span><span class="sxs-lookup"><span data-stu-id="b1596-135">id</span></span>|<span data-ttu-id="b1596-136">String</span><span class="sxs-lookup"><span data-stu-id="b1596-136">String</span></span>|<span data-ttu-id="b1596-137">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="b1596-137">The attachment ID.</span></span>|
|<span data-ttu-id="b1596-138">isInline</span><span class="sxs-lookup"><span data-stu-id="b1596-138">isInline</span></span>|<span data-ttu-id="b1596-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1596-139">Boolean</span></span>|<span data-ttu-id="b1596-140">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="b1596-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="b1596-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1596-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b1596-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1596-142">DateTimeOffset</span></span>|<span data-ttu-id="b1596-143">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b1596-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="b1596-144">name</span><span class="sxs-lookup"><span data-stu-id="b1596-144">name</span></span>|<span data-ttu-id="b1596-145">String</span><span class="sxs-lookup"><span data-stu-id="b1596-145">String</span></span>|<span data-ttu-id="b1596-146">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="b1596-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="b1596-147">size</span><span class="sxs-lookup"><span data-stu-id="b1596-147">size</span></span>|<span data-ttu-id="b1596-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b1596-148">Int32</span></span>|<span data-ttu-id="b1596-149">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="b1596-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1596-150">关系</span><span class="sxs-lookup"><span data-stu-id="b1596-150">Relationships</span></span>
<span data-ttu-id="b1596-151">无</span><span class="sxs-lookup"><span data-stu-id="b1596-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1596-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1596-152">JSON representation</span></span>

<span data-ttu-id="b1596-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1596-153">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
