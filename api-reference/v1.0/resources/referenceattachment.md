---
title: referenceAttachment 资源类型
description: 到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。
localization_priority: Normal
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: 8a9b4d43a7bbc31c737c85ea1a18bd14beefcb05
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722410"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="73fe9-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="73fe9-103">referenceAttachment resource type</span></span>

<span data-ttu-id="73fe9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73fe9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73fe9-105">到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。</span><span class="sxs-lookup"><span data-stu-id="73fe9-105">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="73fe9-106">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="73fe9-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="73fe9-107">方法</span><span class="sxs-lookup"><span data-stu-id="73fe9-107">Methods</span></span>

| <span data-ttu-id="73fe9-108">方法</span><span class="sxs-lookup"><span data-stu-id="73fe9-108">Method</span></span>       | <span data-ttu-id="73fe9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="73fe9-109">Return Type</span></span>  |<span data-ttu-id="73fe9-110">说明</span><span class="sxs-lookup"><span data-stu-id="73fe9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73fe9-111">获取</span><span class="sxs-lookup"><span data-stu-id="73fe9-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="73fe9-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="73fe9-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="73fe9-113">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73fe9-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="73fe9-114">删除</span><span class="sxs-lookup"><span data-stu-id="73fe9-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="73fe9-115">无</span><span class="sxs-lookup"><span data-stu-id="73fe9-115">None</span></span> |<span data-ttu-id="73fe9-116">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="73fe9-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="73fe9-117">属性</span><span class="sxs-lookup"><span data-stu-id="73fe9-117">Properties</span></span>
| <span data-ttu-id="73fe9-118">属性</span><span class="sxs-lookup"><span data-stu-id="73fe9-118">Property</span></span>     | <span data-ttu-id="73fe9-119">类型</span><span class="sxs-lookup"><span data-stu-id="73fe9-119">Type</span></span>   |<span data-ttu-id="73fe9-120">说明</span><span class="sxs-lookup"><span data-stu-id="73fe9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73fe9-121">contentType</span><span class="sxs-lookup"><span data-stu-id="73fe9-121">contentType</span></span>|<span data-ttu-id="73fe9-122">String</span><span class="sxs-lookup"><span data-stu-id="73fe9-122">String</span></span>|<span data-ttu-id="73fe9-123">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="73fe9-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="73fe9-124">id</span><span class="sxs-lookup"><span data-stu-id="73fe9-124">id</span></span>|<span data-ttu-id="73fe9-125">字符串</span><span class="sxs-lookup"><span data-stu-id="73fe9-125">String</span></span>|<span data-ttu-id="73fe9-p101">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="73fe9-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="73fe9-128">isInline</span><span class="sxs-lookup"><span data-stu-id="73fe9-128">isInline</span></span>|<span data-ttu-id="73fe9-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="73fe9-129">Boolean</span></span>|<span data-ttu-id="73fe9-130">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="73fe9-130">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="73fe9-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73fe9-131">lastModifiedDateTime</span></span>|<span data-ttu-id="73fe9-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73fe9-132">DateTimeOffset</span></span>|<span data-ttu-id="73fe9-133">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73fe9-133">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="73fe9-134">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="73fe9-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73fe9-135">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="73fe9-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="73fe9-136">name</span><span class="sxs-lookup"><span data-stu-id="73fe9-136">name</span></span>|<span data-ttu-id="73fe9-137">字符串</span><span class="sxs-lookup"><span data-stu-id="73fe9-137">String</span></span>|<span data-ttu-id="73fe9-p103">显示在用于表示嵌入附件的图标下方的文本。这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="73fe9-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="73fe9-140">size</span><span class="sxs-lookup"><span data-stu-id="73fe9-140">size</span></span>|<span data-ttu-id="73fe9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="73fe9-141">Int32</span></span>|<span data-ttu-id="73fe9-142">存储在邮件附件中的元数据大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="73fe9-142">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="73fe9-143">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="73fe9-143">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73fe9-144">关系</span><span class="sxs-lookup"><span data-stu-id="73fe9-144">Relationships</span></span>
<span data-ttu-id="73fe9-145">无</span><span class="sxs-lookup"><span data-stu-id="73fe9-145">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="73fe9-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73fe9-146">JSON representation</span></span>

<span data-ttu-id="73fe9-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73fe9-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.referenceAttachment"
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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

