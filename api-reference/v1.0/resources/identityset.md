---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
ms.openlocfilehash: 4d2bb5d92ebe06e79a68d69b949baec19a33a4c6
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="identityset-resource-type"></a><span data-ttu-id="e947f-102">IdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="e947f-102">IdentitySet resource type</span></span>

<span data-ttu-id="e947f-p101">**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="e947f-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e947f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e947f-105">JSON representation</span></span>

<span data-ttu-id="e947f-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e947f-106">Here is a JSON representation of the resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="e947f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e947f-107">Properties</span></span>

| <span data-ttu-id="e947f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e947f-108">Property</span></span>    | <span data-ttu-id="e947f-109">类型</span><span class="sxs-lookup"><span data-stu-id="e947f-109">Type</span></span>                    | <span data-ttu-id="e947f-110">说明</span><span class="sxs-lookup"><span data-stu-id="e947f-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="e947f-111">application</span><span class="sxs-lookup"><span data-stu-id="e947f-111">application</span></span> | [<span data-ttu-id="e947f-112">标识</span><span class="sxs-lookup"><span data-stu-id="e947f-112">Identity</span></span>](identity.md) | <span data-ttu-id="e947f-p102">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e947f-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="e947f-115">设备</span><span class="sxs-lookup"><span data-stu-id="e947f-115">device</span></span>      | [<span data-ttu-id="e947f-116">标识</span><span class="sxs-lookup"><span data-stu-id="e947f-116">Identity</span></span>](identity.md) | <span data-ttu-id="e947f-p103">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="e947f-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="e947f-119">用户</span><span class="sxs-lookup"><span data-stu-id="e947f-119">user</span></span>        | [<span data-ttu-id="e947f-120">标识</span><span class="sxs-lookup"><span data-stu-id="e947f-120">Identity</span></span>](identity.md) | <span data-ttu-id="e947f-p104">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="e947f-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="e947f-123">注解</span><span class="sxs-lookup"><span data-stu-id="e947f-123">Remarks</span></span> 

<span data-ttu-id="e947f-124">请参阅 [DriveItem](driveitem.md) 以了解 **IdentitySet** 资源的使用情况。</span><span class="sxs-lookup"><span data-stu-id="e947f-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
