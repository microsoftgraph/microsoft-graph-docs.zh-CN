---
title: teamworkActivityTopic 资源类型
description: 表示活动源通知的主题。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abf2372aca7d58061f609c97521795f328af89f6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473993"
---
# <a name="teamworkactivitytopic-resource-type"></a><span data-ttu-id="9d415-103">teamworkActivityTopic 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d415-103">teamworkActivityTopic resource type</span></span>

<span data-ttu-id="9d415-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d415-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d415-105">表示活动源通知的主题。</span><span class="sxs-lookup"><span data-stu-id="9d415-105">Represents the topic of an activity feed notification.</span></span>

## <a name="properties"></a><span data-ttu-id="9d415-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d415-106">Properties</span></span>
|<span data-ttu-id="9d415-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d415-107">Property</span></span>|<span data-ttu-id="9d415-108">类型</span><span class="sxs-lookup"><span data-stu-id="9d415-108">Type</span></span>|<span data-ttu-id="9d415-109">说明</span><span class="sxs-lookup"><span data-stu-id="9d415-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d415-110">source</span><span class="sxs-lookup"><span data-stu-id="9d415-110">source</span></span>|<span data-ttu-id="9d415-111">teamworkActivityTopicSource</span><span class="sxs-lookup"><span data-stu-id="9d415-111">teamworkActivityTopicSource</span></span>|<span data-ttu-id="9d415-112">源的类型。</span><span class="sxs-lookup"><span data-stu-id="9d415-112">Type of source.</span></span> <span data-ttu-id="9d415-113">可取值为：`entityUrl`、`text`。</span><span class="sxs-lookup"><span data-stu-id="9d415-113">Possible values are: `entityUrl`, `text`.</span></span> <span data-ttu-id="9d415-114">对于支持的 Microsoft Graph URL，请使用 `entityUrl` 。</span><span class="sxs-lookup"><span data-stu-id="9d415-114">For supported Microsoft Graph URLs, use `entityUrl`.</span></span> <span data-ttu-id="9d415-115">对于自定义文本，请使用 `text` 。</span><span class="sxs-lookup"><span data-stu-id="9d415-115">For custom text, use `text`.</span></span>|
|<span data-ttu-id="9d415-116">value</span><span class="sxs-lookup"><span data-stu-id="9d415-116">value</span></span>|<span data-ttu-id="9d415-117">String</span><span class="sxs-lookup"><span data-stu-id="9d415-117">String</span></span>|<span data-ttu-id="9d415-118">主题值。</span><span class="sxs-lookup"><span data-stu-id="9d415-118">The topic value.</span></span> <span data-ttu-id="9d415-119">如果源 **属性的值为** `entityUrl` ，则它必须是 Microsoft Graph URL。</span><span class="sxs-lookup"><span data-stu-id="9d415-119">If the value of the **source** property is `entityUrl`, this must be a Microsoft Graph URL.</span></span> <span data-ttu-id="9d415-120">如果模块是 `text` ，则它必须是纯文本值。</span><span class="sxs-lookup"><span data-stu-id="9d415-120">If the vaule is `text`, this must be a plain text value.</span></span>|
|<span data-ttu-id="9d415-121">webUrl</span><span class="sxs-lookup"><span data-stu-id="9d415-121">webUrl</span></span>|<span data-ttu-id="9d415-122">String</span><span class="sxs-lookup"><span data-stu-id="9d415-122">String</span></span>|<span data-ttu-id="9d415-123">用户在选择通知时单击的链接。</span><span class="sxs-lookup"><span data-stu-id="9d415-123">The link the user clicks when they select the notification.</span></span> <span data-ttu-id="9d415-124">当 **source** 为 `entityUrl` 时可选;当 **source** 为 时为 必需 `text` 。</span><span class="sxs-lookup"><span data-stu-id="9d415-124">Optional when **source** is `entityUrl`; required when **source** is `text`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d415-125">关系</span><span class="sxs-lookup"><span data-stu-id="9d415-125">Relationships</span></span>
<span data-ttu-id="9d415-126">无。</span><span class="sxs-lookup"><span data-stu-id="9d415-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d415-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d415-127">JSON representation</span></span>
<span data-ttu-id="9d415-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d415-128">The following is a JSON representation of the resource.</span></span>
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

