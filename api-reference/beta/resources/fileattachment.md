---
title: fileAttachment 资源类型
description: 附加到事件，文件 （如文本文件或 Word 文档中）
localization_priority: Normal
ms.openlocfilehash: 7032bcd234d07f0f3fdce0787968d72530a0a442
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510762"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="0e573-103">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e573-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e573-104">附加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)（如文本文件或 Word 文档） 的文件。</span><span class="sxs-lookup"><span data-stu-id="0e573-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="0e573-105">**ContentBytes**属性将包含 base64 编码的文件的内容。</span><span class="sxs-lookup"><span data-stu-id="0e573-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="0e573-106">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="0e573-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="0e573-107">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="0e573-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="0e573-108">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="0e573-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0e573-109">方法</span><span class="sxs-lookup"><span data-stu-id="0e573-109">Methods</span></span>

| <span data-ttu-id="0e573-110">方法</span><span class="sxs-lookup"><span data-stu-id="0e573-110">Method</span></span>       | <span data-ttu-id="0e573-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e573-111">Return Type</span></span>  |<span data-ttu-id="0e573-112">说明</span><span class="sxs-lookup"><span data-stu-id="0e573-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e573-113">Get</span><span class="sxs-lookup"><span data-stu-id="0e573-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="0e573-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="0e573-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="0e573-115">读取 fileattachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e573-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="0e573-116">删除</span><span class="sxs-lookup"><span data-stu-id="0e573-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="0e573-117">无</span><span class="sxs-lookup"><span data-stu-id="0e573-117">None</span></span> |<span data-ttu-id="0e573-118">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="0e573-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e573-119">属性</span><span class="sxs-lookup"><span data-stu-id="0e573-119">Properties</span></span>
| <span data-ttu-id="0e573-120">属性</span><span class="sxs-lookup"><span data-stu-id="0e573-120">Property</span></span>     | <span data-ttu-id="0e573-121">类型</span><span class="sxs-lookup"><span data-stu-id="0e573-121">Type</span></span>   |<span data-ttu-id="0e573-122">说明</span><span class="sxs-lookup"><span data-stu-id="0e573-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e573-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="0e573-123">contentBytes</span></span>|<span data-ttu-id="0e573-124">Binary</span><span class="sxs-lookup"><span data-stu-id="0e573-124">Binary</span></span>|<span data-ttu-id="0e573-125">文件的 Base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="0e573-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="0e573-126">contentId</span><span class="sxs-lookup"><span data-stu-id="0e573-126">contentId</span></span>|<span data-ttu-id="0e573-127">String</span><span class="sxs-lookup"><span data-stu-id="0e573-127">String</span></span>|<span data-ttu-id="0e573-128">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="0e573-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="0e573-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="0e573-129">contentLocation</span></span>|<span data-ttu-id="0e573-130">String</span><span class="sxs-lookup"><span data-stu-id="0e573-130">String</span></span>|<span data-ttu-id="0e573-131">对应于附件内容所在位置的统一资源标识符 (URI)。</span><span class="sxs-lookup"><span data-stu-id="0e573-131">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="0e573-132">contentType</span><span class="sxs-lookup"><span data-stu-id="0e573-132">contentType</span></span>|<span data-ttu-id="0e573-133">String</span><span class="sxs-lookup"><span data-stu-id="0e573-133">String</span></span>|<span data-ttu-id="0e573-134">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="0e573-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="0e573-135">id</span><span class="sxs-lookup"><span data-stu-id="0e573-135">id</span></span>|<span data-ttu-id="0e573-136">字串符号</span><span class="sxs-lookup"><span data-stu-id="0e573-136">String</span></span>|<span data-ttu-id="0e573-137">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="0e573-137">The attachment ID.</span></span>|
|<span data-ttu-id="0e573-138">isInline</span><span class="sxs-lookup"><span data-stu-id="0e573-138">isInline</span></span>|<span data-ttu-id="0e573-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e573-139">Boolean</span></span>|<span data-ttu-id="0e573-140">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="0e573-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="0e573-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e573-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0e573-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e573-142">DateTimeOffset</span></span>|<span data-ttu-id="0e573-143">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0e573-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="0e573-144">name</span><span class="sxs-lookup"><span data-stu-id="0e573-144">name</span></span>|<span data-ttu-id="0e573-145">String</span><span class="sxs-lookup"><span data-stu-id="0e573-145">String</span></span>|<span data-ttu-id="0e573-146">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="0e573-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="0e573-147">size</span><span class="sxs-lookup"><span data-stu-id="0e573-147">size</span></span>|<span data-ttu-id="0e573-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0e573-148">Int32</span></span>|<span data-ttu-id="0e573-149">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="0e573-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e573-150">关系</span><span class="sxs-lookup"><span data-stu-id="0e573-150">Relationships</span></span>
<span data-ttu-id="0e573-151">无</span><span class="sxs-lookup"><span data-stu-id="0e573-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0e573-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e573-152">JSON representation</span></span>

<span data-ttu-id="0e573-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e573-153">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/fileattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
