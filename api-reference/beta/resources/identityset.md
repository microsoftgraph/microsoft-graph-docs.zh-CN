---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 10b39bd5747e10ea4340bb5b4c54df0f94eb4229
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547142"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="21268-102">了解 identityset 资源类型</span><span class="sxs-lookup"><span data-stu-id="21268-102">identitySet resource type</span></span>

<span data-ttu-id="21268-103">**了解 identityset**资源是[标识](identity.md)资源的键控集合。</span><span class="sxs-lookup"><span data-stu-id="21268-103">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>
<span data-ttu-id="21268-104">它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="21268-104">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21268-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21268-105">JSON representation</span></span>

<span data-ttu-id="21268-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21268-106">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="21268-107">属性</span><span class="sxs-lookup"><span data-stu-id="21268-107">Properties</span></span>

| <span data-ttu-id="21268-108">属性</span><span class="sxs-lookup"><span data-stu-id="21268-108">Property</span></span>    | <span data-ttu-id="21268-109">类型</span><span class="sxs-lookup"><span data-stu-id="21268-109">Type</span></span>                    | <span data-ttu-id="21268-110">说明</span><span class="sxs-lookup"><span data-stu-id="21268-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="21268-111">application</span><span class="sxs-lookup"><span data-stu-id="21268-111">application</span></span> | [<span data-ttu-id="21268-112">标识</span><span class="sxs-lookup"><span data-stu-id="21268-112">Identity</span></span>](identity.md) | <span data-ttu-id="21268-p102">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="21268-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="21268-115">对话</span><span class="sxs-lookup"><span data-stu-id="21268-115">conversation</span></span>| [<span data-ttu-id="21268-116">标识</span><span class="sxs-lookup"><span data-stu-id="21268-116">Identity</span></span>](identity.md) | <span data-ttu-id="21268-117">可选。</span><span class="sxs-lookup"><span data-stu-id="21268-117">Optional.</span></span> <span data-ttu-id="21268-118">与此操作关联的团队或频道。</span><span class="sxs-lookup"><span data-stu-id="21268-118">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="21268-119">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="21268-119">conversationIdentityType</span></span>| [<span data-ttu-id="21268-120">标识</span><span class="sxs-lookup"><span data-stu-id="21268-120">Identity</span></span>](identity.md) | <span data-ttu-id="21268-121">可选。</span><span class="sxs-lookup"><span data-stu-id="21268-121">Optional.</span></span> <span data-ttu-id="21268-122">指示**会话**属性是否标识团队或频道。</span><span class="sxs-lookup"><span data-stu-id="21268-122">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="21268-123">设备</span><span class="sxs-lookup"><span data-stu-id="21268-123">device</span></span>      | [<span data-ttu-id="21268-124">标识</span><span class="sxs-lookup"><span data-stu-id="21268-124">Identity</span></span>](identity.md) | <span data-ttu-id="21268-p105">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="21268-p105">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="21268-127">phone</span><span class="sxs-lookup"><span data-stu-id="21268-127">phone</span></span>       | [<span data-ttu-id="21268-128">identity</span><span class="sxs-lookup"><span data-stu-id="21268-128">identity</span></span>](identity.md) | <span data-ttu-id="21268-129">可选。</span><span class="sxs-lookup"><span data-stu-id="21268-129">Optional.</span></span> <span data-ttu-id="21268-130">与此操作关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="21268-130">The phone number associated with this action.</span></span> |
| <span data-ttu-id="21268-131">用户</span><span class="sxs-lookup"><span data-stu-id="21268-131">user</span></span>        | [<span data-ttu-id="21268-132">标识</span><span class="sxs-lookup"><span data-stu-id="21268-132">Identity</span></span>](identity.md) | <span data-ttu-id="21268-p107">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="21268-p107">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="21268-135">注解</span><span class="sxs-lookup"><span data-stu-id="21268-135">Remarks</span></span> 

<span data-ttu-id="21268-136">有关**了解 identityset**资源的使用情况, 请参阅[Call](call.md) 。</span><span class="sxs-lookup"><span data-stu-id="21268-136">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
