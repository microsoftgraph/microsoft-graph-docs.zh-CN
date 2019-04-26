---
title: scopedRoleMembership 资源类型
description: 作用域角色成员身份描述了用户目录角色的成员身份, 该角色将进一步限定为管理单元 (AU)。  这提供了一种机制, 允许租户范围内的公司 adminsistrator 将管理权限委派给用户, 以管理组织的某个子集 (由 AU 定义的子集) 中的用户和组。
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562977"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="e6c19-104">scopedRoleMembership 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6c19-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c19-105">作用域角色成员身份描述了用户目录角色的成员身份, 该角色将进一步限定为管理单元 (AU)。</span><span class="sxs-lookup"><span data-stu-id="e6c19-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="e6c19-106">这提供了一种机制, 允许租户范围内的公司 adminsistrator 将管理权限委派给用户, 以管理组织的某个子集 (由 AU 定义的子集) 中的用户和组。</span><span class="sxs-lookup"><span data-stu-id="e6c19-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="e6c19-107">方法</span><span class="sxs-lookup"><span data-stu-id="e6c19-107">Methods</span></span>
<span data-ttu-id="e6c19-108">不支持直接向此资源进行查询。</span><span class="sxs-lookup"><span data-stu-id="e6c19-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="e6c19-109">请参阅[管理 units](administrativeunit.md)主题, 查看有关如何查询作用域内角色成员身份的信息, 以及如何添加和删除作用域角色成员身份。</span><span class="sxs-lookup"><span data-stu-id="e6c19-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="e6c19-110">属性</span><span class="sxs-lookup"><span data-stu-id="e6c19-110">Properties</span></span>
| <span data-ttu-id="e6c19-111">属性</span><span class="sxs-lookup"><span data-stu-id="e6c19-111">Property</span></span>   | <span data-ttu-id="e6c19-112">类型</span><span class="sxs-lookup"><span data-stu-id="e6c19-112">Type</span></span> | <span data-ttu-id="e6c19-113">说明</span><span class="sxs-lookup"><span data-stu-id="e6c19-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e6c19-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="e6c19-114">administrativeUnitId</span></span>|<span data-ttu-id="e6c19-115">string</span><span class="sxs-lookup"><span data-stu-id="e6c19-115">string</span></span>|<span data-ttu-id="e6c19-116">目录角色作用域的管理单元的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e6c19-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="e6c19-117">id</span><span class="sxs-lookup"><span data-stu-id="e6c19-117">id</span></span>|<span data-ttu-id="e6c19-118">string</span><span class="sxs-lookup"><span data-stu-id="e6c19-118">string</span></span>| <span data-ttu-id="e6c19-119">作用域角色成员身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e6c19-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="e6c19-120">只读。</span><span class="sxs-lookup"><span data-stu-id="e6c19-120">Read-only.</span></span>|
|<span data-ttu-id="e6c19-121">roleId</span><span class="sxs-lookup"><span data-stu-id="e6c19-121">roleId</span></span>|<span data-ttu-id="e6c19-122">string</span><span class="sxs-lookup"><span data-stu-id="e6c19-122">string</span></span>| <span data-ttu-id="e6c19-123">成员所在目录角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e6c19-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="e6c19-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="e6c19-124">roleMemberInfo</span></span>|[<span data-ttu-id="e6c19-125">identity</span><span class="sxs-lookup"><span data-stu-id="e6c19-125">identity</span></span>](identity.md)| <span data-ttu-id="e6c19-126">角色成员标识信息。</span><span class="sxs-lookup"><span data-stu-id="e6c19-126">Role member identity information.</span></span> <span data-ttu-id="e6c19-127">表示属于此作用域角色的成员的用户。</span><span class="sxs-lookup"><span data-stu-id="e6c19-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6c19-128">关系</span><span class="sxs-lookup"><span data-stu-id="e6c19-128">Relationships</span></span>
<span data-ttu-id="e6c19-129">无</span><span class="sxs-lookup"><span data-stu-id="e6c19-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6c19-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6c19-130">JSON representation</span></span>

<span data-ttu-id="e6c19-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6c19-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
