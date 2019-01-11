---
title: itemAttachment 资源类型
description: '附加到另一个事件、邮件或帖子的联系人、事件或邮件。  '
localization_priority: Priority
ms.openlocfilehash: df996175e545b78f4ca9a1b6271b9cb012ffffce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853520"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="ceb92-103">itemAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="ceb92-103">itemAttachment resource type</span></span>

<span data-ttu-id="ceb92-104">附加到另一个事件、邮件或帖子的联系人、事件或邮件。</span><span class="sxs-lookup"><span data-stu-id="ceb92-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="ceb92-105">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="ceb92-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ceb92-106">方法</span><span class="sxs-lookup"><span data-stu-id="ceb92-106">Methods</span></span>

| <span data-ttu-id="ceb92-107">方法</span><span class="sxs-lookup"><span data-stu-id="ceb92-107">Method</span></span>       | <span data-ttu-id="ceb92-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ceb92-108">Return Type</span></span>  |<span data-ttu-id="ceb92-109">说明</span><span class="sxs-lookup"><span data-stu-id="ceb92-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ceb92-110">Get</span><span class="sxs-lookup"><span data-stu-id="ceb92-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ceb92-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="ceb92-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="ceb92-112">读取 itemAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ceb92-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="ceb92-113">删除</span><span class="sxs-lookup"><span data-stu-id="ceb92-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ceb92-114">无</span><span class="sxs-lookup"><span data-stu-id="ceb92-114">None</span></span> |<span data-ttu-id="ceb92-115">删除 itemAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="ceb92-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ceb92-116">属性</span><span class="sxs-lookup"><span data-stu-id="ceb92-116">Properties</span></span>
| <span data-ttu-id="ceb92-117">属性</span><span class="sxs-lookup"><span data-stu-id="ceb92-117">Property</span></span>     | <span data-ttu-id="ceb92-118">类型</span><span class="sxs-lookup"><span data-stu-id="ceb92-118">Type</span></span>   |<span data-ttu-id="ceb92-119">说明</span><span class="sxs-lookup"><span data-stu-id="ceb92-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ceb92-120">contentType</span><span class="sxs-lookup"><span data-stu-id="ceb92-120">contentType</span></span>|<span data-ttu-id="ceb92-121">String</span><span class="sxs-lookup"><span data-stu-id="ceb92-121">String</span></span>|<span data-ttu-id="ceb92-122">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="ceb92-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="ceb92-123">id</span><span class="sxs-lookup"><span data-stu-id="ceb92-123">id</span></span>|<span data-ttu-id="ceb92-124">String</span><span class="sxs-lookup"><span data-stu-id="ceb92-124">String</span></span>| <span data-ttu-id="ceb92-125">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="ceb92-125">The attachment ID.</span></span>|
|<span data-ttu-id="ceb92-126">isInline</span><span class="sxs-lookup"><span data-stu-id="ceb92-126">isInline</span></span>|<span data-ttu-id="ceb92-127">布尔</span><span class="sxs-lookup"><span data-stu-id="ceb92-127">Boolean</span></span>|<span data-ttu-id="ceb92-128">如果附件是内联的（例如嵌入到项目正文中的图像），请设置为 true。</span><span class="sxs-lookup"><span data-stu-id="ceb92-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="ceb92-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ceb92-129">lastModifiedDateTime</span></span>|<span data-ttu-id="ceb92-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceb92-130">DateTimeOffset</span></span>|<span data-ttu-id="ceb92-131">上次修改附件的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="ceb92-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="ceb92-132">name</span><span class="sxs-lookup"><span data-stu-id="ceb92-132">name</span></span>|<span data-ttu-id="ceb92-133">String</span><span class="sxs-lookup"><span data-stu-id="ceb92-133">String</span></span>|<span data-ttu-id="ceb92-134">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ceb92-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="ceb92-135">大小</span><span class="sxs-lookup"><span data-stu-id="ceb92-135">size</span></span>|<span data-ttu-id="ceb92-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ceb92-136">Int32</span></span>|<span data-ttu-id="ceb92-137">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="ceb92-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceb92-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="ceb92-138">Relationships</span></span>
| <span data-ttu-id="ceb92-139">关系</span><span class="sxs-lookup"><span data-stu-id="ceb92-139">Relationship</span></span> | <span data-ttu-id="ceb92-140">类型</span><span class="sxs-lookup"><span data-stu-id="ceb92-140">Type</span></span>   |<span data-ttu-id="ceb92-141">说明</span><span class="sxs-lookup"><span data-stu-id="ceb92-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ceb92-142">项</span><span class="sxs-lookup"><span data-stu-id="ceb92-142">item</span></span>|[<span data-ttu-id="ceb92-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="ceb92-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="ceb92-p101">附加的消息或事件。导航属性。</span><span class="sxs-lookup"><span data-stu-id="ceb92-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ceb92-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ceb92-146">JSON representation</span></span>

<span data-ttu-id="ceb92-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ceb92-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
