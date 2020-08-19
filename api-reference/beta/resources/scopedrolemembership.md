---
title: scopedRoleMembership 资源类型
description: 作用域角色成员身份描述用户目录角色的成员身份，该角色的成员将进一步限定为管理单元 (AU) 。  这提供了一种机制，允许租户范围内的公司 adminsistrator 将管理权限委派给用户，以管理由 AU) 定义的一部分组织中的用户和组 (。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abhijeetsinha
ms.openlocfilehash: 27eae463ab0f5fe0718a6d97602e366d32b11b86
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812440"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="aeebf-104">scopedRoleMembership 资源类型</span><span class="sxs-lookup"><span data-stu-id="aeebf-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="aeebf-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeebf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aeebf-106">作用域角色成员身份描述用户目录角色的成员身份，该角色的成员将进一步限定为管理单元 (AU) 。</span><span class="sxs-lookup"><span data-stu-id="aeebf-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="aeebf-107">这提供了一种机制，允许租户范围内的公司管理员将管理权限委派给用户，以管理由 AU) 定义的部分组织中的用户和组 (。</span><span class="sxs-lookup"><span data-stu-id="aeebf-107">This provides a mechanism to allow a tenant-wide company administrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="aeebf-108">方法</span><span class="sxs-lookup"><span data-stu-id="aeebf-108">Methods</span></span>
<span data-ttu-id="aeebf-109">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="aeebf-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="aeebf-110">请参阅 " [管理单元](administrativeunit.md) " 主题，查看有关如何查询作用域内角色成员身份以及如何添加和删除作用域角色成员身份的信息。</span><span class="sxs-lookup"><span data-stu-id="aeebf-110">Please see the [administrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span>

## <a name="properties"></a><span data-ttu-id="aeebf-111">属性</span><span class="sxs-lookup"><span data-stu-id="aeebf-111">Properties</span></span>
| <span data-ttu-id="aeebf-112">属性</span><span class="sxs-lookup"><span data-stu-id="aeebf-112">Property</span></span>   | <span data-ttu-id="aeebf-113">类型</span><span class="sxs-lookup"><span data-stu-id="aeebf-113">Type</span></span> | <span data-ttu-id="aeebf-114">说明</span><span class="sxs-lookup"><span data-stu-id="aeebf-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aeebf-115">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="aeebf-115">administrativeUnitId</span></span>|<span data-ttu-id="aeebf-116">string</span><span class="sxs-lookup"><span data-stu-id="aeebf-116">string</span></span>|<span data-ttu-id="aeebf-117">目录角色作用域的管理单元的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="aeebf-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="aeebf-118">id</span><span class="sxs-lookup"><span data-stu-id="aeebf-118">id</span></span>|<span data-ttu-id="aeebf-119">string</span><span class="sxs-lookup"><span data-stu-id="aeebf-119">string</span></span>| <span data-ttu-id="aeebf-120">作用域角色成员身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aeebf-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="aeebf-121">只读。</span><span class="sxs-lookup"><span data-stu-id="aeebf-121">Read-only.</span></span>|
|<span data-ttu-id="aeebf-122">roleId</span><span class="sxs-lookup"><span data-stu-id="aeebf-122">roleId</span></span>|<span data-ttu-id="aeebf-123">string</span><span class="sxs-lookup"><span data-stu-id="aeebf-123">string</span></span>| <span data-ttu-id="aeebf-124">成员所在目录角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aeebf-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="aeebf-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="aeebf-125">roleMemberInfo</span></span>|[<span data-ttu-id="aeebf-126">identity</span><span class="sxs-lookup"><span data-stu-id="aeebf-126">identity</span></span>](identity.md)| <span data-ttu-id="aeebf-127">角色成员标识信息。</span><span class="sxs-lookup"><span data-stu-id="aeebf-127">Role member identity information.</span></span> <span data-ttu-id="aeebf-128">表示属于此作用域角色的成员的用户。</span><span class="sxs-lookup"><span data-stu-id="aeebf-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aeebf-129">关系</span><span class="sxs-lookup"><span data-stu-id="aeebf-129">Relationships</span></span>
<span data-ttu-id="aeebf-130">无</span><span class="sxs-lookup"><span data-stu-id="aeebf-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aeebf-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aeebf-131">JSON representation</span></span>

<span data-ttu-id="aeebf-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aeebf-132">Here is a JSON representation of the resource.</span></span>

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
