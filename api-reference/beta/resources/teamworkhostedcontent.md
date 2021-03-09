---
title: teamworkHostedContent 资源类型
description: 表示 Microsoft Teams 托管的丰富内容
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 93b3b4fc817c1fe3aa3973a112b9cf887c825b6e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578849"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="c818c-103">teamworkHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="c818c-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="c818c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c818c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c818c-105">表示 Microsoft Teams 中的丰富内容，如图像和代码段。</span><span class="sxs-lookup"><span data-stu-id="c818c-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="c818c-106">有关频道和聊天消息[中的丰富内容](chatMessage.md)，请参阅[chatMessageHostedContent。](chatMessageHostedContent.md)</span><span class="sxs-lookup"><span data-stu-id="c818c-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c818c-107">属性</span><span class="sxs-lookup"><span data-stu-id="c818c-107">Properties</span></span>
|<span data-ttu-id="c818c-108">属性</span><span class="sxs-lookup"><span data-stu-id="c818c-108">Property</span></span>|<span data-ttu-id="c818c-109">类型</span><span class="sxs-lookup"><span data-stu-id="c818c-109">Type</span></span>|<span data-ttu-id="c818c-110">说明</span><span class="sxs-lookup"><span data-stu-id="c818c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c818c-111">contentBytes</span><span class="sxs-lookup"><span data-stu-id="c818c-111">contentBytes</span></span>|<span data-ttu-id="c818c-112">Binary</span><span class="sxs-lookup"><span data-stu-id="c818c-112">Binary</span></span>|<span data-ttu-id="c818c-113">仅写入。</span><span class="sxs-lookup"><span data-stu-id="c818c-113">Write only.</span></span> <span data-ttu-id="c818c-114">托管内容存储的字节 (例如图像) 。</span><span class="sxs-lookup"><span data-stu-id="c818c-114">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="c818c-115">contentType</span><span class="sxs-lookup"><span data-stu-id="c818c-115">contentType</span></span>|<span data-ttu-id="c818c-116">String</span><span class="sxs-lookup"><span data-stu-id="c818c-116">String</span></span>|<span data-ttu-id="c818c-117">仅写入。</span><span class="sxs-lookup"><span data-stu-id="c818c-117">Write only.</span></span> <span data-ttu-id="c818c-118">内容类型，如 image/png、image/jpg。</span><span class="sxs-lookup"><span data-stu-id="c818c-118">Content type, such as image/png, image/jpg.</span></span>|
|<span data-ttu-id="c818c-119">id</span><span class="sxs-lookup"><span data-stu-id="c818c-119">id</span></span>|<span data-ttu-id="c818c-120">字符串</span><span class="sxs-lookup"><span data-stu-id="c818c-120">String</span></span>|<span data-ttu-id="c818c-121">托管内容的 ID。</span><span class="sxs-lookup"><span data-stu-id="c818c-121">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c818c-122">关系</span><span class="sxs-lookup"><span data-stu-id="c818c-122">Relationships</span></span>
<span data-ttu-id="c818c-123">无。</span><span class="sxs-lookup"><span data-stu-id="c818c-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c818c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c818c-124">JSON representation</span></span>
<span data-ttu-id="c818c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c818c-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```

