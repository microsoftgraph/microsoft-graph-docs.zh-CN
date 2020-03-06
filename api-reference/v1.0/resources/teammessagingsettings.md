---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e742dd0e785a94b33a57e55b50a00aab0c207ab4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533521"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="f0680-103">teamMessagingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0680-103">teamMessagingSettings resource type</span></span>

<span data-ttu-id="f0680-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0680-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f0680-105">用于配置[团队](team.md)中的消息传递和提及的设置。</span><span class="sxs-lookup"><span data-stu-id="f0680-105">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0680-106">属性</span><span class="sxs-lookup"><span data-stu-id="f0680-106">Properties</span></span>
| <span data-ttu-id="f0680-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0680-107">Property</span></span>     | <span data-ttu-id="f0680-108">类型</span><span class="sxs-lookup"><span data-stu-id="f0680-108">Type</span></span>   |<span data-ttu-id="f0680-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0680-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0680-110">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="f0680-110">allowUserEditMessages</span></span>|<span data-ttu-id="f0680-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0680-111">Boolean</span></span>|<span data-ttu-id="f0680-112">如果设置为 true，则用户可以编辑其邮件。</span><span class="sxs-lookup"><span data-stu-id="f0680-112">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="f0680-113">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="f0680-113">allowUserDeleteMessages</span></span>|<span data-ttu-id="f0680-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0680-114">Boolean</span></span>|<span data-ttu-id="f0680-115">如果设置为 true，则用户可以删除其邮件。</span><span class="sxs-lookup"><span data-stu-id="f0680-115">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="f0680-116">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="f0680-116">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="f0680-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0680-117">Boolean</span></span>|<span data-ttu-id="f0680-118">如果设置为 true，则所有者可以删除任何邮件。</span><span class="sxs-lookup"><span data-stu-id="f0680-118">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="f0680-119">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="f0680-119">allowTeamMentions</span></span>|<span data-ttu-id="f0680-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0680-120">Boolean</span></span>|<span data-ttu-id="f0680-121">如果设置为 true，则允许 @team 提及。</span><span class="sxs-lookup"><span data-stu-id="f0680-121">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="f0680-122">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="f0680-122">allowChannelMentions</span></span>|<span data-ttu-id="f0680-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0680-123">Boolean</span></span>|<span data-ttu-id="f0680-124">如果设置为 true，则允许 @channel 提及。</span><span class="sxs-lookup"><span data-stu-id="f0680-124">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0680-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0680-125">JSON representation</span></span>

<span data-ttu-id="f0680-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0680-126">The following is a JSON representation of the resource.</span></span>

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
