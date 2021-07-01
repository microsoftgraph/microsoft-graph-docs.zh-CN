---
title: chatViewpoint 资源类型
description: 表示聊天的用户特定属性。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca6a542903aae7b203c6183a25dd99889b97f275
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236295"
---
# <a name="chatviewpoint-resource-type"></a><span data-ttu-id="f7cd8-103">chatViewpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7cd8-103">chatViewpoint resource type</span></span>

<span data-ttu-id="f7cd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7cd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7cd8-105">表示聊天的特定于用户 [的属性](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="f7cd8-105">Represents user-specific properties of a [chat](../resources/chat.md).</span></span> <span data-ttu-id="f7cd8-106">这些属性可能会根据 API 调用方的身份而更改。</span><span class="sxs-lookup"><span data-stu-id="f7cd8-106">These properties might change based on who the caller of the API is.</span></span>

> <span data-ttu-id="f7cd8-107">**注意：** 目前，仅 [列表聊天](../api/chat-list.md) 操作支持 **chatViewpoint**。</span><span class="sxs-lookup"><span data-stu-id="f7cd8-107">**Note:** Currently, only the [list chats](../api/chat-list.md) operation supports **chatViewpoint**.</span></span>

## <a name="properties"></a><span data-ttu-id="f7cd8-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7cd8-108">Properties</span></span>
|<span data-ttu-id="f7cd8-109">属性</span><span class="sxs-lookup"><span data-stu-id="f7cd8-109">Property</span></span>|<span data-ttu-id="f7cd8-110">类型</span><span class="sxs-lookup"><span data-stu-id="f7cd8-110">Type</span></span>|<span data-ttu-id="f7cd8-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7cd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7cd8-112">lastMessageReadDateTime</span><span class="sxs-lookup"><span data-stu-id="f7cd8-112">lastMessageReadDateTime</span></span>|<span data-ttu-id="f7cd8-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7cd8-113">DateTimeOffset</span></span>|<span data-ttu-id="f7cd8-114">表示直到呼叫用户已读取特定聊天中的 [chatMessages](../resources/chatmessage.md) 的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f7cd8-114">Represents the dateTime up until which the calling user has read [chatMessages](../resources/chatmessage.md) in a specific chat.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7cd8-115">关系</span><span class="sxs-lookup"><span data-stu-id="f7cd8-115">Relationships</span></span>
<span data-ttu-id="f7cd8-116">无。</span><span class="sxs-lookup"><span data-stu-id="f7cd8-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7cd8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7cd8-117">JSON representation</span></span>
<span data-ttu-id="f7cd8-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7cd8-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatViewpoint",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

