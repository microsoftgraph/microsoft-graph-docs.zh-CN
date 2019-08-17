---
title: fileAttachment 资源类型
description: 附加到事件的文件 (如文本文件或 Word 文档)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 7161d8bf17aa573cad61123200785ff254c24feb
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453153"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="5525f-103">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5525f-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5525f-104">附加到[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[公告](../resources/post.md)的文件 (如文本文件或 Word 文档)。</span><span class="sxs-lookup"><span data-stu-id="5525f-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="5525f-105">**ContentBytes**属性包含文件的 base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="5525f-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="5525f-106">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="5525f-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="5525f-107">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="5525f-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="5525f-108">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="5525f-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5525f-109">方法</span><span class="sxs-lookup"><span data-stu-id="5525f-109">Methods</span></span>

| <span data-ttu-id="5525f-110">方法</span><span class="sxs-lookup"><span data-stu-id="5525f-110">Method</span></span>       | <span data-ttu-id="5525f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5525f-111">Return Type</span></span>  |<span data-ttu-id="5525f-112">说明</span><span class="sxs-lookup"><span data-stu-id="5525f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5525f-113">Get</span><span class="sxs-lookup"><span data-stu-id="5525f-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="5525f-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="5525f-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="5525f-115">读取 fileattachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5525f-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="5525f-116">删除</span><span class="sxs-lookup"><span data-stu-id="5525f-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="5525f-117">无</span><span class="sxs-lookup"><span data-stu-id="5525f-117">None</span></span> |<span data-ttu-id="5525f-118">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="5525f-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5525f-119">属性</span><span class="sxs-lookup"><span data-stu-id="5525f-119">Properties</span></span>
| <span data-ttu-id="5525f-120">属性</span><span class="sxs-lookup"><span data-stu-id="5525f-120">Property</span></span>     | <span data-ttu-id="5525f-121">类型</span><span class="sxs-lookup"><span data-stu-id="5525f-121">Type</span></span>   |<span data-ttu-id="5525f-122">说明</span><span class="sxs-lookup"><span data-stu-id="5525f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5525f-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="5525f-123">contentBytes</span></span>|<span data-ttu-id="5525f-124">Edm</span><span class="sxs-lookup"><span data-stu-id="5525f-124">Edm.Binary</span></span>|<span data-ttu-id="5525f-125">文件的 Base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="5525f-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="5525f-126">contentId</span><span class="sxs-lookup"><span data-stu-id="5525f-126">contentId</span></span>|<span data-ttu-id="5525f-127">String</span><span class="sxs-lookup"><span data-stu-id="5525f-127">String</span></span>|<span data-ttu-id="5525f-128">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="5525f-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="5525f-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="5525f-129">contentLocation</span></span>|<span data-ttu-id="5525f-130">String</span><span class="sxs-lookup"><span data-stu-id="5525f-130">String</span></span>|<span data-ttu-id="5525f-131">请勿使用此属性，因为它不受支持。</span><span class="sxs-lookup"><span data-stu-id="5525f-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="5525f-132">contentType</span><span class="sxs-lookup"><span data-stu-id="5525f-132">contentType</span></span>|<span data-ttu-id="5525f-133">String</span><span class="sxs-lookup"><span data-stu-id="5525f-133">String</span></span>|<span data-ttu-id="5525f-134">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="5525f-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="5525f-135">id</span><span class="sxs-lookup"><span data-stu-id="5525f-135">id</span></span>|<span data-ttu-id="5525f-136">String</span><span class="sxs-lookup"><span data-stu-id="5525f-136">String</span></span>|<span data-ttu-id="5525f-137">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="5525f-137">The attachment ID.</span></span>|
|<span data-ttu-id="5525f-138">isInline</span><span class="sxs-lookup"><span data-stu-id="5525f-138">isInline</span></span>|<span data-ttu-id="5525f-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="5525f-139">Boolean</span></span>|<span data-ttu-id="5525f-140">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5525f-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="5525f-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5525f-141">lastModifiedDateTime</span></span>|<span data-ttu-id="5525f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5525f-142">DateTimeOffset</span></span>|<span data-ttu-id="5525f-143">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5525f-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="5525f-144">name</span><span class="sxs-lookup"><span data-stu-id="5525f-144">name</span></span>|<span data-ttu-id="5525f-145">String</span><span class="sxs-lookup"><span data-stu-id="5525f-145">String</span></span>|<span data-ttu-id="5525f-146">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="5525f-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="5525f-147">size</span><span class="sxs-lookup"><span data-stu-id="5525f-147">size</span></span>|<span data-ttu-id="5525f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5525f-148">Int32</span></span>|<span data-ttu-id="5525f-149">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="5525f-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5525f-150">关系</span><span class="sxs-lookup"><span data-stu-id="5525f-150">Relationships</span></span>
<span data-ttu-id="5525f-151">无</span><span class="sxs-lookup"><span data-stu-id="5525f-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5525f-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5525f-152">JSON representation</span></span>

<span data-ttu-id="5525f-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5525f-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "string (binary)",
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
