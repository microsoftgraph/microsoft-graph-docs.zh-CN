---
title: teamMessagingSettings 资源类型
description: 要配置的消息设置和团队中的提及。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: df80fbb828a400e736b2e8c3b73f949fe6bfd1ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878377"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="75d90-103">teamMessagingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="75d90-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="75d90-104">要配置的消息设置和[团队](team.md)中的提及。</span><span class="sxs-lookup"><span data-stu-id="75d90-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="75d90-105">属性</span><span class="sxs-lookup"><span data-stu-id="75d90-105">Properties</span></span>
| <span data-ttu-id="75d90-106">属性</span><span class="sxs-lookup"><span data-stu-id="75d90-106">Property</span></span>     | <span data-ttu-id="75d90-107">类型</span><span class="sxs-lookup"><span data-stu-id="75d90-107">Type</span></span>   |<span data-ttu-id="75d90-108">Description</span><span class="sxs-lookup"><span data-stu-id="75d90-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75d90-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="75d90-109">allowUserEditMessages</span></span>|<span data-ttu-id="75d90-110">布尔</span><span class="sxs-lookup"><span data-stu-id="75d90-110">Boolean</span></span>|<span data-ttu-id="75d90-111">如果设置为 true，则用户可以编辑他们的邮件。</span><span class="sxs-lookup"><span data-stu-id="75d90-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="75d90-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="75d90-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="75d90-113">布尔</span><span class="sxs-lookup"><span data-stu-id="75d90-113">Boolean</span></span>|<span data-ttu-id="75d90-114">如果设置为 true，则用户可以删除其邮件。</span><span class="sxs-lookup"><span data-stu-id="75d90-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="75d90-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="75d90-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="75d90-116">布尔</span><span class="sxs-lookup"><span data-stu-id="75d90-116">Boolean</span></span>|<span data-ttu-id="75d90-117">如果设置为 true，则所有者可以删除任何消息。</span><span class="sxs-lookup"><span data-stu-id="75d90-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="75d90-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="75d90-118">allowTeamMentions</span></span>|<span data-ttu-id="75d90-119">布尔</span><span class="sxs-lookup"><span data-stu-id="75d90-119">Boolean</span></span>|<span data-ttu-id="75d90-120">如果设置为 true，允许提及的 @team。</span><span class="sxs-lookup"><span data-stu-id="75d90-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="75d90-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="75d90-121">allowChannelMentions</span></span>|<span data-ttu-id="75d90-122">布尔</span><span class="sxs-lookup"><span data-stu-id="75d90-122">Boolean</span></span>|<span data-ttu-id="75d90-123">如果设置为 true，允许提及的 @channel。</span><span class="sxs-lookup"><span data-stu-id="75d90-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75d90-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75d90-124">JSON representation</span></span>

<span data-ttu-id="75d90-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75d90-125">The following is a JSON representation of the resource.</span></span>

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
