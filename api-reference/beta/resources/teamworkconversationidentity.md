---
title: teamworkConversationIdentity 资源类型
description: 表示对话中的Microsoft Teams。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 84e936368b7cc4589b7611b15cf310f92b055e2a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211219"
---
# <a name="teamworkconversationidentity-resource-type"></a><span data-ttu-id="df58c-103">teamworkConversationIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="df58c-103">teamworkConversationIdentity resource type</span></span>

<span data-ttu-id="df58c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df58c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df58c-105">代表 **用户 (** 聊天、团队或频道) 对话Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="df58c-105">Represents a **conversation** (chat, team, or channel) in Microsoft Teams.</span></span>

<span data-ttu-id="df58c-106">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="df58c-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df58c-107">属性</span><span class="sxs-lookup"><span data-stu-id="df58c-107">Properties</span></span>
|<span data-ttu-id="df58c-108">属性</span><span class="sxs-lookup"><span data-stu-id="df58c-108">Property</span></span>|<span data-ttu-id="df58c-109">类型</span><span class="sxs-lookup"><span data-stu-id="df58c-109">Type</span></span>|<span data-ttu-id="df58c-110">说明</span><span class="sxs-lookup"><span data-stu-id="df58c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df58c-111">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="df58c-111">conversationIdentityType</span></span>|<span data-ttu-id="df58c-112">teamworkConversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="df58c-112">teamworkConversationIdentityType</span></span>|<span data-ttu-id="df58c-113">对话类型。</span><span class="sxs-lookup"><span data-stu-id="df58c-113">Type of conversation.</span></span> <span data-ttu-id="df58c-114">可能的值是 `team` ：、 `channel` 和 `chat` 。</span><span class="sxs-lookup"><span data-stu-id="df58c-114">Possible values are: `team`, `channel`, and `chat`.</span></span>|
|<span data-ttu-id="df58c-115">displayName</span><span class="sxs-lookup"><span data-stu-id="df58c-115">displayName</span></span>|<span data-ttu-id="df58c-116">String</span><span class="sxs-lookup"><span data-stu-id="df58c-116">String</span></span>|<span data-ttu-id="df58c-117">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="df58c-117">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="df58c-118">对话的显示名称。</span><span class="sxs-lookup"><span data-stu-id="df58c-118">Display name of the conversation.</span></span> <span data-ttu-id="df58c-119">可选。</span><span class="sxs-lookup"><span data-stu-id="df58c-119">Optional.</span></span>|
|<span data-ttu-id="df58c-120">id</span><span class="sxs-lookup"><span data-stu-id="df58c-120">id</span></span>|<span data-ttu-id="df58c-121">String</span><span class="sxs-lookup"><span data-stu-id="df58c-121">String</span></span>|<span data-ttu-id="df58c-122">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="df58c-122">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="df58c-123">对话的 ID。</span><span class="sxs-lookup"><span data-stu-id="df58c-123">ID of the conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df58c-124">关系</span><span class="sxs-lookup"><span data-stu-id="df58c-124">Relationships</span></span>
<span data-ttu-id="df58c-125">无。</span><span class="sxs-lookup"><span data-stu-id="df58c-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df58c-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df58c-126">JSON representation</span></span>
<span data-ttu-id="df58c-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df58c-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConversationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConversationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "conversationIdentityType": "String"
}
```

