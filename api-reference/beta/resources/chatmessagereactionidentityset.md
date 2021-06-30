---
title: chatMessageReactionIdentitySet 资源类型
description: 表示对聊天或频道中的消息做出响应的用户。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 032b335656d768f505cdb673b56ef0955cf9ed58
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211225"
---
# <a name="chatmessagereactionidentityset-resource-type"></a><span data-ttu-id="5de2f-103">chatMessageReactionIdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="5de2f-103">chatMessageReactionIdentitySet resource type</span></span>

<span data-ttu-id="5de2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5de2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5de2f-105">表示 **对** 聊天 [或频道中](../resources/chatmessage.md) 的消息做出响应的用户。</span><span class="sxs-lookup"><span data-stu-id="5de2f-105">Represents a **user** that reacted to a [message](../resources/chatmessage.md) in a chat or a channel.</span></span> <span data-ttu-id="5de2f-106">仅 `user` 属性具有值。</span><span class="sxs-lookup"><span data-stu-id="5de2f-106">Only the `user` property has a value.</span></span>


<span data-ttu-id="5de2f-107">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="5de2f-107">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5de2f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5de2f-108">Properties</span></span>
|<span data-ttu-id="5de2f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5de2f-109">Property</span></span>|<span data-ttu-id="5de2f-110">类型</span><span class="sxs-lookup"><span data-stu-id="5de2f-110">Type</span></span>|<span data-ttu-id="5de2f-111">说明</span><span class="sxs-lookup"><span data-stu-id="5de2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5de2f-112">application</span><span class="sxs-lookup"><span data-stu-id="5de2f-112">application</span></span>|[<span data-ttu-id="5de2f-113">Identity</span><span class="sxs-lookup"><span data-stu-id="5de2f-113">identity</span></span>](../resources/identity.md)|<span data-ttu-id="5de2f-114">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="5de2f-114">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="5de2f-115">未设置，因为应用程序无法对消息做出反应。</span><span class="sxs-lookup"><span data-stu-id="5de2f-115">Not set because applications can't react to messages.</span></span>|
|<span data-ttu-id="5de2f-116">设备</span><span class="sxs-lookup"><span data-stu-id="5de2f-116">device</span></span>|[<span data-ttu-id="5de2f-117">identity</span><span class="sxs-lookup"><span data-stu-id="5de2f-117">identity</span></span>](../resources/identity.md)|<span data-ttu-id="5de2f-118">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="5de2f-118">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="5de2f-119">未设置，因为设备无法对消息做出反应。</span><span class="sxs-lookup"><span data-stu-id="5de2f-119">Not set because devices can't react to messages.</span></span>|
|<span data-ttu-id="5de2f-120">user</span><span class="sxs-lookup"><span data-stu-id="5de2f-120">user</span></span>|[<span data-ttu-id="5de2f-121">identity</span><span class="sxs-lookup"><span data-stu-id="5de2f-121">identity</span></span>](../resources/identity.md)|<span data-ttu-id="5de2f-122">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="5de2f-122">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="5de2f-123">有关对邮件做出响应的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5de2f-123">Details about the user who reacted to the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5de2f-124">关系</span><span class="sxs-lookup"><span data-stu-id="5de2f-124">Relationships</span></span>
<span data-ttu-id="5de2f-125">无。</span><span class="sxs-lookup"><span data-stu-id="5de2f-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5de2f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5de2f-126">JSON representation</span></span>
<span data-ttu-id="5de2f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5de2f-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageReactionIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

