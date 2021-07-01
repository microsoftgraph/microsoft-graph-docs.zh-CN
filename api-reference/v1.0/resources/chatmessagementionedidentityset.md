---
title: chatMessageIdentitySet 资源类型
description: 表示聊天@mentioned频道中的消息中的资源资源。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 42369cd75b030ee7c46a6f270fcee548f42338a4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211077"
---
# <a name="chatmessagementionedidentityset-resource-type"></a><span data-ttu-id="f1055-103">chatMessageIdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1055-103">chatMessageMentionedIdentitySet resource type</span></span>

<span data-ttu-id="f1055-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1055-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1055-105">表示用户 (、应用程序或对话) @mentioned聊天或频道中的消息中的资源资源。 [](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="f1055-105">Represents the resource (user, application, or conversation) @mentioned in a [message](../resources/chatmessage.md) in a chat or a channel.</span></span>


<span data-ttu-id="f1055-106">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="f1055-106">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f1055-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1055-107">Properties</span></span>
|<span data-ttu-id="f1055-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1055-108">Property</span></span>|<span data-ttu-id="f1055-109">类型</span><span class="sxs-lookup"><span data-stu-id="f1055-109">Type</span></span>|<span data-ttu-id="f1055-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1055-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1055-111">application</span><span class="sxs-lookup"><span data-stu-id="f1055-111">application</span></span>|[<span data-ttu-id="f1055-112">Identity</span><span class="sxs-lookup"><span data-stu-id="f1055-112">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f1055-113">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="f1055-113">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="f1055-114">如果存在，表示应用程序 (例如，自动程序) @mentioned消息 [中的自动程序](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="f1055-114">If present, represents an application (for example, bot) @mentioned in a [message](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="f1055-115">对话</span><span class="sxs-lookup"><span data-stu-id="f1055-115">conversation</span></span>|[<span data-ttu-id="f1055-116">teamworkConversationIdentity</span><span class="sxs-lookup"><span data-stu-id="f1055-116">teamworkConversationIdentity</span></span>](../resources/teamworkconversationidentity.md)|<span data-ttu-id="f1055-117">如果存在，表示对话 (例如，团队或频道) @mentioned消息 [中](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="f1055-117">If present, represents a conversation (for example, team or channel) @mentioned in a [message](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="f1055-118">设备</span><span class="sxs-lookup"><span data-stu-id="f1055-118">device</span></span>|[<span data-ttu-id="f1055-119">identity</span><span class="sxs-lookup"><span data-stu-id="f1055-119">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f1055-120">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="f1055-120">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="f1055-121">由于不支持在设备上使用@mention使用。</span><span class="sxs-lookup"><span data-stu-id="f1055-121">Not used because it's not supported to @mention devices.</span></span>|
|<span data-ttu-id="f1055-122">user</span><span class="sxs-lookup"><span data-stu-id="f1055-122">user</span></span>|[<span data-ttu-id="f1055-123">identity</span><span class="sxs-lookup"><span data-stu-id="f1055-123">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f1055-124">继承自 [identitySet](../resources/identityset.md)。</span><span class="sxs-lookup"><span data-stu-id="f1055-124">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="f1055-125">如果存在，表示用户@mentioned消息[中显示。](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="f1055-125">If present, represents a user @mentioned in a [message](../resources/chatmessage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1055-126">关系</span><span class="sxs-lookup"><span data-stu-id="f1055-126">Relationships</span></span>
<span data-ttu-id="f1055-127">无。</span><span class="sxs-lookup"><span data-stu-id="f1055-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1055-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1055-128">JSON representation</span></span>
<span data-ttu-id="f1055-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1055-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageMentionedIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  },
  "conversation": {
    "@odata.type": "microsoft.graph.teamworkConversationIdentity"
  }
}
```