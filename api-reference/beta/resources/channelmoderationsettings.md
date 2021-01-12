---
title: channelModerationSettings 资源类型
description: 用于控制谁可以启动新帖子和回复频道中的帖子。
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b67d55eb57d1a4b554b027270f700cbd590d4416
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796582"
---
# <a name="channelmoderationsettings-resource-type"></a><span data-ttu-id="4f708-103">channelModerationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f708-103">channelModerationSettings resource type</span></span>

<span data-ttu-id="4f708-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f708-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f708-105">在 Microsoft Teams 中，团队所有者可以启用频道审核，以控制谁可以启动新帖子并回复该频道中的帖子。</span><span class="sxs-lookup"><span data-stu-id="4f708-105">In Microsoft Teams, team owners can turn on moderation for a channel to control who can start new posts and reply to posts in that channel.</span></span> <span data-ttu-id="4f708-106">例如，所有者可能希望执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4f708-106">For example, owners might want to do the following:</span></span>

- <span data-ttu-id="4f708-107">仅对通知使用频道。</span><span class="sxs-lookup"><span data-stu-id="4f708-107">Use a channel for announcements only.</span></span>
- <span data-ttu-id="4f708-108">使用频道在课堂团队中讨论，只有教师才能开始新的讨论。</span><span class="sxs-lookup"><span data-stu-id="4f708-108">Use a channel for discussions in a class team where only the teacher can start new discussions.</span></span>
- <span data-ttu-id="4f708-109">使用一个通道解决可通过连接器启动新帖子的现场问题。</span><span class="sxs-lookup"><span data-stu-id="4f708-109">Use a channel for livesite issues where new posts can be started by connectors.</span></span>

<span data-ttu-id="4f708-110">默认情况下，审核是，这意味着常规频道设置适用于团队所有者和团队成员，具有其他控制，以仅允许团队成员或包括来宾在内的每个人启动新 `OFF` 频道帖子。</span><span class="sxs-lookup"><span data-stu-id="4f708-110">By default, moderation is `OFF`, which means that the usual channel settings apply to team owners and team members, with additional control to allow only team members or everyone including guests to start a new channel post.</span></span> <span data-ttu-id="4f708-111">将频道审阅设置为仅允许审阅人启动 `ON` 新帖子，并额外控制团队成员。</span><span class="sxs-lookup"><span data-stu-id="4f708-111">Setting channel moderation to `ON` allows only moderators to start new posts, with additional control for team members.</span></span>

<span data-ttu-id="4f708-112">若要通过 Microsoft Graph API 支持频道审核设置，</span><span class="sxs-lookup"><span data-stu-id="4f708-112">To support channel moderation settings via Microsoft Graph APIs:</span></span>

- <span data-ttu-id="4f708-113">团队成员应能够查询频道审核设置。</span><span class="sxs-lookup"><span data-stu-id="4f708-113">Team members should be able to query channel moderation settings.</span></span>
- <span data-ttu-id="4f708-114">团队所有者应能够设置频道审核设置。</span><span class="sxs-lookup"><span data-stu-id="4f708-114">Team owners should be able to set channel moderation settings.</span></span>

## <a name="properties"></a><span data-ttu-id="4f708-115">属性</span><span class="sxs-lookup"><span data-stu-id="4f708-115">Properties</span></span>
|<span data-ttu-id="4f708-116">属性</span><span class="sxs-lookup"><span data-stu-id="4f708-116">Property</span></span>|<span data-ttu-id="4f708-117">类型</span><span class="sxs-lookup"><span data-stu-id="4f708-117">Type</span></span>|<span data-ttu-id="4f708-118">说明</span><span class="sxs-lookup"><span data-stu-id="4f708-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f708-119">allowNewMessageFromBots</span><span class="sxs-lookup"><span data-stu-id="4f708-119">allowNewMessageFromBots</span></span>|<span data-ttu-id="4f708-120">布尔</span><span class="sxs-lookup"><span data-stu-id="4f708-120">Boolean</span></span>|<span data-ttu-id="4f708-121">指示是否允许机器人发布消息。</span><span class="sxs-lookup"><span data-stu-id="4f708-121">Indicates whether bots are allowed to post messages.</span></span>|
|<span data-ttu-id="4f708-122">allowNewMessageFromConnectors</span><span class="sxs-lookup"><span data-stu-id="4f708-122">allowNewMessageFromConnectors</span></span>|<span data-ttu-id="4f708-123">布尔</span><span class="sxs-lookup"><span data-stu-id="4f708-123">Boolean</span></span>|<span data-ttu-id="4f708-124">指示是否允许连接器发布邮件。</span><span class="sxs-lookup"><span data-stu-id="4f708-124">Indicates whether connectors are allowed to post messages.</span></span>|
|<span data-ttu-id="4f708-125">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="4f708-125">replyRestriction</span></span>|<span data-ttu-id="4f708-126">replyRestriction</span><span class="sxs-lookup"><span data-stu-id="4f708-126">replyRestriction</span></span>|<span data-ttu-id="4f708-127">指示允许谁回复团队频道。</span><span class="sxs-lookup"><span data-stu-id="4f708-127">Indicates who is allowed to reply to the teams channel.</span></span> <span data-ttu-id="4f708-128">可取值为：`everyone`、`authorAndModerators`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4f708-128">Possible values are: `everyone`, `authorAndModerators`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4f708-129">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="4f708-129">userNewMessageRestriction</span></span>|<span data-ttu-id="4f708-130">userNewMessageRestriction</span><span class="sxs-lookup"><span data-stu-id="4f708-130">userNewMessageRestriction</span></span>|<span data-ttu-id="4f708-131">指示允许谁向团队频道发布消息。</span><span class="sxs-lookup"><span data-stu-id="4f708-131">Indicates who is allowed to post messages to teams channel.</span></span> <span data-ttu-id="4f708-132">可取值为：`everyone`、`everyoneExceptGuests`、`moderators`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4f708-132">Possible values are: `everyone`, `everyoneExceptGuests`, `moderators`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f708-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f708-133">JSON representation</span></span>
<span data-ttu-id="4f708-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f708-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelModerationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelModerationSettings",
  "userNewMessageRestriction": "String",
  "replyRestriction": "String",
  "allowNewMessageFromBots": "Boolean",
  "allowNewMessageFromConnectors": "Boolean"
}
```

## <a name="see-also"></a><span data-ttu-id="4f708-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4f708-135">See also</span></span>

- <span data-ttu-id="4f708-136">若要修改频道的审核设置，请参阅更新频道中 [的示例](../api/channel-patch.md)2。</span><span class="sxs-lookup"><span data-stu-id="4f708-136">To modify moderation settings of a channel, see example 2 in [Update channel](../api/channel-patch.md).</span></span>
