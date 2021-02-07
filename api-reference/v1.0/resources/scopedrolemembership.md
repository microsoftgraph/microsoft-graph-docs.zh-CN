---
title: scopedRoleMembership 资源类型
description: 作用域角色成员身份描述目录角色的用户成员身份，该角色的范围进一步缩小到 AU (管理) 。  这提供了一种机制，允许租户范围的公司管理员将管理权限委派给用户，以管理组织子集中的用户和组 (由 AU 管理员定义的子集) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: 8b7a2239d0ee44ab6caf0e98c7d818431764b1b1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129903"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="fc6be-104">scopedRoleMembership 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc6be-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="fc6be-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc6be-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc6be-106">作用域角色成员身份描述目录角色的用户成员身份，该角色的范围进一步缩小到 AU (管理) 。</span><span class="sxs-lookup"><span data-stu-id="fc6be-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="fc6be-107">这提供了一种机制，允许租户范围的公司管理员将管理权限委派给用户，以管理组织子集中的用户和组 (该子集由 AU) 。</span><span class="sxs-lookup"><span data-stu-id="fc6be-107">This provides a mechanism to allow a tenant-wide company administrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="fc6be-108">Methods</span><span class="sxs-lookup"><span data-stu-id="fc6be-108">Methods</span></span>
<span data-ttu-id="fc6be-109">不支持直接查询此资源。</span><span class="sxs-lookup"><span data-stu-id="fc6be-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="fc6be-110">请参阅管理 [单元](administrativeunit.md) 主题，了解如何查询作用域角色成员身份以及添加和删除作用域角色成员身份。</span><span class="sxs-lookup"><span data-stu-id="fc6be-110">Please see the [administrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span>

## <a name="properties"></a><span data-ttu-id="fc6be-111">属性</span><span class="sxs-lookup"><span data-stu-id="fc6be-111">Properties</span></span>
| <span data-ttu-id="fc6be-112">属性</span><span class="sxs-lookup"><span data-stu-id="fc6be-112">Property</span></span>   | <span data-ttu-id="fc6be-113">类型</span><span class="sxs-lookup"><span data-stu-id="fc6be-113">Type</span></span> | <span data-ttu-id="fc6be-114">说明</span><span class="sxs-lookup"><span data-stu-id="fc6be-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fc6be-115">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="fc6be-115">administrativeUnitId</span></span>|<span data-ttu-id="fc6be-116">string</span><span class="sxs-lookup"><span data-stu-id="fc6be-116">string</span></span>|<span data-ttu-id="fc6be-117">目录角色作用域为的管理单元的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="fc6be-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="fc6be-118">id</span><span class="sxs-lookup"><span data-stu-id="fc6be-118">id</span></span>|<span data-ttu-id="fc6be-119">string</span><span class="sxs-lookup"><span data-stu-id="fc6be-119">string</span></span>| <span data-ttu-id="fc6be-120">作用域角色成员身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fc6be-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="fc6be-121">只读。</span><span class="sxs-lookup"><span data-stu-id="fc6be-121">Read-only.</span></span>|
|<span data-ttu-id="fc6be-122">roleId</span><span class="sxs-lookup"><span data-stu-id="fc6be-122">roleId</span></span>|<span data-ttu-id="fc6be-123">string</span><span class="sxs-lookup"><span data-stu-id="fc6be-123">string</span></span>| <span data-ttu-id="fc6be-124">成员位于的目录角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fc6be-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="fc6be-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="fc6be-125">roleMemberInfo</span></span>|[<span data-ttu-id="fc6be-126">identity</span><span class="sxs-lookup"><span data-stu-id="fc6be-126">identity</span></span>](identity.md)| <span data-ttu-id="fc6be-127">角色成员标识信息。</span><span class="sxs-lookup"><span data-stu-id="fc6be-127">Role member identity information.</span></span> <span data-ttu-id="fc6be-128">表示是此作用域角色的成员的用户。</span><span class="sxs-lookup"><span data-stu-id="fc6be-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc6be-129">关系</span><span class="sxs-lookup"><span data-stu-id="fc6be-129">Relationships</span></span>
<span data-ttu-id="fc6be-130">无</span><span class="sxs-lookup"><span data-stu-id="fc6be-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fc6be-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc6be-131">JSON representation</span></span>

<span data-ttu-id="fc6be-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc6be-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
