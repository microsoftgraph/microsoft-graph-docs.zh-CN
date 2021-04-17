---
title: teamworkHostedContent 资源类型
description: 表示由 Microsoft Teams 托管的丰富内容
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da0b157bab78867bd3309b4529afe8ef734f0144
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882311"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="8a154-103">teamworkHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a154-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="8a154-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a154-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a154-105">表示 Microsoft Teams 中的丰富内容，如图像和代码段。</span><span class="sxs-lookup"><span data-stu-id="8a154-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="8a154-106">有关频道和聊天 [消息中的丰富内容，](chatMessage.md)请参阅 [chatMessageHostedContent](chatMessageHostedContent.md)。</span><span class="sxs-lookup"><span data-stu-id="8a154-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8a154-107">方法</span><span class="sxs-lookup"><span data-stu-id="8a154-107">Methods</span></span>

| <span data-ttu-id="8a154-108">方法</span><span class="sxs-lookup"><span data-stu-id="8a154-108">Method</span></span>                                            | <span data-ttu-id="8a154-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a154-109">Return Type</span></span>                                       | <span data-ttu-id="8a154-110">说明</span><span class="sxs-lookup"><span data-stu-id="8a154-110">Description</span></span>                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [<span data-ttu-id="8a154-111">获取应用图标字节数</span><span class="sxs-lookup"><span data-stu-id="8a154-111">Get app icon bytes</span></span>](../api/teamsappicon-get.md)     | [<span data-ttu-id="8a154-112">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="8a154-112">teamworkHostedContent</span></span>](teamworkhostedcontent.md)                   | <span data-ttu-id="8a154-113">获取支持 Teams 应用图标的托管内容的字节数。</span><span class="sxs-lookup"><span data-stu-id="8a154-113">Get the bytes of the hosted content backing a Teams app icon.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a154-114">属性</span><span class="sxs-lookup"><span data-stu-id="8a154-114">Properties</span></span>
|<span data-ttu-id="8a154-115">属性</span><span class="sxs-lookup"><span data-stu-id="8a154-115">Property</span></span>|<span data-ttu-id="8a154-116">类型</span><span class="sxs-lookup"><span data-stu-id="8a154-116">Type</span></span>|<span data-ttu-id="8a154-117">说明</span><span class="sxs-lookup"><span data-stu-id="8a154-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a154-118">contentBytes</span><span class="sxs-lookup"><span data-stu-id="8a154-118">contentBytes</span></span>|<span data-ttu-id="8a154-119">Binary</span><span class="sxs-lookup"><span data-stu-id="8a154-119">Binary</span></span>|<span data-ttu-id="8a154-120">只写。</span><span class="sxs-lookup"><span data-stu-id="8a154-120">Write only.</span></span> <span data-ttu-id="8a154-121">托管内容存储的字节 (如图像) 。</span><span class="sxs-lookup"><span data-stu-id="8a154-121">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="8a154-122">contentType</span><span class="sxs-lookup"><span data-stu-id="8a154-122">contentType</span></span>|<span data-ttu-id="8a154-123">String</span><span class="sxs-lookup"><span data-stu-id="8a154-123">String</span></span>|<span data-ttu-id="8a154-124">只写。</span><span class="sxs-lookup"><span data-stu-id="8a154-124">Write only.</span></span> <span data-ttu-id="8a154-125">内容类型，如 image/png、image/jpg。</span><span class="sxs-lookup"><span data-stu-id="8a154-125">Content type, such as image/png, image/jpg.</span></span>|
|<span data-ttu-id="8a154-126">id</span><span class="sxs-lookup"><span data-stu-id="8a154-126">id</span></span>|<span data-ttu-id="8a154-127">String</span><span class="sxs-lookup"><span data-stu-id="8a154-127">String</span></span>|<span data-ttu-id="8a154-128">托管内容的 ID。</span><span class="sxs-lookup"><span data-stu-id="8a154-128">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a154-129">关系</span><span class="sxs-lookup"><span data-stu-id="8a154-129">Relationships</span></span>
<span data-ttu-id="8a154-130">无。</span><span class="sxs-lookup"><span data-stu-id="8a154-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a154-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a154-131">JSON representation</span></span>
<span data-ttu-id="8a154-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a154-132">The following is a JSON representation of the resource.</span></span>
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

