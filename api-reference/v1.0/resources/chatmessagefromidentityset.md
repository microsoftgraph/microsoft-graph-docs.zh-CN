---
title: chatMessageFromIdentitySet 资源类型
description: 表示聊天或频道中消息的发送方。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 30b8c8add62c94ff16fe5e560a78ec5c9c95627d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211075"
---
# <a name="chatmessagefromidentityset-resource-type"></a><span data-ttu-id="3201a-103">chatMessageFromIdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="3201a-103">chatMessageFromIdentitySet resource type</span></span>

<span data-ttu-id="3201a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3201a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3201a-105">表示聊天 [或](../resources/chatmessage.md) 频道中消息的发送方。</span><span class="sxs-lookup"><span data-stu-id="3201a-105">Represents the sender of a [message](../resources/chatmessage.md) in a chat or a channel.</span></span> <span data-ttu-id="3201a-106">此对象可能适用于内部系统已删除或发送Microsoft Teams的邮件;例如，用于添加 `null` 成员的事件消息。</span><span class="sxs-lookup"><span data-stu-id="3201a-106">This object may be `null` for a message that has been deleted or sent by the Microsoft Teams internal system; for example, event messages for addition of members.</span></span>


<span data-ttu-id="3201a-107">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="3201a-107">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3201a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3201a-108">Properties</span></span>
|<span data-ttu-id="3201a-109">属性</span><span class="sxs-lookup"><span data-stu-id="3201a-109">Property</span></span>|<span data-ttu-id="3201a-110">类型</span><span class="sxs-lookup"><span data-stu-id="3201a-110">Type</span></span>|<span data-ttu-id="3201a-111">说明</span><span class="sxs-lookup"><span data-stu-id="3201a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3201a-112">application</span><span class="sxs-lookup"><span data-stu-id="3201a-112">application</span></span>|[<span data-ttu-id="3201a-113">Identity</span><span class="sxs-lookup"><span data-stu-id="3201a-113">identity</span></span>](../resources/identity.md)|<span data-ttu-id="3201a-114">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="3201a-114">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="3201a-115">如果存在，表示应用程序 (例如，自动程序) 发送消息。</span><span class="sxs-lookup"><span data-stu-id="3201a-115">If present, represents the application (for instance, bot) that sent the message.</span></span>|
|<span data-ttu-id="3201a-116">设备</span><span class="sxs-lookup"><span data-stu-id="3201a-116">device</span></span>|[<span data-ttu-id="3201a-117">identity</span><span class="sxs-lookup"><span data-stu-id="3201a-117">identity</span></span>](../resources/identity.md)|<span data-ttu-id="3201a-118">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="3201a-118">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="3201a-119">未使用。</span><span class="sxs-lookup"><span data-stu-id="3201a-119">Not used.</span></span>|
|<span data-ttu-id="3201a-120">user</span><span class="sxs-lookup"><span data-stu-id="3201a-120">user</span></span>|[<span data-ttu-id="3201a-121">identity</span><span class="sxs-lookup"><span data-stu-id="3201a-121">identity</span></span>](../resources/identity.md)|<span data-ttu-id="3201a-122">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="3201a-122">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="3201a-123">如果存在，表示发送消息的用户。</span><span class="sxs-lookup"><span data-stu-id="3201a-123">If present, represents the user that sent the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3201a-124">关系</span><span class="sxs-lookup"><span data-stu-id="3201a-124">Relationships</span></span>
<span data-ttu-id="3201a-125">无。</span><span class="sxs-lookup"><span data-stu-id="3201a-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3201a-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3201a-126">JSON representation</span></span>
<span data-ttu-id="3201a-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3201a-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageFromIdentitySet",
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

