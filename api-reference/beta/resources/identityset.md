---
author: JeremyKelley
description: 了解 identityset 资源是标识资源的键控集合。
ms.date: 09/10/2017
title: 了解 identityset
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 08986af20ae7591798a222e68d9b9bee5244e273
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496605"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="cfb3f-103">了解 identityset 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfb3f-103">identitySet resource type</span></span>

<span data-ttu-id="cfb3f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cfb3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfb3f-105">**了解 identityset**资源是[标识](identity.md)资源的键控集合。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-105">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="cfb3f-106">它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-106">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfb3f-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfb3f-107">JSON representation</span></span>

<span data-ttu-id="cfb3f-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-108">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cfb3f-109">属性</span><span class="sxs-lookup"><span data-stu-id="cfb3f-109">Properties</span></span>

| <span data-ttu-id="cfb3f-110">属性</span><span class="sxs-lookup"><span data-stu-id="cfb3f-110">Property</span></span>    | <span data-ttu-id="cfb3f-111">类型</span><span class="sxs-lookup"><span data-stu-id="cfb3f-111">Type</span></span>                    | <span data-ttu-id="cfb3f-112">说明</span><span class="sxs-lookup"><span data-stu-id="cfb3f-112">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="cfb3f-113">application</span><span class="sxs-lookup"><span data-stu-id="cfb3f-113">application</span></span> | [<span data-ttu-id="cfb3f-114">标识</span><span class="sxs-lookup"><span data-stu-id="cfb3f-114">Identity</span></span>](identity.md) | <span data-ttu-id="cfb3f-p101">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="cfb3f-117">对话</span><span class="sxs-lookup"><span data-stu-id="cfb3f-117">conversation</span></span>| [<span data-ttu-id="cfb3f-118">标识</span><span class="sxs-lookup"><span data-stu-id="cfb3f-118">Identity</span></span>](identity.md) | <span data-ttu-id="cfb3f-119">可选。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-119">Optional.</span></span> <span data-ttu-id="cfb3f-120">与此操作关联的团队或频道。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-120">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="cfb3f-121">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="cfb3f-121">conversationIdentityType</span></span>| [<span data-ttu-id="cfb3f-122">标识</span><span class="sxs-lookup"><span data-stu-id="cfb3f-122">Identity</span></span>](identity.md) | <span data-ttu-id="cfb3f-123">可选。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-123">Optional.</span></span> <span data-ttu-id="cfb3f-124">指示**会话**属性是否标识团队或频道。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-124">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="cfb3f-125">设备</span><span class="sxs-lookup"><span data-stu-id="cfb3f-125">device</span></span>      | [<span data-ttu-id="cfb3f-126">标识</span><span class="sxs-lookup"><span data-stu-id="cfb3f-126">Identity</span></span>](identity.md) | <span data-ttu-id="cfb3f-p104">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="cfb3f-129">phone</span><span class="sxs-lookup"><span data-stu-id="cfb3f-129">phone</span></span>       | [<span data-ttu-id="cfb3f-130">identity</span><span class="sxs-lookup"><span data-stu-id="cfb3f-130">identity</span></span>](identity.md) | <span data-ttu-id="cfb3f-131">可选。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-131">Optional.</span></span> <span data-ttu-id="cfb3f-132">与此操作关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-132">The phone number associated with this action.</span></span> |
| <span data-ttu-id="cfb3f-133">用户</span><span class="sxs-lookup"><span data-stu-id="cfb3f-133">user</span></span>        | [<span data-ttu-id="cfb3f-134">标识</span><span class="sxs-lookup"><span data-stu-id="cfb3f-134">Identity</span></span>](identity.md) | <span data-ttu-id="cfb3f-p106">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="cfb3f-137">注解</span><span class="sxs-lookup"><span data-stu-id="cfb3f-137">Remarks</span></span> 

<span data-ttu-id="cfb3f-138">有关**了解 identityset**资源的使用情况，请参阅[Call](call.md) 。</span><span class="sxs-lookup"><span data-stu-id="cfb3f-138">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
