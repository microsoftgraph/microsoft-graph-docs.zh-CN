---
title: teamworkActivityTopic 资源类型
description: 代表活动源通知的主题。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a4425053cf41ebfbad139c6d0ea5fc246f0b1391
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377522"
---
# <a name="teamworkactivitytopic-resource-type"></a><span data-ttu-id="7031f-103">teamworkActivityTopic 资源类型</span><span class="sxs-lookup"><span data-stu-id="7031f-103">teamworkActivityTopic resource type</span></span>

<span data-ttu-id="7031f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7031f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7031f-105">代表活动源通知的主题。</span><span class="sxs-lookup"><span data-stu-id="7031f-105">Represents the topic of an activity feed notification.</span></span>

## <a name="properties"></a><span data-ttu-id="7031f-106">属性</span><span class="sxs-lookup"><span data-stu-id="7031f-106">Properties</span></span>
|<span data-ttu-id="7031f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7031f-107">Property</span></span>|<span data-ttu-id="7031f-108">类型</span><span class="sxs-lookup"><span data-stu-id="7031f-108">Type</span></span>|<span data-ttu-id="7031f-109">说明</span><span class="sxs-lookup"><span data-stu-id="7031f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7031f-110">source</span><span class="sxs-lookup"><span data-stu-id="7031f-110">source</span></span>|<span data-ttu-id="7031f-111">teamworkActivityTopicSource</span><span class="sxs-lookup"><span data-stu-id="7031f-111">teamworkActivityTopicSource</span></span>|<span data-ttu-id="7031f-112">源的类型。</span><span class="sxs-lookup"><span data-stu-id="7031f-112">Type of source.</span></span> <span data-ttu-id="7031f-113">可取值为：`entityUrl`、`text`。</span><span class="sxs-lookup"><span data-stu-id="7031f-113">Possible values are: `entityUrl`, `text`.</span></span> <span data-ttu-id="7031f-114">若要获取受支持的 Microsoft Graph Url，请使用 `entityUrl` 。</span><span class="sxs-lookup"><span data-stu-id="7031f-114">For supported Microsoft Graph URLs, use `entityUrl`.</span></span> <span data-ttu-id="7031f-115">对于自定义文本，请使用 `text` 。</span><span class="sxs-lookup"><span data-stu-id="7031f-115">For custom text, use `text`.</span></span>|
|<span data-ttu-id="7031f-116">value</span><span class="sxs-lookup"><span data-stu-id="7031f-116">value</span></span>|<span data-ttu-id="7031f-117">String</span><span class="sxs-lookup"><span data-stu-id="7031f-117">String</span></span>|<span data-ttu-id="7031f-118">主题值。</span><span class="sxs-lookup"><span data-stu-id="7031f-118">The topic value.</span></span> <span data-ttu-id="7031f-119">如果 **source** 属性的值为，则 `entityUrl` 它必须是 Microsoft Graph URL。</span><span class="sxs-lookup"><span data-stu-id="7031f-119">If the value of the **source** property is `entityUrl`, this must be a Microsoft Graph URL.</span></span> <span data-ttu-id="7031f-120">如果 vaule 为 `text` ，则它必须为纯文本值。</span><span class="sxs-lookup"><span data-stu-id="7031f-120">If the vaule is `text`, this must be a plain text value.</span></span>|
|<span data-ttu-id="7031f-121">WebUrl</span><span class="sxs-lookup"><span data-stu-id="7031f-121">webUrl</span></span>|<span data-ttu-id="7031f-122">String</span><span class="sxs-lookup"><span data-stu-id="7031f-122">String</span></span>|<span data-ttu-id="7031f-123">用户在选择通知时单击的链接。</span><span class="sxs-lookup"><span data-stu-id="7031f-123">The link the user clicks when they select the notification.</span></span> <span data-ttu-id="7031f-124">**源** 为时 `entityUrl` 为可选;**源** 为时为必需 `text` 。</span><span class="sxs-lookup"><span data-stu-id="7031f-124">Optional when **source** is `entityUrl`; required when **source** is `text`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7031f-125">关系</span><span class="sxs-lookup"><span data-stu-id="7031f-125">Relationships</span></span>
<span data-ttu-id="7031f-126">无。</span><span class="sxs-lookup"><span data-stu-id="7031f-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7031f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7031f-127">JSON representation</span></span>
<span data-ttu-id="7031f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7031f-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivityTopic"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.teamworkActivityTopic",
  "source": "String",
  "value": "String",
  "webUrl": "String"
}
```

