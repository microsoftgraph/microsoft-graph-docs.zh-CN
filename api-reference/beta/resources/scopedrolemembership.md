---
title: scopedRoleMembership 资源类型
description: 作用域角色成员身份描述了用户目录角色的成员身份，该角色将进一步限定为管理单元（AU）。  这提供了一种机制，允许租户范围内的公司 adminsistrator 将管理权限委派给用户，以管理组织的某个子集（由 AU 定义的子集）中的用户和组。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d5448db2bb73146b3f3e435376ea7b5d708f0474
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520940"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="75194-104">scopedRoleMembership 资源类型</span><span class="sxs-lookup"><span data-stu-id="75194-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="75194-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="75194-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75194-106">作用域角色成员身份描述了用户目录角色的成员身份，该角色将进一步限定为管理单元（AU）。</span><span class="sxs-lookup"><span data-stu-id="75194-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="75194-107">这提供了一种机制，允许租户范围内的公司 adminsistrator 将管理权限委派给用户，以管理组织的某个子集（由 AU 定义的子集）中的用户和组。</span><span class="sxs-lookup"><span data-stu-id="75194-107">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="75194-108">方法</span><span class="sxs-lookup"><span data-stu-id="75194-108">Methods</span></span>
<span data-ttu-id="75194-109">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="75194-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="75194-110">请参阅[管理 units](administrativeunit.md)主题，查看有关如何查询作用域内角色成员身份的信息，以及如何添加和删除作用域角色成员身份。</span><span class="sxs-lookup"><span data-stu-id="75194-110">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="75194-111">属性</span><span class="sxs-lookup"><span data-stu-id="75194-111">Properties</span></span>
| <span data-ttu-id="75194-112">属性</span><span class="sxs-lookup"><span data-stu-id="75194-112">Property</span></span>   | <span data-ttu-id="75194-113">类型</span><span class="sxs-lookup"><span data-stu-id="75194-113">Type</span></span> | <span data-ttu-id="75194-114">说明</span><span class="sxs-lookup"><span data-stu-id="75194-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="75194-115">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="75194-115">administrativeUnitId</span></span>|<span data-ttu-id="75194-116">string</span><span class="sxs-lookup"><span data-stu-id="75194-116">string</span></span>|<span data-ttu-id="75194-117">目录角色作用域的管理单元的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="75194-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="75194-118">id</span><span class="sxs-lookup"><span data-stu-id="75194-118">id</span></span>|<span data-ttu-id="75194-119">string</span><span class="sxs-lookup"><span data-stu-id="75194-119">string</span></span>| <span data-ttu-id="75194-120">作用域角色成员身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75194-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="75194-121">只读。</span><span class="sxs-lookup"><span data-stu-id="75194-121">Read-only.</span></span>|
|<span data-ttu-id="75194-122">roleId</span><span class="sxs-lookup"><span data-stu-id="75194-122">roleId</span></span>|<span data-ttu-id="75194-123">string</span><span class="sxs-lookup"><span data-stu-id="75194-123">string</span></span>| <span data-ttu-id="75194-124">成员所在目录角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75194-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="75194-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="75194-125">roleMemberInfo</span></span>|[<span data-ttu-id="75194-126">identity</span><span class="sxs-lookup"><span data-stu-id="75194-126">identity</span></span>](identity.md)| <span data-ttu-id="75194-127">角色成员标识信息。</span><span class="sxs-lookup"><span data-stu-id="75194-127">Role member identity information.</span></span> <span data-ttu-id="75194-128">表示属于此作用域角色的成员的用户。</span><span class="sxs-lookup"><span data-stu-id="75194-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75194-129">关系</span><span class="sxs-lookup"><span data-stu-id="75194-129">Relationships</span></span>
<span data-ttu-id="75194-130">无</span><span class="sxs-lookup"><span data-stu-id="75194-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="75194-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75194-131">JSON representation</span></span>

<span data-ttu-id="75194-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75194-132">Here is a JSON representation of the resource.</span></span>

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
