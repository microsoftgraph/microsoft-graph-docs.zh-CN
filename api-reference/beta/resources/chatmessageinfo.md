---
title: chatMessageInfo 资源类型
description: 表示 chatMessage 资源的预览。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dc03ee6743aa8115f5a231b3766cc2d6c3d5537b
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236292"
---
# <a name="chatmessageinfo-resource-type"></a><span data-ttu-id="92749-103">chatMessageInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="92749-103">chatMessageInfo resource type</span></span>

<span data-ttu-id="92749-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92749-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92749-105">表示 [chatMessage 资源的](../resources/chatmessage.md) 预览。</span><span class="sxs-lookup"><span data-stu-id="92749-105">Represents a preview of a [chatMessage](../resources/chatmessage.md) resource.</span></span> <span data-ttu-id="92749-106">此对象只能作为聊天列表的一 [部分获取](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="92749-106">This object can only be fetched as part of a list of [chats](../resources/chat.md).</span></span>

## <a name="properties"></a><span data-ttu-id="92749-107">属性</span><span class="sxs-lookup"><span data-stu-id="92749-107">Properties</span></span>
|<span data-ttu-id="92749-108">属性</span><span class="sxs-lookup"><span data-stu-id="92749-108">Property</span></span>|<span data-ttu-id="92749-109">类型</span><span class="sxs-lookup"><span data-stu-id="92749-109">Type</span></span>|<span data-ttu-id="92749-110">说明</span><span class="sxs-lookup"><span data-stu-id="92749-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92749-111">body</span><span class="sxs-lookup"><span data-stu-id="92749-111">body</span></span>|[<span data-ttu-id="92749-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="92749-112">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="92749-113">[chatMessage 的正文](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="92749-113">Body of the [chatMessage](../resources/chatmessage.md).</span></span> <span data-ttu-id="92749-114">即使对象不返回@mentions和附件，这仍将包含@mentions标记。</span><span class="sxs-lookup"><span data-stu-id="92749-114">This will still contain markers for @mentions and attachments even though the object does not return @mentions and attachments.</span></span>|
|<span data-ttu-id="92749-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92749-115">createdDateTime</span></span>|<span data-ttu-id="92749-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92749-116">DateTimeOffset</span></span>|<span data-ttu-id="92749-117">表示创建邮件的时间的日期时间对象。</span><span class="sxs-lookup"><span data-stu-id="92749-117">Date time object representing the time at which message was created.</span></span>|
|<span data-ttu-id="92749-118">起始数量</span><span class="sxs-lookup"><span data-stu-id="92749-118">from</span></span>|[<span data-ttu-id="92749-119">chatMessageFromIdentitySet</span><span class="sxs-lookup"><span data-stu-id="92749-119">chatMessageFromIdentitySet</span></span>](../resources/chatmessagefromidentityset.md)|<span data-ttu-id="92749-120">有关邮件发件人的信息。</span><span class="sxs-lookup"><span data-stu-id="92749-120">Information about the sender of the message.</span></span>|
|<span data-ttu-id="92749-121">id</span><span class="sxs-lookup"><span data-stu-id="92749-121">id</span></span>|<span data-ttu-id="92749-122">String</span><span class="sxs-lookup"><span data-stu-id="92749-122">String</span></span>|<span data-ttu-id="92749-123">[chatMessage](../resources/chatmessage.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="92749-123">ID of the [chatMessage](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="92749-124">isDeleted</span><span class="sxs-lookup"><span data-stu-id="92749-124">isDeleted</span></span>|<span data-ttu-id="92749-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="92749-125">Boolean</span></span>|<span data-ttu-id="92749-126">如果设置为 `true` ，则原始邮件已删除。</span><span class="sxs-lookup"><span data-stu-id="92749-126">If set to `true`, the original message has been deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92749-127">关系</span><span class="sxs-lookup"><span data-stu-id="92749-127">Relationships</span></span>
<span data-ttu-id="92749-128">无。</span><span class="sxs-lookup"><span data-stu-id="92749-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92749-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92749-129">JSON representation</span></span>
<span data-ttu-id="92749-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92749-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageInfo",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "from": {
    "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
  },
  "createdDateTime": "String (timestamp)",
  "isDeleted": "Boolean"
}
```

## <a name="see-also"></a><span data-ttu-id="92749-131">另请参阅</span><span class="sxs-lookup"><span data-stu-id="92749-131">See also</span></span>

- [<span data-ttu-id="92749-132">聊天</span><span class="sxs-lookup"><span data-stu-id="92749-132">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="92749-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="92749-133">chatMessage</span></span>](../resources/chatmessage.md)

