---
title: itemAttachment 资源类型
description: '附加到另一事件、邮件或帖子的联系人、事件或邮件。  '
localization_priority: Priority
ms.prod: outlook
author: angelgolfer-ms
doc_type: resourcePageType
ms.openlocfilehash: 7df14ea5d6611cb3771aeb23250c1e65fb6e60a4
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484357"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="6a959-103">itemAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a959-103">itemAttachment resource type</span></span>

<span data-ttu-id="6a959-104">附加到另一个事件、邮件或帖子的联系人、事件或邮件。</span><span class="sxs-lookup"><span data-stu-id="6a959-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="6a959-105">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="6a959-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6a959-106">方法</span><span class="sxs-lookup"><span data-stu-id="6a959-106">Methods</span></span>

| <span data-ttu-id="6a959-107">方法</span><span class="sxs-lookup"><span data-stu-id="6a959-107">Method</span></span>       | <span data-ttu-id="6a959-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a959-108">Return Type</span></span>  |<span data-ttu-id="6a959-109">说明</span><span class="sxs-lookup"><span data-stu-id="6a959-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a959-110">Get</span><span class="sxs-lookup"><span data-stu-id="6a959-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="6a959-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="6a959-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="6a959-112">读取 itemAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a959-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="6a959-113">删除</span><span class="sxs-lookup"><span data-stu-id="6a959-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="6a959-114">无</span><span class="sxs-lookup"><span data-stu-id="6a959-114">None</span></span> |<span data-ttu-id="6a959-115">删除 itemAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="6a959-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a959-116">属性</span><span class="sxs-lookup"><span data-stu-id="6a959-116">Properties</span></span>
| <span data-ttu-id="6a959-117">属性</span><span class="sxs-lookup"><span data-stu-id="6a959-117">Property</span></span>     | <span data-ttu-id="6a959-118">类型</span><span class="sxs-lookup"><span data-stu-id="6a959-118">Type</span></span>   |<span data-ttu-id="6a959-119">说明</span><span class="sxs-lookup"><span data-stu-id="6a959-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a959-120">contentType</span><span class="sxs-lookup"><span data-stu-id="6a959-120">contentType</span></span>|<span data-ttu-id="6a959-121">String</span><span class="sxs-lookup"><span data-stu-id="6a959-121">String</span></span>|<span data-ttu-id="6a959-122">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="6a959-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="6a959-123">id</span><span class="sxs-lookup"><span data-stu-id="6a959-123">id</span></span>|<span data-ttu-id="6a959-124">String</span><span class="sxs-lookup"><span data-stu-id="6a959-124">String</span></span>| <span data-ttu-id="6a959-125">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="6a959-125">The attachment ID.</span></span>|
|<span data-ttu-id="6a959-126">isInline</span><span class="sxs-lookup"><span data-stu-id="6a959-126">isInline</span></span>|<span data-ttu-id="6a959-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a959-127">Boolean</span></span>|<span data-ttu-id="6a959-128">如果附件是内联的（例如嵌入到项目正文中的图像），请设置为 true。</span><span class="sxs-lookup"><span data-stu-id="6a959-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="6a959-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a959-129">lastModifiedDateTime</span></span>|<span data-ttu-id="6a959-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a959-130">DateTimeOffset</span></span>|<span data-ttu-id="6a959-131">上次修改附件的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="6a959-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="6a959-132">name</span><span class="sxs-lookup"><span data-stu-id="6a959-132">name</span></span>|<span data-ttu-id="6a959-133">String</span><span class="sxs-lookup"><span data-stu-id="6a959-133">String</span></span>|<span data-ttu-id="6a959-134">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6a959-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="6a959-135">大小</span><span class="sxs-lookup"><span data-stu-id="6a959-135">size</span></span>|<span data-ttu-id="6a959-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6a959-136">Int32</span></span>|<span data-ttu-id="6a959-137">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="6a959-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a959-138">关系</span><span class="sxs-lookup"><span data-stu-id="6a959-138">Relationships</span></span>
| <span data-ttu-id="6a959-139">关系</span><span class="sxs-lookup"><span data-stu-id="6a959-139">Relationship</span></span> | <span data-ttu-id="6a959-140">类型</span><span class="sxs-lookup"><span data-stu-id="6a959-140">Type</span></span>   |<span data-ttu-id="6a959-141">说明</span><span class="sxs-lookup"><span data-stu-id="6a959-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a959-142">项</span><span class="sxs-lookup"><span data-stu-id="6a959-142">item</span></span>|[<span data-ttu-id="6a959-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="6a959-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="6a959-p101">附加的消息或事件。导航属性。</span><span class="sxs-lookup"><span data-stu-id="6a959-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a959-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a959-146">JSON representation</span></span>

<span data-ttu-id="6a959-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a959-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
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
