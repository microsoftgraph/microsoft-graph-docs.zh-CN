---
author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: IdentitySet 资源是 标识 资源的键控集合。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e6f7aef915596e39173f286a3433e0114656e707
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239959"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="2a706-103">IdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a706-103">IdentitySet resource type</span></span>

<span data-ttu-id="2a706-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a706-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a706-p101">**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如 _创建者_ 或 _上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="2a706-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a706-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a706-107">JSON representation</span></span>

<span data-ttu-id="2a706-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a706-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2a706-109">属性</span><span class="sxs-lookup"><span data-stu-id="2a706-109">Properties</span></span>

| <span data-ttu-id="2a706-110">属性</span><span class="sxs-lookup"><span data-stu-id="2a706-110">Property</span></span>    | <span data-ttu-id="2a706-111">类型</span><span class="sxs-lookup"><span data-stu-id="2a706-111">Type</span></span>                    | <span data-ttu-id="2a706-112">说明</span><span class="sxs-lookup"><span data-stu-id="2a706-112">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="2a706-113">application</span><span class="sxs-lookup"><span data-stu-id="2a706-113">application</span></span> | [<span data-ttu-id="2a706-114">标识</span><span class="sxs-lookup"><span data-stu-id="2a706-114">Identity</span></span>](identity.md) | <span data-ttu-id="2a706-p102">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="2a706-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="2a706-117">设备</span><span class="sxs-lookup"><span data-stu-id="2a706-117">device</span></span>      | [<span data-ttu-id="2a706-118">标识</span><span class="sxs-lookup"><span data-stu-id="2a706-118">Identity</span></span>](identity.md) | <span data-ttu-id="2a706-p103">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="2a706-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="2a706-121">用户</span><span class="sxs-lookup"><span data-stu-id="2a706-121">user</span></span>        | [<span data-ttu-id="2a706-122">标识</span><span class="sxs-lookup"><span data-stu-id="2a706-122">Identity</span></span>](identity.md) | <span data-ttu-id="2a706-p104">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="2a706-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="2a706-125">注解</span><span class="sxs-lookup"><span data-stu-id="2a706-125">Remarks</span></span> 

<span data-ttu-id="2a706-126">请参阅 [DriveItem](driveitem.md) 以了解 **IdentitySet** 资源的使用情况。</span><span class="sxs-lookup"><span data-stu-id="2a706-126">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

