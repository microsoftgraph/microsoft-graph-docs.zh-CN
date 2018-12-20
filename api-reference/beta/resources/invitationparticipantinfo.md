---
title: invitationParticipantInfo 资源类型
description: '**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。'
author: VinodRavichandran
ms.openlocfilehash: f833fcd0c555dfcc88da4027313ed7f40da81428
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380483"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="7ba72-103">invitationParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ba72-103">invitationParticipantInfo resource type</span></span>

> <span data-ttu-id="7ba72-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ba72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ba72-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ba72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ba72-106">**InvitationParticipant**用于表示一组标识相关联的对话邀请，并提供其他邀请参数。</span><span class="sxs-lookup"><span data-stu-id="7ba72-106">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="7ba72-107">属性</span><span class="sxs-lookup"><span data-stu-id="7ba72-107">Properties</span></span>

| <span data-ttu-id="7ba72-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ba72-108">Property</span></span>                           | <span data-ttu-id="7ba72-109">类型</span><span class="sxs-lookup"><span data-stu-id="7ba72-109">Type</span></span>                          | <span data-ttu-id="7ba72-110">说明</span><span class="sxs-lookup"><span data-stu-id="7ba72-110">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="7ba72-111">endpointType</span><span class="sxs-lookup"><span data-stu-id="7ba72-111">endpointType</span></span>                       | <span data-ttu-id="7ba72-112">String</span><span class="sxs-lookup"><span data-stu-id="7ba72-112">String</span></span>                        | <span data-ttu-id="7ba72-113">可取值为：`default`、`voicemail`。</span><span class="sxs-lookup"><span data-stu-id="7ba72-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="7ba72-114">identity</span><span class="sxs-lookup"><span data-stu-id="7ba72-114">identity</span></span>                           | [<span data-ttu-id="7ba72-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="7ba72-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="7ba72-116">与此邀请关联[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="7ba72-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="7ba72-117">languageId</span><span class="sxs-lookup"><span data-stu-id="7ba72-117">languageId</span></span>                         | <span data-ttu-id="7ba72-118">字符串</span><span class="sxs-lookup"><span data-stu-id="7ba72-118">String</span></span>                        | <span data-ttu-id="7ba72-119">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="7ba72-119">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="7ba72-120">区域</span><span class="sxs-lookup"><span data-stu-id="7ba72-120">region</span></span>                             | <span data-ttu-id="7ba72-121">字符串</span><span class="sxs-lookup"><span data-stu-id="7ba72-121">String</span></span>                        | <span data-ttu-id="7ba72-122">参与者的区域。</span><span class="sxs-lookup"><span data-stu-id="7ba72-122">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="7ba72-123">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="7ba72-123">replacesCallId</span></span>                     | <span data-ttu-id="7ba72-124">字符串</span><span class="sxs-lookup"><span data-stu-id="7ba72-124">String</span></span>                        | <span data-ttu-id="7ba72-125">可选。</span><span class="sxs-lookup"><span data-stu-id="7ba72-125">Optional.</span></span> <span data-ttu-id="7ba72-126">呼叫的目标 idenity 目前的一部分。</span><span class="sxs-lookup"><span data-stu-id="7ba72-126">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="7ba72-127">一旦添加参与者，此呼叫将被丢弃。</span><span class="sxs-lookup"><span data-stu-id="7ba72-127">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ba72-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ba72-128">JSON representation</span></span>

<span data-ttu-id="7ba72-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ba72-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
