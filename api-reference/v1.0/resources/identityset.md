---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 了解 identityset
localization_priority: Normal
ms.openlocfilehash: 369068dd48b9173032542303e3fd9831d25e6e9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567569"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="3c7b4-102">IdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c7b4-102">IdentitySet resource type</span></span>

<span data-ttu-id="3c7b4-p101">**IdentitySet** 资源是 [标识](identity.md) 资源的键控集合。它用来表示一组与项目的各种事件相关的标识，例如_创建者_或_上次修改人_。</span><span class="sxs-lookup"><span data-stu-id="3c7b4-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c7b4-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c7b4-105">JSON representation</span></span>

<span data-ttu-id="3c7b4-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c7b4-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3c7b4-107">属性</span><span class="sxs-lookup"><span data-stu-id="3c7b4-107">Properties</span></span>

| <span data-ttu-id="3c7b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c7b4-108">Property</span></span>    | <span data-ttu-id="3c7b4-109">类型</span><span class="sxs-lookup"><span data-stu-id="3c7b4-109">Type</span></span>                    | <span data-ttu-id="3c7b4-110">说明</span><span class="sxs-lookup"><span data-stu-id="3c7b4-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="3c7b4-111">application</span><span class="sxs-lookup"><span data-stu-id="3c7b4-111">application</span></span> | [<span data-ttu-id="3c7b4-112">标识</span><span class="sxs-lookup"><span data-stu-id="3c7b4-112">Identity</span></span>](identity.md) | <span data-ttu-id="3c7b4-p102">可选。与此操作关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="3c7b4-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="3c7b4-115">设备</span><span class="sxs-lookup"><span data-stu-id="3c7b4-115">device</span></span>      | [<span data-ttu-id="3c7b4-116">标识</span><span class="sxs-lookup"><span data-stu-id="3c7b4-116">Identity</span></span>](identity.md) | <span data-ttu-id="3c7b4-p103">可选。与此操作关联的设备。</span><span class="sxs-lookup"><span data-stu-id="3c7b4-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="3c7b4-119">用户</span><span class="sxs-lookup"><span data-stu-id="3c7b4-119">user</span></span>        | [<span data-ttu-id="3c7b4-120">标识</span><span class="sxs-lookup"><span data-stu-id="3c7b4-120">Identity</span></span>](identity.md) | <span data-ttu-id="3c7b4-p104">可选。与此操作关联的用户。</span><span class="sxs-lookup"><span data-stu-id="3c7b4-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="3c7b4-123">注解</span><span class="sxs-lookup"><span data-stu-id="3c7b4-123">Remarks</span></span> 

<span data-ttu-id="3c7b4-124">请参阅 [DriveItem](driveitem.md) 以了解 **IdentitySet** 资源的使用情况。</span><span class="sxs-lookup"><span data-stu-id="3c7b4-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
