---
title: fileAttachment 资源类型
description: 不 (例如文本文件或 Word) 文档）的文件，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 770cb2750df46243d6050832feeca301549b2c76
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849483"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="c6d99-103">fileAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6d99-103">fileAttachment resource type</span></span>

<span data-ttu-id="c6d99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6d99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="c6d99-105">用于将 (文档或 Word 文档等) 文件) 用户事件、[邮件](../resources/event.md)[、Outlook](../resources/message.md)[任务](../resources/outlooktask.md)或帖[子中](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="c6d99-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="c6d99-106">创建文件附件时，在请求正文中包括以下内容：</span><span class="sxs-lookup"><span data-stu-id="c6d99-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="c6d99-107">必要属性**名称**和 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="c6d99-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="c6d99-108">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="c6d99-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="c6d99-109">确保先使用 base64 为文件内容编码，然后再将其分配到 **contentBytes**。</span><span class="sxs-lookup"><span data-stu-id="c6d99-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="c6d99-110">方法</span><span class="sxs-lookup"><span data-stu-id="c6d99-110">Methods</span></span>

| <span data-ttu-id="c6d99-111">方法</span><span class="sxs-lookup"><span data-stu-id="c6d99-111">Method</span></span>       | <span data-ttu-id="c6d99-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6d99-112">Return Type</span></span>  |<span data-ttu-id="c6d99-113">说明</span><span class="sxs-lookup"><span data-stu-id="c6d99-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6d99-114">Get</span><span class="sxs-lookup"><span data-stu-id="c6d99-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="c6d99-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="c6d99-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="c6d99-116">读取 fileAttachment 对象的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="c6d99-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="c6d99-117">删除</span><span class="sxs-lookup"><span data-stu-id="c6d99-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="c6d99-118">无</span><span class="sxs-lookup"><span data-stu-id="c6d99-118">None</span></span> |<span data-ttu-id="c6d99-119">删除 fileAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="c6d99-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6d99-120">属性</span><span class="sxs-lookup"><span data-stu-id="c6d99-120">Properties</span></span>
| <span data-ttu-id="c6d99-121">属性</span><span class="sxs-lookup"><span data-stu-id="c6d99-121">Property</span></span>     | <span data-ttu-id="c6d99-122">类型</span><span class="sxs-lookup"><span data-stu-id="c6d99-122">Type</span></span>   |<span data-ttu-id="c6d99-123">说明</span><span class="sxs-lookup"><span data-stu-id="c6d99-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6d99-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="c6d99-124">contentBytes</span></span>|<span data-ttu-id="c6d99-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="c6d99-125">Edm.Binary</span></span>|<span data-ttu-id="c6d99-126">文件的 Base64 编码内容。</span><span class="sxs-lookup"><span data-stu-id="c6d99-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="c6d99-127">contentId</span><span class="sxs-lookup"><span data-stu-id="c6d99-127">contentId</span></span>|<span data-ttu-id="c6d99-128">String</span><span class="sxs-lookup"><span data-stu-id="c6d99-128">String</span></span>|<span data-ttu-id="c6d99-129">获取 Exchange 存储中的附件 ID。</span><span class="sxs-lookup"><span data-stu-id="c6d99-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="c6d99-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="c6d99-130">contentLocation</span></span>|<span data-ttu-id="c6d99-131">String</span><span class="sxs-lookup"><span data-stu-id="c6d99-131">String</span></span>|<span data-ttu-id="c6d99-132">请勿使用此属性，因为它不受支持。</span><span class="sxs-lookup"><span data-stu-id="c6d99-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="c6d99-133">contentType</span><span class="sxs-lookup"><span data-stu-id="c6d99-133">contentType</span></span>|<span data-ttu-id="c6d99-134">String</span><span class="sxs-lookup"><span data-stu-id="c6d99-134">String</span></span>|<span data-ttu-id="c6d99-135">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="c6d99-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="c6d99-136">id</span><span class="sxs-lookup"><span data-stu-id="c6d99-136">id</span></span>|<span data-ttu-id="c6d99-137">String</span><span class="sxs-lookup"><span data-stu-id="c6d99-137">String</span></span>|<span data-ttu-id="c6d99-138">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="c6d99-138">The attachment ID.</span></span>|
|<span data-ttu-id="c6d99-139">isInline</span><span class="sxs-lookup"><span data-stu-id="c6d99-139">isInline</span></span>|<span data-ttu-id="c6d99-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d99-140">Boolean</span></span>|<span data-ttu-id="c6d99-141">如果是内嵌附件则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c6d99-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="c6d99-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6d99-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c6d99-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6d99-143">DateTimeOffset</span></span>|<span data-ttu-id="c6d99-144">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c6d99-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="c6d99-145">name</span><span class="sxs-lookup"><span data-stu-id="c6d99-145">name</span></span>|<span data-ttu-id="c6d99-146">String</span><span class="sxs-lookup"><span data-stu-id="c6d99-146">String</span></span>|<span data-ttu-id="c6d99-147">表示显示在表示嵌入的附件的图标下方的文本的名称。该名称不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="c6d99-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="c6d99-148">size</span><span class="sxs-lookup"><span data-stu-id="c6d99-148">size</span></span>|<span data-ttu-id="c6d99-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c6d99-149">Int32</span></span>|<span data-ttu-id="c6d99-150">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="c6d99-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6d99-151">关系</span><span class="sxs-lookup"><span data-stu-id="c6d99-151">Relationships</span></span>
<span data-ttu-id="c6d99-152">无</span><span class="sxs-lookup"><span data-stu-id="c6d99-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c6d99-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6d99-153">JSON representation</span></span>

<span data-ttu-id="c6d99-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6d99-154">Here is a JSON representation of the resource</span></span>

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
