---
title: referenceAttachment 资源类型
description: 到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21f88a6b3e8374eda3af11ca7094539e66137148
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034788"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="2250f-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2250f-103">referenceAttachment resource type</span></span>

<span data-ttu-id="2250f-104">到 OneDrive for Business 云驱动器或其他支持的存储位置上的文件（例如文本文件或 Word 文档）的链接，附加到事件、邮件或帖子中。</span><span class="sxs-lookup"><span data-stu-id="2250f-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="2250f-105">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="2250f-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2250f-106">方法</span><span class="sxs-lookup"><span data-stu-id="2250f-106">Methods</span></span>

| <span data-ttu-id="2250f-107">方法</span><span class="sxs-lookup"><span data-stu-id="2250f-107">Method</span></span>       | <span data-ttu-id="2250f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2250f-108">Return Type</span></span>  |<span data-ttu-id="2250f-109">说明</span><span class="sxs-lookup"><span data-stu-id="2250f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2250f-110">Get</span><span class="sxs-lookup"><span data-stu-id="2250f-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="2250f-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="2250f-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="2250f-112">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2250f-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="2250f-113">删除</span><span class="sxs-lookup"><span data-stu-id="2250f-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="2250f-114">无</span><span class="sxs-lookup"><span data-stu-id="2250f-114">None</span></span> |<span data-ttu-id="2250f-115">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="2250f-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2250f-116">属性</span><span class="sxs-lookup"><span data-stu-id="2250f-116">Properties</span></span>
| <span data-ttu-id="2250f-117">属性</span><span class="sxs-lookup"><span data-stu-id="2250f-117">Property</span></span>     | <span data-ttu-id="2250f-118">类型</span><span class="sxs-lookup"><span data-stu-id="2250f-118">Type</span></span>   |<span data-ttu-id="2250f-119">说明</span><span class="sxs-lookup"><span data-stu-id="2250f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2250f-120">contentType</span><span class="sxs-lookup"><span data-stu-id="2250f-120">contentType</span></span>|<span data-ttu-id="2250f-121">String</span><span class="sxs-lookup"><span data-stu-id="2250f-121">String</span></span>|<span data-ttu-id="2250f-122">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="2250f-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="2250f-123">id</span><span class="sxs-lookup"><span data-stu-id="2250f-123">id</span></span>|<span data-ttu-id="2250f-124">String</span><span class="sxs-lookup"><span data-stu-id="2250f-124">String</span></span>|<span data-ttu-id="2250f-p101">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="2250f-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="2250f-127">isInline</span><span class="sxs-lookup"><span data-stu-id="2250f-127">isInline</span></span>|<span data-ttu-id="2250f-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="2250f-128">Boolean</span></span>|<span data-ttu-id="2250f-129">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="2250f-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="2250f-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2250f-130">lastModifiedDateTime</span></span>|<span data-ttu-id="2250f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2250f-131">DateTimeOffset</span></span>|<span data-ttu-id="2250f-p102">上次修改附件的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2250f-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2250f-135">name</span><span class="sxs-lookup"><span data-stu-id="2250f-135">name</span></span>|<span data-ttu-id="2250f-136">字符串</span><span class="sxs-lookup"><span data-stu-id="2250f-136">String</span></span>|<span data-ttu-id="2250f-p103">显示在用于表示嵌入附件的图标下方的文本。这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="2250f-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="2250f-139">size</span><span class="sxs-lookup"><span data-stu-id="2250f-139">size</span></span>|<span data-ttu-id="2250f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2250f-140">Int32</span></span>|<span data-ttu-id="2250f-141">存储在邮件附件中的元数据大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="2250f-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="2250f-142">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="2250f-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2250f-143">关系</span><span class="sxs-lookup"><span data-stu-id="2250f-143">Relationships</span></span>
<span data-ttu-id="2250f-144">无</span><span class="sxs-lookup"><span data-stu-id="2250f-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="2250f-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2250f-145">JSON representation</span></span>

<span data-ttu-id="2250f-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2250f-146">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
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
