---
author: JeremyKelley
description: 了解 identityset 资源是标识资源的键控集合。
ms.date: 09/10/2017
title: 了解 identityset
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c43981c1f7e79567afe901217030a0b5abed6f53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006288"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="0505d-103">了解 identityset 资源类型</span><span class="sxs-lookup"><span data-stu-id="0505d-103">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0505d-104">**了解 identityset**资源是[标识](identity.md)资源的键控集合。</span><span class="sxs-lookup"><span data-stu-id="0505d-104">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="0505d-105">它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="0505d-105">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0505d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0505d-106">JSON representation</span></span>

<span data-ttu-id="0505d-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0505d-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0505d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0505d-108">Properties</span></span>

| <span data-ttu-id="0505d-109">属性</span><span class="sxs-lookup"><span data-stu-id="0505d-109">Property</span></span>    | <span data-ttu-id="0505d-110">类型</span><span class="sxs-lookup"><span data-stu-id="0505d-110">Type</span></span>                    | <span data-ttu-id="0505d-111">说明</span><span class="sxs-lookup"><span data-stu-id="0505d-111">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="0505d-112">application</span><span class="sxs-lookup"><span data-stu-id="0505d-112">application</span></span> | [<span data-ttu-id="0505d-113">标识</span><span class="sxs-lookup"><span data-stu-id="0505d-113">Identity</span></span>](identity.md) | <span data-ttu-id="0505d-p101">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0505d-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="0505d-116">对话</span><span class="sxs-lookup"><span data-stu-id="0505d-116">conversation</span></span>| [<span data-ttu-id="0505d-117">标识</span><span class="sxs-lookup"><span data-stu-id="0505d-117">Identity</span></span>](identity.md) | <span data-ttu-id="0505d-118">可选。</span><span class="sxs-lookup"><span data-stu-id="0505d-118">Optional.</span></span> <span data-ttu-id="0505d-119">与此操作关联的团队或频道。</span><span class="sxs-lookup"><span data-stu-id="0505d-119">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="0505d-120">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="0505d-120">conversationIdentityType</span></span>| [<span data-ttu-id="0505d-121">标识</span><span class="sxs-lookup"><span data-stu-id="0505d-121">Identity</span></span>](identity.md) | <span data-ttu-id="0505d-122">可选。</span><span class="sxs-lookup"><span data-stu-id="0505d-122">Optional.</span></span> <span data-ttu-id="0505d-123">指示**会话**属性是否标识团队或频道。</span><span class="sxs-lookup"><span data-stu-id="0505d-123">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="0505d-124">设备</span><span class="sxs-lookup"><span data-stu-id="0505d-124">device</span></span>      | [<span data-ttu-id="0505d-125">标识</span><span class="sxs-lookup"><span data-stu-id="0505d-125">Identity</span></span>](identity.md) | <span data-ttu-id="0505d-p104">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="0505d-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="0505d-128">phone</span><span class="sxs-lookup"><span data-stu-id="0505d-128">phone</span></span>       | [<span data-ttu-id="0505d-129">identity</span><span class="sxs-lookup"><span data-stu-id="0505d-129">identity</span></span>](identity.md) | <span data-ttu-id="0505d-130">可选。</span><span class="sxs-lookup"><span data-stu-id="0505d-130">Optional.</span></span> <span data-ttu-id="0505d-131">与此操作关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="0505d-131">The phone number associated with this action.</span></span> |
| <span data-ttu-id="0505d-132">用户</span><span class="sxs-lookup"><span data-stu-id="0505d-132">user</span></span>        | [<span data-ttu-id="0505d-133">标识</span><span class="sxs-lookup"><span data-stu-id="0505d-133">Identity</span></span>](identity.md) | <span data-ttu-id="0505d-p106">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="0505d-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="0505d-136">注解</span><span class="sxs-lookup"><span data-stu-id="0505d-136">Remarks</span></span> 

<span data-ttu-id="0505d-137">有关**了解 identityset**资源的使用情况, 请参阅[Call](call.md) 。</span><span class="sxs-lookup"><span data-stu-id="0505d-137">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
