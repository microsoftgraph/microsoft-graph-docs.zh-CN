---
title: teamMessagingSettings 资源类型
description: 要配置的消息设置和团队中的提及。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06aca84355a07052dcea316145dfff437eee743b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848256"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="22f90-103">teamMessagingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="22f90-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="22f90-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22f90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22f90-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22f90-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22f90-106">要配置的消息设置和[团队](team.md)中的提及。</span><span class="sxs-lookup"><span data-stu-id="22f90-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="22f90-107">属性</span><span class="sxs-lookup"><span data-stu-id="22f90-107">Properties</span></span>
| <span data-ttu-id="22f90-108">属性</span><span class="sxs-lookup"><span data-stu-id="22f90-108">Property</span></span>     | <span data-ttu-id="22f90-109">类型</span><span class="sxs-lookup"><span data-stu-id="22f90-109">Type</span></span>   |<span data-ttu-id="22f90-110">Description</span><span class="sxs-lookup"><span data-stu-id="22f90-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22f90-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="22f90-111">allowUserEditMessages</span></span>|<span data-ttu-id="22f90-112">布尔</span><span class="sxs-lookup"><span data-stu-id="22f90-112">Boolean</span></span>|<span data-ttu-id="22f90-113">如果设置为 true，则用户可以编辑他们的邮件。</span><span class="sxs-lookup"><span data-stu-id="22f90-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="22f90-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="22f90-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="22f90-115">布尔</span><span class="sxs-lookup"><span data-stu-id="22f90-115">Boolean</span></span>|<span data-ttu-id="22f90-116">如果设置为 true，则用户可以删除其邮件。</span><span class="sxs-lookup"><span data-stu-id="22f90-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="22f90-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="22f90-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="22f90-118">布尔</span><span class="sxs-lookup"><span data-stu-id="22f90-118">Boolean</span></span>|<span data-ttu-id="22f90-119">如果设置为 true，则所有者可以删除任何消息。</span><span class="sxs-lookup"><span data-stu-id="22f90-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="22f90-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="22f90-120">allowTeamMentions</span></span>|<span data-ttu-id="22f90-121">布尔</span><span class="sxs-lookup"><span data-stu-id="22f90-121">Boolean</span></span>|<span data-ttu-id="22f90-122">如果设置为 true，允许提及的 @team。</span><span class="sxs-lookup"><span data-stu-id="22f90-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="22f90-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="22f90-123">allowChannelMentions</span></span>|<span data-ttu-id="22f90-124">布尔</span><span class="sxs-lookup"><span data-stu-id="22f90-124">Boolean</span></span>|<span data-ttu-id="22f90-125">如果设置为 true，允许提及的 @channel。</span><span class="sxs-lookup"><span data-stu-id="22f90-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22f90-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22f90-126">JSON representation</span></span>

<span data-ttu-id="22f90-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22f90-127">The following is a JSON representation of the resource.</span></span>

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
