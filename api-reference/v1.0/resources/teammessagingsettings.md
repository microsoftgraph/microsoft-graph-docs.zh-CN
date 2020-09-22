---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5fe43e317bd0231bb8d2e87143e4230c8719ce9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093992"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="df2e7-103">teamMessagingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="df2e7-103">teamMessagingSettings resource type</span></span>

<span data-ttu-id="df2e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df2e7-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="df2e7-105">用于配置 [团队](team.md)中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="df2e7-105">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df2e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="df2e7-106">Properties</span></span>
| <span data-ttu-id="df2e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="df2e7-107">Property</span></span>     | <span data-ttu-id="df2e7-108">类型</span><span class="sxs-lookup"><span data-stu-id="df2e7-108">Type</span></span>   |<span data-ttu-id="df2e7-109">说明</span><span class="sxs-lookup"><span data-stu-id="df2e7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df2e7-110">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="df2e7-110">allowUserEditMessages</span></span>|<span data-ttu-id="df2e7-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="df2e7-111">Boolean</span></span>|<span data-ttu-id="df2e7-112">如果设置为 true，则用户可以编辑其邮件。</span><span class="sxs-lookup"><span data-stu-id="df2e7-112">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="df2e7-113">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="df2e7-113">allowUserDeleteMessages</span></span>|<span data-ttu-id="df2e7-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="df2e7-114">Boolean</span></span>|<span data-ttu-id="df2e7-115">如果设置为 true，则用户可以删除其邮件。</span><span class="sxs-lookup"><span data-stu-id="df2e7-115">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="df2e7-116">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="df2e7-116">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="df2e7-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="df2e7-117">Boolean</span></span>|<span data-ttu-id="df2e7-118">如果设置为 true，则所有者可以删除任何邮件。</span><span class="sxs-lookup"><span data-stu-id="df2e7-118">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="df2e7-119">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="df2e7-119">allowTeamMentions</span></span>|<span data-ttu-id="df2e7-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="df2e7-120">Boolean</span></span>|<span data-ttu-id="df2e7-121">如果设置为 true，则允许 @team 提及。</span><span class="sxs-lookup"><span data-stu-id="df2e7-121">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="df2e7-122">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="df2e7-122">allowChannelMentions</span></span>|<span data-ttu-id="df2e7-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="df2e7-123">Boolean</span></span>|<span data-ttu-id="df2e7-124">如果设置为 true，则允许 @channel 提及。</span><span class="sxs-lookup"><span data-stu-id="df2e7-124">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df2e7-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df2e7-125">JSON representation</span></span>

<span data-ttu-id="df2e7-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df2e7-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

