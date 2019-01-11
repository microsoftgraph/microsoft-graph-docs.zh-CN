---
title: itemAttachment 资源类型
description: 联系人、 事件或附加到另一个事件的消息
localization_priority: Normal
ms.openlocfilehash: f7372db19a545bd7d6ae39121fd14be4c9f4436b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825002"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="964b9-103">itemAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="964b9-103">itemAttachment resource type</span></span>

> <span data-ttu-id="964b9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="964b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="964b9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="964b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="964b9-106">联系人、 事件或附加到另一个[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)的消息。</span><span class="sxs-lookup"><span data-stu-id="964b9-106">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="964b9-107">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="964b9-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="964b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="964b9-108">Methods</span></span>

| <span data-ttu-id="964b9-109">方法</span><span class="sxs-lookup"><span data-stu-id="964b9-109">Method</span></span>       | <span data-ttu-id="964b9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="964b9-110">Return Type</span></span>  |<span data-ttu-id="964b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="964b9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="964b9-112">Get</span><span class="sxs-lookup"><span data-stu-id="964b9-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="964b9-113">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="964b9-113">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="964b9-114">读取 itemAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="964b9-114">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="964b9-115">删除</span><span class="sxs-lookup"><span data-stu-id="964b9-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="964b9-116">无</span><span class="sxs-lookup"><span data-stu-id="964b9-116">None</span></span> |<span data-ttu-id="964b9-117">删除 itemAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="964b9-117">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="964b9-118">属性</span><span class="sxs-lookup"><span data-stu-id="964b9-118">Properties</span></span>
| <span data-ttu-id="964b9-119">属性</span><span class="sxs-lookup"><span data-stu-id="964b9-119">Property</span></span>     | <span data-ttu-id="964b9-120">类型</span><span class="sxs-lookup"><span data-stu-id="964b9-120">Type</span></span>   |<span data-ttu-id="964b9-121">说明</span><span class="sxs-lookup"><span data-stu-id="964b9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="964b9-122">contentType</span><span class="sxs-lookup"><span data-stu-id="964b9-122">contentType</span></span>|<span data-ttu-id="964b9-123">String</span><span class="sxs-lookup"><span data-stu-id="964b9-123">String</span></span>|<span data-ttu-id="964b9-124">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="964b9-124">The content type of the attachment.</span></span>|
|<span data-ttu-id="964b9-125">id</span><span class="sxs-lookup"><span data-stu-id="964b9-125">id</span></span>|<span data-ttu-id="964b9-126">String</span><span class="sxs-lookup"><span data-stu-id="964b9-126">String</span></span>| <span data-ttu-id="964b9-127">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="964b9-127">The attachment ID.</span></span>|
|<span data-ttu-id="964b9-128">isInline</span><span class="sxs-lookup"><span data-stu-id="964b9-128">isInline</span></span>|<span data-ttu-id="964b9-129">布尔</span><span class="sxs-lookup"><span data-stu-id="964b9-129">Boolean</span></span>|<span data-ttu-id="964b9-130">如果附件是内联的（例如嵌入到项目正文中的图像），请设置为 true。</span><span class="sxs-lookup"><span data-stu-id="964b9-130">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="964b9-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="964b9-131">lastModifiedDateTime</span></span>|<span data-ttu-id="964b9-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="964b9-132">DateTimeOffset</span></span>|<span data-ttu-id="964b9-133">上次修改附件的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="964b9-133">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="964b9-134">name</span><span class="sxs-lookup"><span data-stu-id="964b9-134">name</span></span>|<span data-ttu-id="964b9-135">String</span><span class="sxs-lookup"><span data-stu-id="964b9-135">String</span></span>|<span data-ttu-id="964b9-136">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="964b9-136">The display name of the attachment.</span></span>|
|<span data-ttu-id="964b9-137">大小</span><span class="sxs-lookup"><span data-stu-id="964b9-137">size</span></span>|<span data-ttu-id="964b9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="964b9-138">Int32</span></span>|<span data-ttu-id="964b9-139">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="964b9-139">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="964b9-140">Relationships</span><span class="sxs-lookup"><span data-stu-id="964b9-140">Relationships</span></span>
| <span data-ttu-id="964b9-141">关系</span><span class="sxs-lookup"><span data-stu-id="964b9-141">Relationship</span></span> | <span data-ttu-id="964b9-142">类型</span><span class="sxs-lookup"><span data-stu-id="964b9-142">Type</span></span>   |<span data-ttu-id="964b9-143">说明</span><span class="sxs-lookup"><span data-stu-id="964b9-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="964b9-144">项</span><span class="sxs-lookup"><span data-stu-id="964b9-144">item</span></span>|[<span data-ttu-id="964b9-145">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="964b9-145">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="964b9-146">附加的联系人、 消息或事件中。</span><span class="sxs-lookup"><span data-stu-id="964b9-146">The attached contact, message or event.</span></span> <span data-ttu-id="964b9-147">导航属性。</span><span class="sxs-lookup"><span data-stu-id="964b9-147">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="964b9-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="964b9-148">JSON representation</span></span>

<span data-ttu-id="964b9-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="964b9-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
