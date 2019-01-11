---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 63178fc9add3d097b7e8aaf0c5c2a697a91eaeed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807019"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="b60ae-102">identitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="b60ae-102">identitySet resource type</span></span>

<span data-ttu-id="b60ae-p101">**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="b60ae-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b60ae-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b60ae-105">JSON representation</span></span>

<span data-ttu-id="b60ae-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b60ae-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
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
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="b60ae-107">属性</span><span class="sxs-lookup"><span data-stu-id="b60ae-107">Properties</span></span>

| <span data-ttu-id="b60ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="b60ae-108">Property</span></span>    | <span data-ttu-id="b60ae-109">类型</span><span class="sxs-lookup"><span data-stu-id="b60ae-109">Type</span></span>                    | <span data-ttu-id="b60ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="b60ae-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="b60ae-111">application</span><span class="sxs-lookup"><span data-stu-id="b60ae-111">application</span></span> | [<span data-ttu-id="b60ae-112">标识</span><span class="sxs-lookup"><span data-stu-id="b60ae-112">Identity</span></span>](identity.md) | <span data-ttu-id="b60ae-p102">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b60ae-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="b60ae-115">设备</span><span class="sxs-lookup"><span data-stu-id="b60ae-115">device</span></span>      | [<span data-ttu-id="b60ae-116">标识</span><span class="sxs-lookup"><span data-stu-id="b60ae-116">Identity</span></span>](identity.md) | <span data-ttu-id="b60ae-p103">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="b60ae-p103">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="b60ae-119">phone</span><span class="sxs-lookup"><span data-stu-id="b60ae-119">phone</span></span>       | [<span data-ttu-id="b60ae-120">identity</span><span class="sxs-lookup"><span data-stu-id="b60ae-120">identity</span></span>](identity.md) | <span data-ttu-id="b60ae-121">可选。</span><span class="sxs-lookup"><span data-stu-id="b60ae-121">Optional.</span></span> <span data-ttu-id="b60ae-122">与此操作关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b60ae-122">The phone number associated with this action.</span></span> |
| <span data-ttu-id="b60ae-123">用户</span><span class="sxs-lookup"><span data-stu-id="b60ae-123">user</span></span>        | [<span data-ttu-id="b60ae-124">标识</span><span class="sxs-lookup"><span data-stu-id="b60ae-124">Identity</span></span>](identity.md) | <span data-ttu-id="b60ae-p105">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="b60ae-p105">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="b60ae-127">注解</span><span class="sxs-lookup"><span data-stu-id="b60ae-127">Remarks</span></span> 

<span data-ttu-id="b60ae-128">**IdentitySet**资源的使用情况，请参阅[呼叫](call.md)。</span><span class="sxs-lookup"><span data-stu-id="b60ae-128">See [Call](call.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
