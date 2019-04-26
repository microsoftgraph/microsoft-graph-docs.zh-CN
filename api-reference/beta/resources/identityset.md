---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 了解 identityset
localization_priority: Normal
ms.openlocfilehash: b1570fc0ec0a6e28bab569dfae6992675d8b3537
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333657"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="31368-102">了解 identityset 资源类型</span><span class="sxs-lookup"><span data-stu-id="31368-102">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31368-103">**了解 identityset**资源是[标识](identity.md)资源的键控集合。</span><span class="sxs-lookup"><span data-stu-id="31368-103">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="31368-104">它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="31368-104">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31368-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31368-105">JSON representation</span></span>

<span data-ttu-id="31368-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31368-106">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="31368-107">属性</span><span class="sxs-lookup"><span data-stu-id="31368-107">Properties</span></span>

| <span data-ttu-id="31368-108">属性</span><span class="sxs-lookup"><span data-stu-id="31368-108">Property</span></span>    | <span data-ttu-id="31368-109">类型</span><span class="sxs-lookup"><span data-stu-id="31368-109">Type</span></span>                    | <span data-ttu-id="31368-110">说明</span><span class="sxs-lookup"><span data-stu-id="31368-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="31368-111">application</span><span class="sxs-lookup"><span data-stu-id="31368-111">application</span></span> | [<span data-ttu-id="31368-112">标识</span><span class="sxs-lookup"><span data-stu-id="31368-112">Identity</span></span>](identity.md) | <span data-ttu-id="31368-p101">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="31368-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="31368-115">conversation</span><span class="sxs-lookup"><span data-stu-id="31368-115">conversation</span></span>| [<span data-ttu-id="31368-116">标识</span><span class="sxs-lookup"><span data-stu-id="31368-116">Identity</span></span>](identity.md) | <span data-ttu-id="31368-117">可选。</span><span class="sxs-lookup"><span data-stu-id="31368-117">Optional.</span></span> <span data-ttu-id="31368-118">与此操作关联的团队或频道。</span><span class="sxs-lookup"><span data-stu-id="31368-118">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="31368-119">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="31368-119">conversationIdentityType</span></span>| [<span data-ttu-id="31368-120">标识</span><span class="sxs-lookup"><span data-stu-id="31368-120">Identity</span></span>](identity.md) | <span data-ttu-id="31368-121">可选。</span><span class="sxs-lookup"><span data-stu-id="31368-121">Optional.</span></span> <span data-ttu-id="31368-122">指示**会话**属性是否标识团队或频道。</span><span class="sxs-lookup"><span data-stu-id="31368-122">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="31368-123">设备</span><span class="sxs-lookup"><span data-stu-id="31368-123">device</span></span>      | [<span data-ttu-id="31368-124">标识</span><span class="sxs-lookup"><span data-stu-id="31368-124">Identity</span></span>](identity.md) | <span data-ttu-id="31368-p104">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="31368-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="31368-127">phone</span><span class="sxs-lookup"><span data-stu-id="31368-127">phone</span></span>       | [<span data-ttu-id="31368-128">identity</span><span class="sxs-lookup"><span data-stu-id="31368-128">identity</span></span>](identity.md) | <span data-ttu-id="31368-129">可选。</span><span class="sxs-lookup"><span data-stu-id="31368-129">Optional.</span></span> <span data-ttu-id="31368-130">与此操作关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="31368-130">The phone number associated with this action.</span></span> |
| <span data-ttu-id="31368-131">用户</span><span class="sxs-lookup"><span data-stu-id="31368-131">user</span></span>        | [<span data-ttu-id="31368-132">标识</span><span class="sxs-lookup"><span data-stu-id="31368-132">Identity</span></span>](identity.md) | <span data-ttu-id="31368-p106">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="31368-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="31368-135">注解</span><span class="sxs-lookup"><span data-stu-id="31368-135">Remarks</span></span> 

<span data-ttu-id="31368-136">有关**了解 identityset**资源的使用情况, 请参阅[Call](call.md) 。</span><span class="sxs-lookup"><span data-stu-id="31368-136">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
