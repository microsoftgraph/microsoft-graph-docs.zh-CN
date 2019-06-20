---
title: chatMessageHostedImage 资源类型
description: 代表了 chatmessage 中的承载的图像。
localization_priority: Normal
author: clearab
ms.openlocfilehash: 1f7ce24dfae680937ecb1c43f9a34f6b9bb35646
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/20/2019
ms.locfileid: "35085814"
---
# <a name="chatmessagehostedimage-resource-type"></a><span data-ttu-id="d37e5-103">chatMessageHostedImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="d37e5-103">chatMessageHostedImage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d37e5-104">代表[了 chatmessage](../resources/chatmessage.md)中的承载的图像。</span><span class="sxs-lookup"><span data-stu-id="d37e5-104">Represents a hosted image inside a [chatMessage](../resources/chatmessage.md).</span></span>

<span data-ttu-id="d37e5-105">托管图像是显示在邮件正文中的图像。包含以开头`https://graph.microsoft.com`的 src \<属性的 img> 标记中的**内容。**</span><span class="sxs-lookup"><span data-stu-id="d37e5-105">Hosted images are the images that appear in the message's **body.content** in an \<img> tag with a src attribute that starts with `https://graph.microsoft.com`.</span></span>

<span data-ttu-id="d37e5-106">并非邮件中的所有图像都承载图像, Microsoft 团队还支持公用图像 (其中 img src 属性指向公共网站)。</span><span class="sxs-lookup"><span data-stu-id="d37e5-106">Not all images in a message are hosted images, Microsoft Teams also supports public images (where the img src attribute points to a public website).</span></span>

## <a name="methods"></a><span data-ttu-id="d37e5-107">方法</span><span class="sxs-lookup"><span data-stu-id="d37e5-107">Methods</span></span>

| <span data-ttu-id="d37e5-108">方法</span><span class="sxs-lookup"><span data-stu-id="d37e5-108">Method</span></span>       | <span data-ttu-id="d37e5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d37e5-109">Return Type</span></span>  |<span data-ttu-id="d37e5-110">说明</span><span class="sxs-lookup"><span data-stu-id="d37e5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d37e5-111">在了 chatmessage 中列出 chatMessageHostedImages</span><span class="sxs-lookup"><span data-stu-id="d37e5-111">List chatMessageHostedImages in a chatMessage</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="d37e5-112">[chatMessageHostedImage](chatmessagehostedimage.md)集合</span><span class="sxs-lookup"><span data-stu-id="d37e5-112">[chatMessageHostedImage](chatmessagehostedimage.md) collection</span></span> | <span data-ttu-id="d37e5-113">**了 chatmessage**中所有托管图像的列表。</span><span class="sxs-lookup"><span data-stu-id="d37e5-113">List of all hosted images in a **chatMessage**.</span></span>|
|[<span data-ttu-id="d37e5-114">获取 chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="d37e5-114">Get chatMessageHostedImage</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="d37e5-115">chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="d37e5-115">chatMessageHostedImage</span></span>](chatmessagehostedimage.md) | <span data-ttu-id="d37e5-116">获取一个托管的图像。</span><span class="sxs-lookup"><span data-stu-id="d37e5-116">Get a single hosted image.</span></span>|
|[<span data-ttu-id="d37e5-117">chatMessageHostedImage: getBytes</span><span class="sxs-lookup"><span data-stu-id="d37e5-117">chatMessageHostedImage: getBytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="d37e5-118">内容类型: 图像/jpeg</span><span class="sxs-lookup"><span data-stu-id="d37e5-118">Content-type: image/jpeg</span></span> | <span data-ttu-id="d37e5-119">获取托管图像的原始字节。</span><span class="sxs-lookup"><span data-stu-id="d37e5-119">Get the raw bytes of the hosted image.</span></span>|

## <a name="properties"></a><span data-ttu-id="d37e5-120">属性</span><span class="sxs-lookup"><span data-stu-id="d37e5-120">Properties</span></span>

| <span data-ttu-id="d37e5-121">属性</span><span class="sxs-lookup"><span data-stu-id="d37e5-121">Property</span></span>     | <span data-ttu-id="d37e5-122">类型</span><span class="sxs-lookup"><span data-stu-id="d37e5-122">Type</span></span>   |<span data-ttu-id="d37e5-123">说明</span><span class="sxs-lookup"><span data-stu-id="d37e5-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d37e5-124">id</span><span class="sxs-lookup"><span data-stu-id="d37e5-124">id</span></span>|<span data-ttu-id="d37e5-125">String</span><span class="sxs-lookup"><span data-stu-id="d37e5-125">String</span></span>| <span data-ttu-id="d37e5-126">只读。</span><span class="sxs-lookup"><span data-stu-id="d37e5-126">Read-only.</span></span> <span data-ttu-id="d37e5-127">消息的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="d37e5-127">Unique ID of the message.</span></span>|
|<span data-ttu-id="d37e5-128">URL</span><span class="sxs-lookup"><span data-stu-id="d37e5-128">URL</span></span>| <span data-ttu-id="d37e5-129">string</span><span class="sxs-lookup"><span data-stu-id="d37e5-129">string</span></span> | <span data-ttu-id="d37e5-130">从中检索图像内容的 url。</span><span class="sxs-lookup"><span data-stu-id="d37e5-130">The url to retrieve the image contents from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d37e5-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d37e5-131">JSON representation</span></span>

<span data-ttu-id="d37e5-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d37e5-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
