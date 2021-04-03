---
title: chatMessageAttachment 资源类型
description: 表示聊天消息实体的附件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: b4660e92643d868fbd09c693187a486fc3937584
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582569"
---
# <a name="chatmessageattachment-resource-type"></a><span data-ttu-id="314c6-103">chatMessageAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="314c6-103">chatMessageAttachment resource type</span></span>

<span data-ttu-id="314c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="314c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="314c6-105">表示聊天消息实体的附件。</span><span class="sxs-lookup"><span data-stu-id="314c6-105">Represents an attachment to a chat message entity.</span></span>

<span data-ttu-id="314c6-106">类型实体作为 `chatMessageAttachment` [chatMessage](chatmessage.md)实体的一部分作为[获取](../api/channel-list-messages.md)频道消息 API 的一部分返回。</span><span class="sxs-lookup"><span data-stu-id="314c6-106">An entity of type `chatMessageAttachment` is returned as part of the [Get channel messages](../api/channel-list-messages.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="314c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="314c6-107">Properties</span></span>
| <span data-ttu-id="314c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="314c6-108">Property</span></span>     | <span data-ttu-id="314c6-109">类型</span><span class="sxs-lookup"><span data-stu-id="314c6-109">Type</span></span>   |<span data-ttu-id="314c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="314c6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="314c6-111">id</span><span class="sxs-lookup"><span data-stu-id="314c6-111">id</span></span>|<span data-ttu-id="314c6-112">string</span><span class="sxs-lookup"><span data-stu-id="314c6-112">string</span></span>| <span data-ttu-id="314c6-113">只读。</span><span class="sxs-lookup"><span data-stu-id="314c6-113">Read-only.</span></span> <span data-ttu-id="314c6-114">附件的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="314c6-114">Unique id of the attachment.</span></span>|
|<span data-ttu-id="314c6-115">contentType</span><span class="sxs-lookup"><span data-stu-id="314c6-115">contentType</span></span>| <span data-ttu-id="314c6-116">string</span><span class="sxs-lookup"><span data-stu-id="314c6-116">string</span></span> | <span data-ttu-id="314c6-117">内容附件的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="314c6-117">The media type of the content attachment.</span></span> <span data-ttu-id="314c6-118">它可以具有以下值：</span><span class="sxs-lookup"><span data-stu-id="314c6-118">It can have the following values:</span></span> <br><ul><li><span data-ttu-id="314c6-119">`reference`：Attachment 是指向其他文件的链接。</span><span class="sxs-lookup"><span data-stu-id="314c6-119">`reference`: Attachment is a link to another file.</span></span> <span data-ttu-id="314c6-120">使用指向对象的链接填充 contentURL。</span><span class="sxs-lookup"><span data-stu-id="314c6-120">Populate the contentURL with the link to the object.</span></span></li><li><span data-ttu-id="314c6-121">Bot Framework 的 Attachment 对象支持的任何 [contentType](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</span><span class="sxs-lookup"><span data-stu-id="314c6-121">Any contentTypes supported by the Bot Framework's [Attachment object](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</span></span></li><li><span data-ttu-id="314c6-122">`application/vnd.microsoft.card.codesnippet`：代码段。</span><span class="sxs-lookup"><span data-stu-id="314c6-122">`application/vnd.microsoft.card.codesnippet`: A code snippet.</span></span> </li><li><span data-ttu-id="314c6-123">`application/vnd.microsoft.card.announcement`：通知标头。</span><span class="sxs-lookup"><span data-stu-id="314c6-123">`application/vnd.microsoft.card.announcement`: An announcement header.</span></span> </li>|
|<span data-ttu-id="314c6-124">contentUrl</span><span class="sxs-lookup"><span data-stu-id="314c6-124">contentUrl</span></span>|<span data-ttu-id="314c6-125">string</span><span class="sxs-lookup"><span data-stu-id="314c6-125">string</span></span>|<span data-ttu-id="314c6-126">附件内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="314c6-126">URL for the content of the attachment.</span></span> <span data-ttu-id="314c6-127">支持的协议：http、https、文件和数据。</span><span class="sxs-lookup"><span data-stu-id="314c6-127">Supported protocols: http, https, file and data.</span></span>|
|<span data-ttu-id="314c6-128">content</span><span class="sxs-lookup"><span data-stu-id="314c6-128">content</span></span>|<span data-ttu-id="314c6-129">string</span><span class="sxs-lookup"><span data-stu-id="314c6-129">string</span></span>|<span data-ttu-id="314c6-130">附件的内容。</span><span class="sxs-lookup"><span data-stu-id="314c6-130">The content of the attachment.</span></span> <span data-ttu-id="314c6-131">如果附件是富 [卡片，](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)将 属性设置为富卡片对象。</span><span class="sxs-lookup"><span data-stu-id="314c6-131">If the attachment is a [rich card](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), set the property to the rich card object.</span></span> <span data-ttu-id="314c6-132">此属性和 contentUrl 相互排斥。</span><span class="sxs-lookup"><span data-stu-id="314c6-132">This property and contentUrl are mutually exclusive.</span></span>|
|<span data-ttu-id="314c6-133">name</span><span class="sxs-lookup"><span data-stu-id="314c6-133">name</span></span>|<span data-ttu-id="314c6-134">string</span><span class="sxs-lookup"><span data-stu-id="314c6-134">string</span></span>|<span data-ttu-id="314c6-135">附件的名称。</span><span class="sxs-lookup"><span data-stu-id="314c6-135">Name of the attachment.</span></span>|
|<span data-ttu-id="314c6-136">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="314c6-136">thumbnailUrl</span></span>| <span data-ttu-id="314c6-137">string</span><span class="sxs-lookup"><span data-stu-id="314c6-137">string</span></span> |<span data-ttu-id="314c6-138">指向缩略图图像的 URL，如果频道支持使用其他较小格式的内容或 contentUrl，可以使用该图像。</span><span class="sxs-lookup"><span data-stu-id="314c6-138">URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.</span></span> <span data-ttu-id="314c6-139">例如，如果将 contentType 设置为 application/word，并且将 contentUrl 设置为 Word 文档的位置，则可能包含表示文档的缩略图图像。</span><span class="sxs-lookup"><span data-stu-id="314c6-139">For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.</span></span> <span data-ttu-id="314c6-140">通道可以显示缩略图图像而不是文档。</span><span class="sxs-lookup"><span data-stu-id="314c6-140">The channel could display the thumbnail image instead of the document.</span></span> <span data-ttu-id="314c6-141">当用户单击该图像时，通道将打开文档。</span><span class="sxs-lookup"><span data-stu-id="314c6-141">When the user clicks the image, the channel would open the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="314c6-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="314c6-142">JSON representation</span></span>
 <span data-ttu-id="314c6-143">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="314c6-143">The following is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


