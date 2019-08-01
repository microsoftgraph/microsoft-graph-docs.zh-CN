---
title: fileAttachment 资源类型
description: '附加到事件、邮件或帖子的文件（如文本文件或 Word 文档）。**contentBytes** '
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7e80a4599d79d17829f2bb07bb61d4adf60df607
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032506"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="6c463-104">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c463-104">fileAttachment resource type</span></span>

<span data-ttu-id="6c463-p102">事件、邮件或帖子中附加的文件（例如文本文件或 Word 文档）。**contentBytes** 属性包含文件的 base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="6c463-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="6c463-107">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="6c463-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="6c463-108">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="6c463-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="6c463-109">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="6c463-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6c463-110">方法</span><span class="sxs-lookup"><span data-stu-id="6c463-110">Methods</span></span>

| <span data-ttu-id="6c463-111">方法</span><span class="sxs-lookup"><span data-stu-id="6c463-111">Method</span></span>       | <span data-ttu-id="6c463-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c463-112">Return Type</span></span>  |<span data-ttu-id="6c463-113">说明</span><span class="sxs-lookup"><span data-stu-id="6c463-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c463-114">Get</span><span class="sxs-lookup"><span data-stu-id="6c463-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="6c463-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="6c463-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="6c463-116">读取 fileattachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c463-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="6c463-117">删除</span><span class="sxs-lookup"><span data-stu-id="6c463-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="6c463-118">无</span><span class="sxs-lookup"><span data-stu-id="6c463-118">None</span></span> |<span data-ttu-id="6c463-119">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="6c463-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6c463-120">属性</span><span class="sxs-lookup"><span data-stu-id="6c463-120">Properties</span></span>
| <span data-ttu-id="6c463-121">属性</span><span class="sxs-lookup"><span data-stu-id="6c463-121">Property</span></span>     | <span data-ttu-id="6c463-122">类型</span><span class="sxs-lookup"><span data-stu-id="6c463-122">Type</span></span>   |<span data-ttu-id="6c463-123">说明</span><span class="sxs-lookup"><span data-stu-id="6c463-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c463-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="6c463-124">contentBytes</span></span>|<span data-ttu-id="6c463-125">Binary</span><span class="sxs-lookup"><span data-stu-id="6c463-125">Binary</span></span>|<span data-ttu-id="6c463-126">文件的 Base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="6c463-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="6c463-127">contentId</span><span class="sxs-lookup"><span data-stu-id="6c463-127">contentId</span></span>|<span data-ttu-id="6c463-128">String</span><span class="sxs-lookup"><span data-stu-id="6c463-128">String</span></span>|<span data-ttu-id="6c463-129">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="6c463-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="6c463-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="6c463-130">contentLocation</span></span>|<span data-ttu-id="6c463-131">String</span><span class="sxs-lookup"><span data-stu-id="6c463-131">String</span></span>|<span data-ttu-id="6c463-132">请勿使用此属性，因为它不受支持。</span><span class="sxs-lookup"><span data-stu-id="6c463-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="6c463-133">contentType</span><span class="sxs-lookup"><span data-stu-id="6c463-133">contentType</span></span>|<span data-ttu-id="6c463-134">String</span><span class="sxs-lookup"><span data-stu-id="6c463-134">String</span></span>|<span data-ttu-id="6c463-135">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="6c463-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="6c463-136">id</span><span class="sxs-lookup"><span data-stu-id="6c463-136">id</span></span>|<span data-ttu-id="6c463-137">String</span><span class="sxs-lookup"><span data-stu-id="6c463-137">String</span></span>|<span data-ttu-id="6c463-138">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="6c463-138">The attachment ID.</span></span>|
|<span data-ttu-id="6c463-139">isInline</span><span class="sxs-lookup"><span data-stu-id="6c463-139">isInline</span></span>|<span data-ttu-id="6c463-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c463-140">Boolean</span></span>|<span data-ttu-id="6c463-141">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="6c463-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="6c463-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c463-142">lastModifiedDateTime</span></span>|<span data-ttu-id="6c463-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c463-143">DateTimeOffset</span></span>|<span data-ttu-id="6c463-144">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6c463-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="6c463-145">name</span><span class="sxs-lookup"><span data-stu-id="6c463-145">name</span></span>|<span data-ttu-id="6c463-146">String</span><span class="sxs-lookup"><span data-stu-id="6c463-146">String</span></span>|<span data-ttu-id="6c463-147">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="6c463-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="6c463-148">size</span><span class="sxs-lookup"><span data-stu-id="6c463-148">size</span></span>|<span data-ttu-id="6c463-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6c463-149">Int32</span></span>|<span data-ttu-id="6c463-150">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="6c463-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c463-151">关系</span><span class="sxs-lookup"><span data-stu-id="6c463-151">Relationships</span></span>
<span data-ttu-id="6c463-152">无</span><span class="sxs-lookup"><span data-stu-id="6c463-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6c463-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c463-153">JSON representation</span></span>

<span data-ttu-id="6c463-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c463-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
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
