---
title: chatMessageAttachment 资源类型
description: 表示聊天消息实体的附件。
localization_priority: Normal
ms.openlocfilehash: 12682ee090a2dc7976db46629cd26df9e5b1595e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640915"
---
# <a name="chatmessageattachment-resource-type"></a><span data-ttu-id="b8785-103">chatMessageAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8785-103">chatMessageAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8785-104">表示聊天消息实体的附件。</span><span class="sxs-lookup"><span data-stu-id="b8785-104">Represents an attachment to a chat message entity.</span></span>

<span data-ttu-id="b8785-105">实体类型的`chatMessageAttachment`返回作为一部分[获取通道消息](../api/channel-list-messages.md)API，作为[chatMessage](chatmessage.md)实体的一部分。</span><span class="sxs-lookup"><span data-stu-id="b8785-105">An entity of type `chatMessageAttachment` is returned as part of the [Get channel messages](../api/channel-list-messages.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="b8785-106">属性</span><span class="sxs-lookup"><span data-stu-id="b8785-106">Properties</span></span>
| <span data-ttu-id="b8785-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8785-107">Property</span></span>     | <span data-ttu-id="b8785-108">类型</span><span class="sxs-lookup"><span data-stu-id="b8785-108">Type</span></span>   |<span data-ttu-id="b8785-109">说明</span><span class="sxs-lookup"><span data-stu-id="b8785-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8785-110">id</span><span class="sxs-lookup"><span data-stu-id="b8785-110">id</span></span>|<span data-ttu-id="b8785-111">string</span><span class="sxs-lookup"><span data-stu-id="b8785-111">string</span></span>| <span data-ttu-id="b8785-112">只读。</span><span class="sxs-lookup"><span data-stu-id="b8785-112">Read-only.</span></span> <span data-ttu-id="b8785-113">附件的唯一 id。</span><span class="sxs-lookup"><span data-stu-id="b8785-113">Unique id of the attachment.</span></span>|
|<span data-ttu-id="b8785-114">contentType</span><span class="sxs-lookup"><span data-stu-id="b8785-114">contentType</span></span>| <span data-ttu-id="b8785-115">string</span><span class="sxs-lookup"><span data-stu-id="b8785-115">string</span></span> | <span data-ttu-id="b8785-116">媒体类型的内容的附件。</span><span class="sxs-lookup"><span data-stu-id="b8785-116">The media type of the content attachment.</span></span> <span data-ttu-id="b8785-117">它可以具有以下值：</span><span class="sxs-lookup"><span data-stu-id="b8785-117">It can have the following values:</span></span> <br><ul><li><span data-ttu-id="b8785-118">参考： 附件是到另一个文件的链接。</span><span class="sxs-lookup"><span data-stu-id="b8785-118">reference: Attachment is a link to another file.</span></span> <span data-ttu-id="b8785-119">填充与对对象链接 contentURL。</span><span class="sxs-lookup"><span data-stu-id="b8785-119">Populate the contentURL with the link to the object.</span></span><br></li><li><span data-ttu-id="b8785-120">文件： 原始文件附件。</span><span class="sxs-lookup"><span data-stu-id="b8785-120">file: Raw file attachment.</span></span> <span data-ttu-id="b8785-121">填充具有中数据的文件的 base64 编码的 contenturl 字段： 格式。</span><span class="sxs-lookup"><span data-stu-id="b8785-121">Populate the contenturl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="b8785-122">图像 /: 与指定的图像的类型图像类型： 图像/png、 image/jpeg 图像/gif。</span><span class="sxs-lookup"><span data-stu-id="b8785-122">image/: Image type with the type of the image specified ex: image/png, image/jpeg, image/gif.</span></span> <span data-ttu-id="b8785-123">填充具有中数据的文件的 base64 编码的 contentUrl 字段： 格式。</span><span class="sxs-lookup"><span data-stu-id="b8785-123">Populate the contentUrl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="b8785-124">视频 /: 视频指定的格式的类型。</span><span class="sxs-lookup"><span data-stu-id="b8785-124">video/: Video type with the format specified.</span></span> <span data-ttu-id="b8785-125">示例： 视频/mp4 （英文)。</span><span class="sxs-lookup"><span data-stu-id="b8785-125">Ex: video/mp4.</span></span> <span data-ttu-id="b8785-126">填充具有中数据的文件的 base64 编码的 contentUrl 字段： 格式。</span><span class="sxs-lookup"><span data-stu-id="b8785-126">Populate the contentUrl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="b8785-127">音频 /: 具有指定的格式的音频类型。</span><span class="sxs-lookup"><span data-stu-id="b8785-127">audio/: Audio type with the format specified.</span></span> <span data-ttu-id="b8785-128">示例： 音频/wmw。</span><span class="sxs-lookup"><span data-stu-id="b8785-128">Ex: audio/wmw.</span></span> <span data-ttu-id="b8785-129">填充具有中数据的文件的 base64 编码的 contentUrl 字段： 格式。</span><span class="sxs-lookup"><span data-stu-id="b8785-129">Populate the contentUrl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="b8785-130">应用程序/名片类型： 富卡片与指定的确切卡格式的卡片类型使用的附件类型。</span><span class="sxs-lookup"><span data-stu-id="b8785-130">application/card type: Rich card attachment type with the card type specifying the exact card format to use.</span></span> <span data-ttu-id="b8785-131">设置与卡片的 json 格式的内容。</span><span class="sxs-lookup"><span data-stu-id="b8785-131">Set content with the json format of the card.</span></span> <span data-ttu-id="b8785-132">支持的名片类型的值包括：</span><span class="sxs-lookup"><span data-stu-id="b8785-132">Supported values for card type include:</span></span><br><ul><li><span data-ttu-id="b8785-133">application/vnd.microsoft.card.adaptive： 可包含文本、 语音、 图像、 按钮和输入的字段的任意组合的丰富卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-133">application/vnd.microsoft.card.adaptive: A rich card that can contain any combination of text, speech, images,,buttons, and input fields.</span></span> <span data-ttu-id="b8785-134">设置对，AdaptiveCard 对象的内容的属性。</span><span class="sxs-lookup"><span data-stu-id="b8785-134">Set the content property to,an AdaptiveCard object.</span></span></li><li><span data-ttu-id="b8785-135">application/vnd.microsoft.card.animation： 播放动画的丰富卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-135">application/vnd.microsoft.card.animation: A rich card that plays animation.</span></span> <span data-ttu-id="b8785-136">设置为 AnimationCardobject 的内容的属性。</span><span class="sxs-lookup"><span data-stu-id="b8785-136">Set the content property,to an AnimationCardobject.</span></span></li><li><span data-ttu-id="b8785-137">application/vnd.microsoft.card.audio： 播放音频文件的丰富卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-137">application/vnd.microsoft.card.audio: A rich card that plays audio files.</span></span> <span data-ttu-id="b8785-138">设置为 AudioCard 对象的内容的属性。</span><span class="sxs-lookup"><span data-stu-id="b8785-138">Set the content property,to an AudioCard object.</span></span></li><li><span data-ttu-id="b8785-139">application/vnd.microsoft.card.video： 播放视频的丰富卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-139">application/vnd.microsoft.card.video: A rich card that plays videos.</span></span> <span data-ttu-id="b8785-140">设置为视频卡的详细对象的内容的属性。</span><span class="sxs-lookup"><span data-stu-id="b8785-140">Set the content property,to a VideoCard object.</span></span></li><li><span data-ttu-id="b8785-141">application/vnd.microsoft.card.hero： 生卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-141">application/vnd.microsoft.card.hero: A Hero card.</span></span> <span data-ttu-id="b8785-142">内容属性设置为 HeroCard 对象。</span><span class="sxs-lookup"><span data-stu-id="b8785-142">Set the content property to a HeroCard object.</span></span></li><li><span data-ttu-id="b8785-143">application/vnd.microsoft.card.thumbnail： 的缩略图卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-143">application/vnd.microsoft.card.thumbnail: A Thumbnail card.</span></span> <span data-ttu-id="b8785-144">内容属性设置为 ThumbnailCard 对象。</span><span class="sxs-lookup"><span data-stu-id="b8785-144">Set the content property to a ThumbnailCard object.</span></span></li><li><span data-ttu-id="b8785-145">application/vnd.microsoft.com.card.receipt： 回执卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-145">application/vnd.microsoft.com.card.receipt: A Receipt card.</span></span> <span data-ttu-id="b8785-146">内容属性设置为 ReceiptCard 对象。</span><span class="sxs-lookup"><span data-stu-id="b8785-146">Set the content property to a ReceiptCard object.</span></span></li><li><span data-ttu-id="b8785-147">application/vnd.microsoft.com.card.signin： 用户登录卡片。</span><span class="sxs-lookup"><span data-stu-id="b8785-147">application/vnd.microsoft.com.card.signin: A user Sign In card.</span></span> <span data-ttu-id="b8785-148">内容属性设置为 SignInCard 对象。</span><span class="sxs-lookup"><span data-stu-id="b8785-148">Set the content property to a SignInCard object.</span></span></ul></ul>|
|<span data-ttu-id="b8785-149">contentUrl</span><span class="sxs-lookup"><span data-stu-id="b8785-149">contentUrl</span></span>|<span data-ttu-id="b8785-150">string</span><span class="sxs-lookup"><span data-stu-id="b8785-150">string</span></span>|<span data-ttu-id="b8785-151">内容的附件的 URL。</span><span class="sxs-lookup"><span data-stu-id="b8785-151">URL for the content of the attachment.</span></span> <span data-ttu-id="b8785-152">支持的协议： http、 https、 文件和数据。</span><span class="sxs-lookup"><span data-stu-id="b8785-152">Supported protocols: http, https, file and data.</span></span>|
|<span data-ttu-id="b8785-153">content</span><span class="sxs-lookup"><span data-stu-id="b8785-153">content</span></span>|<span data-ttu-id="b8785-154">string</span><span class="sxs-lookup"><span data-stu-id="b8785-154">string</span></span>|<span data-ttu-id="b8785-155">附件的内容。</span><span class="sxs-lookup"><span data-stu-id="b8785-155">The content of the attachment.</span></span> <span data-ttu-id="b8785-156">如果附件是丰富卡，设置对丰富卡对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8785-156">If the attachment is a rich card, set the property to the rich card object.</span></span> <span data-ttu-id="b8785-157">此属性和 contentUrl 互斥。</span><span class="sxs-lookup"><span data-stu-id="b8785-157">This property and contentUrl are mutually exclusive.</span></span>|
|<span data-ttu-id="b8785-158">name</span><span class="sxs-lookup"><span data-stu-id="b8785-158">name</span></span>|<span data-ttu-id="b8785-159">string</span><span class="sxs-lookup"><span data-stu-id="b8785-159">string</span></span>|<span data-ttu-id="b8785-160">附件的名称。</span><span class="sxs-lookup"><span data-stu-id="b8785-160">Name of the attachment.</span></span>|
|<span data-ttu-id="b8785-161">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="b8785-161">thumbnailUrl</span></span>| <span data-ttu-id="b8785-162">string</span><span class="sxs-lookup"><span data-stu-id="b8785-162">string</span></span> |<span data-ttu-id="b8785-163">URL 如果它支持使用替代、 较小的内容或 contentUrl 窗体，可以使用该频道的缩略图。</span><span class="sxs-lookup"><span data-stu-id="b8785-163">URL to a a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.</span></span> <span data-ttu-id="b8785-164">例如，如果您将 contentType 设置为应用程序/word，并将 contentUrl 设置为 Word 文档的位置，则可能包括表示的文档的缩略图。</span><span class="sxs-lookup"><span data-stu-id="b8785-164">For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.</span></span> <span data-ttu-id="b8785-165">该频道可以显示而不是文档的缩略图图像。</span><span class="sxs-lookup"><span data-stu-id="b8785-165">The channel could display the thumbnail image instead of the document.</span></span> <span data-ttu-id="b8785-166">当用户单击图像时，通道将打开的文档。</span><span class="sxs-lookup"><span data-stu-id="b8785-166">When the user clicks the image, the channel would open the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8785-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8785-167">JSON representation</span></span>
 <span data-ttu-id="b8785-168">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8785-168">The following is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatAttachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
