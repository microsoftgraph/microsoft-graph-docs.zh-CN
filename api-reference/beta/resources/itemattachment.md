---
title: itemAttachment 资源类型
description: 附加到另一事件的联系人、事件或邮件，
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 5544c2d4530832f1d18d9760445821fbafeec6e3
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849763"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="01204-103">itemAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="01204-103">itemAttachment resource type</span></span>

<span data-ttu-id="01204-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01204-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="01204-105">附加到用户事件、邮件、Outlook 任务[或](../resources/event.md)帖子[的联系人](../resources/message.md)[、事件](../resources/outlooktask.md)或[邮件](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="01204-105">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="01204-106">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="01204-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="01204-107">方法</span><span class="sxs-lookup"><span data-stu-id="01204-107">Methods</span></span>

| <span data-ttu-id="01204-108">方法</span><span class="sxs-lookup"><span data-stu-id="01204-108">Method</span></span>       | <span data-ttu-id="01204-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="01204-109">Return Type</span></span>  |<span data-ttu-id="01204-110">说明</span><span class="sxs-lookup"><span data-stu-id="01204-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01204-111">Get</span><span class="sxs-lookup"><span data-stu-id="01204-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="01204-112">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="01204-112">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="01204-113">读取 itemAttachment 对象的属性、关系或原始内容。</span><span class="sxs-lookup"><span data-stu-id="01204-113">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|[<span data-ttu-id="01204-114">删除</span><span class="sxs-lookup"><span data-stu-id="01204-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="01204-115">无</span><span class="sxs-lookup"><span data-stu-id="01204-115">None</span></span> |<span data-ttu-id="01204-116">删除 itemAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="01204-116">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="01204-117">属性</span><span class="sxs-lookup"><span data-stu-id="01204-117">Properties</span></span>
| <span data-ttu-id="01204-118">属性</span><span class="sxs-lookup"><span data-stu-id="01204-118">Property</span></span>     | <span data-ttu-id="01204-119">类型</span><span class="sxs-lookup"><span data-stu-id="01204-119">Type</span></span>   |<span data-ttu-id="01204-120">说明</span><span class="sxs-lookup"><span data-stu-id="01204-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01204-121">contentType</span><span class="sxs-lookup"><span data-stu-id="01204-121">contentType</span></span>|<span data-ttu-id="01204-122">String</span><span class="sxs-lookup"><span data-stu-id="01204-122">String</span></span>|<span data-ttu-id="01204-123">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="01204-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="01204-124">id</span><span class="sxs-lookup"><span data-stu-id="01204-124">id</span></span>|<span data-ttu-id="01204-125">String</span><span class="sxs-lookup"><span data-stu-id="01204-125">String</span></span>| <span data-ttu-id="01204-126">附件 ID。</span><span class="sxs-lookup"><span data-stu-id="01204-126">The attachment ID.</span></span>|
|<span data-ttu-id="01204-127">isInline</span><span class="sxs-lookup"><span data-stu-id="01204-127">isInline</span></span>|<span data-ttu-id="01204-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="01204-128">Boolean</span></span>|<span data-ttu-id="01204-129">如果附件是内联的（例如嵌入到项目正文中的图像），请设置为 true。</span><span class="sxs-lookup"><span data-stu-id="01204-129">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="01204-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01204-130">lastModifiedDateTime</span></span>|<span data-ttu-id="01204-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01204-131">DateTimeOffset</span></span>|<span data-ttu-id="01204-132">上次修改附件的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="01204-132">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="01204-133">name</span><span class="sxs-lookup"><span data-stu-id="01204-133">name</span></span>|<span data-ttu-id="01204-134">String</span><span class="sxs-lookup"><span data-stu-id="01204-134">String</span></span>|<span data-ttu-id="01204-135">附件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="01204-135">The display name of the attachment.</span></span>|
|<span data-ttu-id="01204-136">大小</span><span class="sxs-lookup"><span data-stu-id="01204-136">size</span></span>|<span data-ttu-id="01204-137">Int32</span><span class="sxs-lookup"><span data-stu-id="01204-137">Int32</span></span>|<span data-ttu-id="01204-138">附件大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="01204-138">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01204-139">关系</span><span class="sxs-lookup"><span data-stu-id="01204-139">Relationships</span></span>
| <span data-ttu-id="01204-140">关系</span><span class="sxs-lookup"><span data-stu-id="01204-140">Relationship</span></span> | <span data-ttu-id="01204-141">类型</span><span class="sxs-lookup"><span data-stu-id="01204-141">Type</span></span>   |<span data-ttu-id="01204-142">说明</span><span class="sxs-lookup"><span data-stu-id="01204-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01204-143">项</span><span class="sxs-lookup"><span data-stu-id="01204-143">item</span></span>|[<span data-ttu-id="01204-144">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="01204-144">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="01204-p101">连接的联系人、邮件或事件。导航属性。</span><span class="sxs-lookup"><span data-stu-id="01204-p101">The attached contact, message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01204-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01204-147">JSON representation</span></span>

<span data-ttu-id="01204-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01204-148">Here is a JSON representation of the resource</span></span>

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
