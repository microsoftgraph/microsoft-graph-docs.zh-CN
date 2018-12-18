---
title: teamMessagingSettings 资源类型
description: 要配置的消息设置和团队中的提及。
author: nkramer
ms.openlocfilehash: 387c2e3ccedc6f11f17d4868b1b0d3eaf67624fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304548"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="24829-103">teamMessagingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="24829-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="24829-104">要配置的消息设置和[团队](team.md)中的提及。</span><span class="sxs-lookup"><span data-stu-id="24829-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="24829-105">属性</span><span class="sxs-lookup"><span data-stu-id="24829-105">Properties</span></span>
| <span data-ttu-id="24829-106">属性</span><span class="sxs-lookup"><span data-stu-id="24829-106">Property</span></span>     | <span data-ttu-id="24829-107">类型</span><span class="sxs-lookup"><span data-stu-id="24829-107">Type</span></span>   |<span data-ttu-id="24829-108">说明</span><span class="sxs-lookup"><span data-stu-id="24829-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24829-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="24829-109">allowUserEditMessages</span></span>|<span data-ttu-id="24829-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="24829-110">Boolean</span></span>|<span data-ttu-id="24829-111">如果设置为 true，则用户可以编辑他们的邮件。</span><span class="sxs-lookup"><span data-stu-id="24829-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="24829-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="24829-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="24829-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="24829-113">Boolean</span></span>|<span data-ttu-id="24829-114">如果设置为 true，则用户可以删除其邮件。</span><span class="sxs-lookup"><span data-stu-id="24829-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="24829-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="24829-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="24829-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="24829-116">Boolean</span></span>|<span data-ttu-id="24829-117">如果设置为 true，则所有者可以删除任何消息。</span><span class="sxs-lookup"><span data-stu-id="24829-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="24829-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="24829-118">allowTeamMentions</span></span>|<span data-ttu-id="24829-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="24829-119">Boolean</span></span>|<span data-ttu-id="24829-120">如果设置为 true，允许提及的 @team。</span><span class="sxs-lookup"><span data-stu-id="24829-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="24829-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="24829-121">allowChannelMentions</span></span>|<span data-ttu-id="24829-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="24829-122">Boolean</span></span>|<span data-ttu-id="24829-123">如果设置为 true，允许提及的 @channel。</span><span class="sxs-lookup"><span data-stu-id="24829-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24829-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24829-124">JSON representation</span></span>

<span data-ttu-id="24829-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24829-125">The following is a JSON representation of the resource.</span></span>

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
