---
title: itemAttachment 资源类型
description: 附加到另一个事件的联系人、事件或邮件,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: b4220a1428edab2eeab89cabe53efc91bea76a8b
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484378"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="efe8b-103">itemAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="efe8b-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efe8b-104">附加到另一个[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[公告](../resources/post.md)的联系人、事件或邮件。</span><span class="sxs-lookup"><span data-stu-id="efe8b-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="efe8b-105">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="efe8b-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="efe8b-106">方法</span><span class="sxs-lookup"><span data-stu-id="efe8b-106">Methods</span></span>

| <span data-ttu-id="efe8b-107">方法</span><span class="sxs-lookup"><span data-stu-id="efe8b-107">Method</span></span>       | <span data-ttu-id="efe8b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="efe8b-108">Return Type</span></span>  |<span data-ttu-id="efe8b-109">说明</span><span class="sxs-lookup"><span data-stu-id="efe8b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efe8b-110">Get</span><span class="sxs-lookup"><span data-stu-id="efe8b-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="efe8b-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="efe8b-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="efe8b-112">读取 itemAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efe8b-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="efe8b-113">删除</span><span class="sxs-lookup"><span data-stu-id="efe8b-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="efe8b-114">无</span><span class="sxs-lookup"><span data-stu-id="efe8b-114">None</span></span> |<span data-ttu-id="efe8b-115">删除 itemAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="efe8b-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="efe8b-116">属性</span><span class="sxs-lookup"><span data-stu-id="efe8b-116">Properties</span></span>
| <span data-ttu-id="efe8b-117">属性</span><span class="sxs-lookup"><span data-stu-id="efe8b-117">Property</span></span>     | <span data-ttu-id="efe8b-118">类型</span><span class="sxs-lookup"><span data-stu-id="efe8b-118">Type</span></span>   |<span data-ttu-id="efe8b-119">说明</span><span class="sxs-lookup"><span data-stu-id="efe8b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe8b-120">contentType</span><span class="sxs-lookup"><span data-stu-id="efe8b-120">contentType</span></span>|<span data-ttu-id="efe8b-121">String</span><span class="sxs-lookup"><span data-stu-id="efe8b-121">String</span></span>|<span data-ttu-id="efe8b-122">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="efe8b-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="efe8b-123">id</span><span class="sxs-lookup"><span data-stu-id="efe8b-123">id</span></span>|<span data-ttu-id="efe8b-124">String</span><span class="sxs-lookup"><span data-stu-id="efe8b-124">String</span></span>| <span data-ttu-id="efe8b-125">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="efe8b-125">The attachment ID.</span></span>|
|<span data-ttu-id="efe8b-126">isInline</span><span class="sxs-lookup"><span data-stu-id="efe8b-126">isInline</span></span>|<span data-ttu-id="efe8b-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="efe8b-127">Boolean</span></span>|<span data-ttu-id="efe8b-128">如果附件是内联的（例如嵌入到项目正文中的图像），请设置为 true。</span><span class="sxs-lookup"><span data-stu-id="efe8b-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="efe8b-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efe8b-129">lastModifiedDateTime</span></span>|<span data-ttu-id="efe8b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efe8b-130">DateTimeOffset</span></span>|<span data-ttu-id="efe8b-131">上次修改附件的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="efe8b-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="efe8b-132">name</span><span class="sxs-lookup"><span data-stu-id="efe8b-132">name</span></span>|<span data-ttu-id="efe8b-133">String</span><span class="sxs-lookup"><span data-stu-id="efe8b-133">String</span></span>|<span data-ttu-id="efe8b-134">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="efe8b-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="efe8b-135">大小</span><span class="sxs-lookup"><span data-stu-id="efe8b-135">size</span></span>|<span data-ttu-id="efe8b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="efe8b-136">Int32</span></span>|<span data-ttu-id="efe8b-137">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="efe8b-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efe8b-138">关系</span><span class="sxs-lookup"><span data-stu-id="efe8b-138">Relationships</span></span>
| <span data-ttu-id="efe8b-139">关系</span><span class="sxs-lookup"><span data-stu-id="efe8b-139">Relationship</span></span> | <span data-ttu-id="efe8b-140">类型</span><span class="sxs-lookup"><span data-stu-id="efe8b-140">Type</span></span>   |<span data-ttu-id="efe8b-141">说明</span><span class="sxs-lookup"><span data-stu-id="efe8b-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe8b-142">项</span><span class="sxs-lookup"><span data-stu-id="efe8b-142">item</span></span>|[<span data-ttu-id="efe8b-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="efe8b-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="efe8b-144">附加的联系人、消息或事件。</span><span class="sxs-lookup"><span data-stu-id="efe8b-144">The attached contact, message or event.</span></span> <span data-ttu-id="efe8b-145">导航属性。</span><span class="sxs-lookup"><span data-stu-id="efe8b-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efe8b-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efe8b-146">JSON representation</span></span>

<span data-ttu-id="efe8b-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efe8b-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
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
<!--
{
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
