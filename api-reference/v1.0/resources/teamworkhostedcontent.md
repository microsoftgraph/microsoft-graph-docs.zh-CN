---
title: teamworkHostedContent 资源类型
description: 表示 Microsoft Teams 托管的丰富内容。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a4a4d0a553f77766dd4ddb1f68e27b440fdbf2f
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634294"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="53a02-103">teamworkHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="53a02-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="53a02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53a02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53a02-105">表示 Microsoft Teams 中的丰富内容，如图像和代码段。</span><span class="sxs-lookup"><span data-stu-id="53a02-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="53a02-106">有关频道和聊天消息[中的丰富内容](chatMessage.md)，请参阅[chatMessageHostedContent。](chatMessageHostedContent.md)</span><span class="sxs-lookup"><span data-stu-id="53a02-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="properties"></a><span data-ttu-id="53a02-107">属性</span><span class="sxs-lookup"><span data-stu-id="53a02-107">Properties</span></span>
|<span data-ttu-id="53a02-108">属性</span><span class="sxs-lookup"><span data-stu-id="53a02-108">Property</span></span>|<span data-ttu-id="53a02-109">类型</span><span class="sxs-lookup"><span data-stu-id="53a02-109">Type</span></span>|<span data-ttu-id="53a02-110">说明</span><span class="sxs-lookup"><span data-stu-id="53a02-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53a02-111">contentBytes</span><span class="sxs-lookup"><span data-stu-id="53a02-111">contentBytes</span></span>|<span data-ttu-id="53a02-112">Binary</span><span class="sxs-lookup"><span data-stu-id="53a02-112">Binary</span></span>|<span data-ttu-id="53a02-113">仅写入。</span><span class="sxs-lookup"><span data-stu-id="53a02-113">Write only.</span></span> <span data-ttu-id="53a02-114">托管内容存储的字节 (例如图像) 。</span><span class="sxs-lookup"><span data-stu-id="53a02-114">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="53a02-115">contentType</span><span class="sxs-lookup"><span data-stu-id="53a02-115">contentType</span></span>|<span data-ttu-id="53a02-116">String</span><span class="sxs-lookup"><span data-stu-id="53a02-116">String</span></span>|<span data-ttu-id="53a02-117">仅写入。</span><span class="sxs-lookup"><span data-stu-id="53a02-117">Write only.</span></span> <span data-ttu-id="53a02-118">内容类型。</span><span class="sxs-lookup"><span data-stu-id="53a02-118">Content type.</span></span> <span data-ttu-id="53a02-119">sicj as image/png， image/jpg.</span><span class="sxs-lookup"><span data-stu-id="53a02-119">sicj as image/png, image/jpg.</span></span>|
|<span data-ttu-id="53a02-120">id</span><span class="sxs-lookup"><span data-stu-id="53a02-120">id</span></span>|<span data-ttu-id="53a02-121">String</span><span class="sxs-lookup"><span data-stu-id="53a02-121">String</span></span>|<span data-ttu-id="53a02-122">托管内容的 ID。</span><span class="sxs-lookup"><span data-stu-id="53a02-122">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53a02-123">关系</span><span class="sxs-lookup"><span data-stu-id="53a02-123">Relationships</span></span>
<span data-ttu-id="53a02-124">无。</span><span class="sxs-lookup"><span data-stu-id="53a02-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53a02-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53a02-125">JSON representation</span></span>
<span data-ttu-id="53a02-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53a02-126">The following is a JSON representation of the resource.</span></span>
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
