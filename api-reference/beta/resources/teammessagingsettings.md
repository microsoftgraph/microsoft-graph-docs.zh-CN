---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553944"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="4f256-103">teamMessagingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f256-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="4f256-104">用于配置[团队](team.md)中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="4f256-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4f256-105">属性</span><span class="sxs-lookup"><span data-stu-id="4f256-105">Properties</span></span>
| <span data-ttu-id="4f256-106">属性</span><span class="sxs-lookup"><span data-stu-id="4f256-106">Property</span></span>     | <span data-ttu-id="4f256-107">类型</span><span class="sxs-lookup"><span data-stu-id="4f256-107">Type</span></span>   |<span data-ttu-id="4f256-108">说明</span><span class="sxs-lookup"><span data-stu-id="4f256-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f256-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="4f256-109">allowUserEditMessages</span></span>|<span data-ttu-id="4f256-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="4f256-110">Boolean</span></span>|<span data-ttu-id="4f256-111">如果设置为 true, 则用户可以编辑其邮件。</span><span class="sxs-lookup"><span data-stu-id="4f256-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="4f256-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="4f256-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="4f256-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="4f256-113">Boolean</span></span>|<span data-ttu-id="4f256-114">如果设置为 true, 则用户可以删除其邮件。</span><span class="sxs-lookup"><span data-stu-id="4f256-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="4f256-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="4f256-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="4f256-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="4f256-116">Boolean</span></span>|<span data-ttu-id="4f256-117">如果设置为 true, 则所有者可以删除任何邮件。</span><span class="sxs-lookup"><span data-stu-id="4f256-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="4f256-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="4f256-118">allowTeamMentions</span></span>|<span data-ttu-id="4f256-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="4f256-119">Boolean</span></span>|<span data-ttu-id="4f256-120">如果设置为 true, 则允许 @team 提及。</span><span class="sxs-lookup"><span data-stu-id="4f256-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="4f256-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="4f256-121">allowChannelMentions</span></span>|<span data-ttu-id="4f256-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="4f256-122">Boolean</span></span>|<span data-ttu-id="4f256-123">如果设置为 true, 则允许 @channel 提及。</span><span class="sxs-lookup"><span data-stu-id="4f256-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f256-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f256-124">JSON representation</span></span>

<span data-ttu-id="4f256-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f256-125">The following is a JSON representation of the resource.</span></span>

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
