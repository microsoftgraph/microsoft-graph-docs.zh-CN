---
title: fileAttachment 资源类型
description: '附加到事件、邮件或帖子的文件（如文本文件或 Word 文档）。**contentBytes** '
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 90fd8d838a15ab087cae5d2ea5e24835779385cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459712"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="12a5e-104">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="12a5e-104">fileAttachment resource type</span></span>

<span data-ttu-id="12a5e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a5e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12a5e-106">用户[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)中附加的文件（例如文本文件或 Word 文档）。</span><span class="sxs-lookup"><span data-stu-id="12a5e-106">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="12a5e-107">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="12a5e-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="12a5e-108">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="12a5e-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="12a5e-109">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="12a5e-109">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="12a5e-110">确保先使用 base64 为文件内容编码，然后再将其分配到 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="12a5e-110">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="12a5e-111">方法</span><span class="sxs-lookup"><span data-stu-id="12a5e-111">Methods</span></span>

| <span data-ttu-id="12a5e-112">方法</span><span class="sxs-lookup"><span data-stu-id="12a5e-112">Method</span></span>       | <span data-ttu-id="12a5e-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="12a5e-113">Return Type</span></span>  |<span data-ttu-id="12a5e-114">说明</span><span class="sxs-lookup"><span data-stu-id="12a5e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12a5e-115">Get</span><span class="sxs-lookup"><span data-stu-id="12a5e-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="12a5e-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="12a5e-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="12a5e-117">读取 fileAttachment 对象的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="12a5e-117">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="12a5e-118">Delete</span><span class="sxs-lookup"><span data-stu-id="12a5e-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="12a5e-119">无</span><span class="sxs-lookup"><span data-stu-id="12a5e-119">None</span></span> |<span data-ttu-id="12a5e-120">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="12a5e-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="12a5e-121">属性</span><span class="sxs-lookup"><span data-stu-id="12a5e-121">Properties</span></span>
| <span data-ttu-id="12a5e-122">属性</span><span class="sxs-lookup"><span data-stu-id="12a5e-122">Property</span></span>     | <span data-ttu-id="12a5e-123">类型</span><span class="sxs-lookup"><span data-stu-id="12a5e-123">Type</span></span>   |<span data-ttu-id="12a5e-124">说明</span><span class="sxs-lookup"><span data-stu-id="12a5e-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12a5e-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="12a5e-125">contentBytes</span></span>|<span data-ttu-id="12a5e-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="12a5e-126">Edm.Binary</span></span>|<span data-ttu-id="12a5e-127">文件的 Base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="12a5e-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="12a5e-128">contentId</span><span class="sxs-lookup"><span data-stu-id="12a5e-128">contentId</span></span>|<span data-ttu-id="12a5e-129">String</span><span class="sxs-lookup"><span data-stu-id="12a5e-129">String</span></span>|<span data-ttu-id="12a5e-130">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="12a5e-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="12a5e-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="12a5e-131">contentLocation</span></span>|<span data-ttu-id="12a5e-132">String</span><span class="sxs-lookup"><span data-stu-id="12a5e-132">String</span></span>|<span data-ttu-id="12a5e-133">请勿使用此属性，因为它不受支持。</span><span class="sxs-lookup"><span data-stu-id="12a5e-133">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="12a5e-134">contentType</span><span class="sxs-lookup"><span data-stu-id="12a5e-134">contentType</span></span>|<span data-ttu-id="12a5e-135">String</span><span class="sxs-lookup"><span data-stu-id="12a5e-135">String</span></span>|<span data-ttu-id="12a5e-136">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="12a5e-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="12a5e-137">id</span><span class="sxs-lookup"><span data-stu-id="12a5e-137">id</span></span>|<span data-ttu-id="12a5e-138">String</span><span class="sxs-lookup"><span data-stu-id="12a5e-138">String</span></span>|<span data-ttu-id="12a5e-139">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="12a5e-139">The attachment ID.</span></span>|
|<span data-ttu-id="12a5e-140">isInline</span><span class="sxs-lookup"><span data-stu-id="12a5e-140">isInline</span></span>|<span data-ttu-id="12a5e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="12a5e-141">Boolean</span></span>|<span data-ttu-id="12a5e-142">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="12a5e-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="12a5e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12a5e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="12a5e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12a5e-144">DateTimeOffset</span></span>|<span data-ttu-id="12a5e-145">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12a5e-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="12a5e-146">name</span><span class="sxs-lookup"><span data-stu-id="12a5e-146">name</span></span>|<span data-ttu-id="12a5e-147">String</span><span class="sxs-lookup"><span data-stu-id="12a5e-147">String</span></span>|<span data-ttu-id="12a5e-148">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="12a5e-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="12a5e-149">size</span><span class="sxs-lookup"><span data-stu-id="12a5e-149">size</span></span>|<span data-ttu-id="12a5e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="12a5e-150">Int32</span></span>|<span data-ttu-id="12a5e-151">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="12a5e-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12a5e-152">关系</span><span class="sxs-lookup"><span data-stu-id="12a5e-152">Relationships</span></span>
<span data-ttu-id="12a5e-153">无</span><span class="sxs-lookup"><span data-stu-id="12a5e-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="12a5e-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12a5e-154">JSON representation</span></span>

<span data-ttu-id="12a5e-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12a5e-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty": "id",
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
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
