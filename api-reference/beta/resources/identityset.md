---
author: JeremyKelley
description: 了解 identityset 资源是标识资源的键控集合。
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 60fdb901ecd74f3826604d139cad71d9d0844221
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966756"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="bace4-103">了解 identityset 资源类型</span><span class="sxs-lookup"><span data-stu-id="bace4-103">identitySet resource type</span></span>

<span data-ttu-id="bace4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bace4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bace4-105">**了解 identityset**资源是[标识](identity.md)资源的键控集合。</span><span class="sxs-lookup"><span data-stu-id="bace4-105">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="bace4-106">它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="bace4-106">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bace4-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bace4-107">JSON representation</span></span>

<span data-ttu-id="bace4-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bace4-108">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="bace4-109">属性</span><span class="sxs-lookup"><span data-stu-id="bace4-109">Properties</span></span>

| <span data-ttu-id="bace4-110">属性</span><span class="sxs-lookup"><span data-stu-id="bace4-110">Property</span></span>    | <span data-ttu-id="bace4-111">类型</span><span class="sxs-lookup"><span data-stu-id="bace4-111">Type</span></span>                    | <span data-ttu-id="bace4-112">说明</span><span class="sxs-lookup"><span data-stu-id="bace4-112">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="bace4-113">application</span><span class="sxs-lookup"><span data-stu-id="bace4-113">application</span></span> | [<span data-ttu-id="bace4-114">标识</span><span class="sxs-lookup"><span data-stu-id="bace4-114">Identity</span></span>](identity.md) | <span data-ttu-id="bace4-p101">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="bace4-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="bace4-117">对话</span><span class="sxs-lookup"><span data-stu-id="bace4-117">conversation</span></span>| [<span data-ttu-id="bace4-118">标识</span><span class="sxs-lookup"><span data-stu-id="bace4-118">Identity</span></span>](identity.md) | <span data-ttu-id="bace4-119">可选。</span><span class="sxs-lookup"><span data-stu-id="bace4-119">Optional.</span></span> <span data-ttu-id="bace4-120">与此操作关联的团队或频道。</span><span class="sxs-lookup"><span data-stu-id="bace4-120">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="bace4-121">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="bace4-121">conversationIdentityType</span></span>| [<span data-ttu-id="bace4-122">标识</span><span class="sxs-lookup"><span data-stu-id="bace4-122">Identity</span></span>](identity.md) | <span data-ttu-id="bace4-123">可选。</span><span class="sxs-lookup"><span data-stu-id="bace4-123">Optional.</span></span> <span data-ttu-id="bace4-124">指示 **会话** 属性是否标识团队或频道。</span><span class="sxs-lookup"><span data-stu-id="bace4-124">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="bace4-125">设备</span><span class="sxs-lookup"><span data-stu-id="bace4-125">device</span></span>      | [<span data-ttu-id="bace4-126">标识</span><span class="sxs-lookup"><span data-stu-id="bace4-126">Identity</span></span>](identity.md) | <span data-ttu-id="bace4-p104">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="bace4-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="bace4-129">phone</span><span class="sxs-lookup"><span data-stu-id="bace4-129">phone</span></span>       | [<span data-ttu-id="bace4-130">identity</span><span class="sxs-lookup"><span data-stu-id="bace4-130">identity</span></span>](identity.md) | <span data-ttu-id="bace4-131">可选。</span><span class="sxs-lookup"><span data-stu-id="bace4-131">Optional.</span></span> <span data-ttu-id="bace4-132">与此操作关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="bace4-132">The phone number associated with this action.</span></span> |
| <span data-ttu-id="bace4-133">用户</span><span class="sxs-lookup"><span data-stu-id="bace4-133">user</span></span>        | [<span data-ttu-id="bace4-134">标识</span><span class="sxs-lookup"><span data-stu-id="bace4-134">Identity</span></span>](identity.md) | <span data-ttu-id="bace4-p106">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="bace4-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="bace4-137">注解</span><span class="sxs-lookup"><span data-stu-id="bace4-137">Remarks</span></span> 

<span data-ttu-id="bace4-138">有关**了解 identityset**资源的使用情况，请参阅[Call](call.md) 。</span><span class="sxs-lookup"><span data-stu-id="bace4-138">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->


