---
title: scopedRoleMembership 资源类型
description: 作用域角色成员身份描述了用户目录角色的成员身份, 该角色将进一步限定为管理单元 (AU)。  这提供了一种机制, 允许租户范围内的公司 adminsistrator 将管理权限委派给用户, 以管理组织的某个子集 (由 AU 定义的子集) 中的用户和组。
localization_priority: Normal
ms.openlocfilehash: 56a2514fa65033154b6ab69c497c90fde201c28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343455"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="206e4-104">scopedRoleMembership 资源类型</span><span class="sxs-lookup"><span data-stu-id="206e4-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="206e4-105">作用域角色成员身份描述了用户目录角色的成员身份, 该角色将进一步限定为管理单元 (AU)。</span><span class="sxs-lookup"><span data-stu-id="206e4-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="206e4-106">这提供了一种机制, 允许租户范围内的公司 adminsistrator 将管理权限委派给用户, 以管理组织的某个子集 (由 AU 定义的子集) 中的用户和组。</span><span class="sxs-lookup"><span data-stu-id="206e4-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="206e4-107">方法</span><span class="sxs-lookup"><span data-stu-id="206e4-107">Methods</span></span>
<span data-ttu-id="206e4-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="206e4-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="206e4-109">请参阅[管理 units](administrativeunit.md)主题, 查看有关如何查询作用域内角色成员身份的信息, 以及如何添加和删除作用域角色成员身份。</span><span class="sxs-lookup"><span data-stu-id="206e4-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="206e4-110">属性</span><span class="sxs-lookup"><span data-stu-id="206e4-110">Properties</span></span>
| <span data-ttu-id="206e4-111">属性</span><span class="sxs-lookup"><span data-stu-id="206e4-111">Property</span></span>   | <span data-ttu-id="206e4-112">类型</span><span class="sxs-lookup"><span data-stu-id="206e4-112">Type</span></span> | <span data-ttu-id="206e4-113">说明</span><span class="sxs-lookup"><span data-stu-id="206e4-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="206e4-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="206e4-114">administrativeUnitId</span></span>|<span data-ttu-id="206e4-115">string</span><span class="sxs-lookup"><span data-stu-id="206e4-115">string</span></span>|<span data-ttu-id="206e4-116">目录角色作用域的管理单元的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="206e4-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="206e4-117">id</span><span class="sxs-lookup"><span data-stu-id="206e4-117">id</span></span>|<span data-ttu-id="206e4-118">string</span><span class="sxs-lookup"><span data-stu-id="206e4-118">string</span></span>| <span data-ttu-id="206e4-119">作用域角色成员身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="206e4-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="206e4-120">只读。</span><span class="sxs-lookup"><span data-stu-id="206e4-120">Read-only.</span></span>|
|<span data-ttu-id="206e4-121">roleId</span><span class="sxs-lookup"><span data-stu-id="206e4-121">roleId</span></span>|<span data-ttu-id="206e4-122">string</span><span class="sxs-lookup"><span data-stu-id="206e4-122">string</span></span>| <span data-ttu-id="206e4-123">成员所在目录角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="206e4-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="206e4-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="206e4-124">roleMemberInfo</span></span>|[<span data-ttu-id="206e4-125">identity</span><span class="sxs-lookup"><span data-stu-id="206e4-125">identity</span></span>](identity.md)| <span data-ttu-id="206e4-126">角色成员标识信息。</span><span class="sxs-lookup"><span data-stu-id="206e4-126">Role member identity information.</span></span> <span data-ttu-id="206e4-127">表示属于此作用域角色的成员的用户。</span><span class="sxs-lookup"><span data-stu-id="206e4-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="206e4-128">关系</span><span class="sxs-lookup"><span data-stu-id="206e4-128">Relationships</span></span>
<span data-ttu-id="206e4-129">无</span><span class="sxs-lookup"><span data-stu-id="206e4-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="206e4-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="206e4-130">JSON representation</span></span>

<span data-ttu-id="206e4-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="206e4-131">Here is a JSON representation of the resource.</span></span>

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
