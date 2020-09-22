---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 了解 identityset
localization_priority: Normal
description: IdentitySet 资源是 标识 资源的键控集合。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 09a0a48ca46f0d3a429705e5becf18f37832e5a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086667"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="d5bca-103">IdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5bca-103">IdentitySet resource type</span></span>

<span data-ttu-id="d5bca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5bca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5bca-p101">**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="d5bca-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5bca-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5bca-107">JSON representation</span></span>

<span data-ttu-id="d5bca-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5bca-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d5bca-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5bca-109">Properties</span></span>

| <span data-ttu-id="d5bca-110">属性</span><span class="sxs-lookup"><span data-stu-id="d5bca-110">Property</span></span>    | <span data-ttu-id="d5bca-111">类型</span><span class="sxs-lookup"><span data-stu-id="d5bca-111">Type</span></span>                    | <span data-ttu-id="d5bca-112">说明</span><span class="sxs-lookup"><span data-stu-id="d5bca-112">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="d5bca-113">application</span><span class="sxs-lookup"><span data-stu-id="d5bca-113">application</span></span> | [<span data-ttu-id="d5bca-114">标识</span><span class="sxs-lookup"><span data-stu-id="d5bca-114">Identity</span></span>](identity.md) | <span data-ttu-id="d5bca-p102">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d5bca-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="d5bca-117">设备</span><span class="sxs-lookup"><span data-stu-id="d5bca-117">device</span></span>      | [<span data-ttu-id="d5bca-118">标识</span><span class="sxs-lookup"><span data-stu-id="d5bca-118">Identity</span></span>](identity.md) | <span data-ttu-id="d5bca-p103">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="d5bca-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="d5bca-121">用户</span><span class="sxs-lookup"><span data-stu-id="d5bca-121">user</span></span>        | [<span data-ttu-id="d5bca-122">标识</span><span class="sxs-lookup"><span data-stu-id="d5bca-122">Identity</span></span>](identity.md) | <span data-ttu-id="d5bca-p104">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="d5bca-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="d5bca-125">注解</span><span class="sxs-lookup"><span data-stu-id="d5bca-125">Remarks</span></span> 

<span data-ttu-id="d5bca-126">请参阅 [DriveItem](driveitem.md) 以了解 **IdentitySet** 资源的使用情况。</span><span class="sxs-lookup"><span data-stu-id="d5bca-126">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

