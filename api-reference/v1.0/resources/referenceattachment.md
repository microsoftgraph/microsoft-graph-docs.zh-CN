---
title: referenceAttachment 资源类型
description: 到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。
localization_priority: Normal
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: ae16b7df05a6a240b0081e189d74b4622f2f7988
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129338"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="ba98d-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba98d-103">referenceAttachment resource type</span></span>

<span data-ttu-id="ba98d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba98d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba98d-105">到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。</span><span class="sxs-lookup"><span data-stu-id="ba98d-105">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="ba98d-106">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="ba98d-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ba98d-107">方法</span><span class="sxs-lookup"><span data-stu-id="ba98d-107">Methods</span></span>

| <span data-ttu-id="ba98d-108">方法</span><span class="sxs-lookup"><span data-stu-id="ba98d-108">Method</span></span>       | <span data-ttu-id="ba98d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba98d-109">Return Type</span></span>  |<span data-ttu-id="ba98d-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba98d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba98d-111">获取</span><span class="sxs-lookup"><span data-stu-id="ba98d-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ba98d-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="ba98d-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="ba98d-113">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba98d-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="ba98d-114">删除</span><span class="sxs-lookup"><span data-stu-id="ba98d-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ba98d-115">无</span><span class="sxs-lookup"><span data-stu-id="ba98d-115">None</span></span> |<span data-ttu-id="ba98d-116">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="ba98d-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ba98d-117">属性</span><span class="sxs-lookup"><span data-stu-id="ba98d-117">Properties</span></span>
| <span data-ttu-id="ba98d-118">属性</span><span class="sxs-lookup"><span data-stu-id="ba98d-118">Property</span></span>     | <span data-ttu-id="ba98d-119">类型</span><span class="sxs-lookup"><span data-stu-id="ba98d-119">Type</span></span>   |<span data-ttu-id="ba98d-120">说明</span><span class="sxs-lookup"><span data-stu-id="ba98d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba98d-121">contentType</span><span class="sxs-lookup"><span data-stu-id="ba98d-121">contentType</span></span>|<span data-ttu-id="ba98d-122">String</span><span class="sxs-lookup"><span data-stu-id="ba98d-122">String</span></span>|<span data-ttu-id="ba98d-123">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="ba98d-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="ba98d-124">id</span><span class="sxs-lookup"><span data-stu-id="ba98d-124">id</span></span>|<span data-ttu-id="ba98d-125">String</span><span class="sxs-lookup"><span data-stu-id="ba98d-125">String</span></span>|<span data-ttu-id="ba98d-p101">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="ba98d-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="ba98d-128">isInline</span><span class="sxs-lookup"><span data-stu-id="ba98d-128">isInline</span></span>|<span data-ttu-id="ba98d-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba98d-129">Boolean</span></span>|<span data-ttu-id="ba98d-130">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="ba98d-130">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="ba98d-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba98d-131">lastModifiedDateTime</span></span>|<span data-ttu-id="ba98d-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba98d-132">DateTimeOffset</span></span>|<span data-ttu-id="ba98d-p102">上次修改附件的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ba98d-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ba98d-136">name</span><span class="sxs-lookup"><span data-stu-id="ba98d-136">name</span></span>|<span data-ttu-id="ba98d-137">String</span><span class="sxs-lookup"><span data-stu-id="ba98d-137">String</span></span>|<span data-ttu-id="ba98d-p103">显示在用于表示嵌入附件的图标下方的文本。这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="ba98d-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="ba98d-140">大小</span><span class="sxs-lookup"><span data-stu-id="ba98d-140">size</span></span>|<span data-ttu-id="ba98d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ba98d-141">Int32</span></span>|<span data-ttu-id="ba98d-142">存储在邮件附件中的元数据大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="ba98d-142">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="ba98d-143">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="ba98d-143">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba98d-144">关系</span><span class="sxs-lookup"><span data-stu-id="ba98d-144">Relationships</span></span>
<span data-ttu-id="ba98d-145">无</span><span class="sxs-lookup"><span data-stu-id="ba98d-145">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="ba98d-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba98d-146">JSON representation</span></span>

<span data-ttu-id="ba98d-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba98d-147">Here is a JSON representation of the resource</span></span>

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

