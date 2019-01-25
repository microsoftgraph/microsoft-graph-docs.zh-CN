---
title: scopedRoleMembership 资源类型
description: 作用域角色成员资格介绍目录角色，进一步范围限定到管理单元 (AU) 的用户的成员的身份。  这提供了一种机制，以允许租户范围公司 adminsistrator 以委派用户管理用户和组的子集组织 （由 AU 正在定义的子集） 的管理权限。
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521500"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="cdc8a-104">scopedRoleMembership 资源类型</span><span class="sxs-lookup"><span data-stu-id="cdc8a-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc8a-105">作用域角色成员资格介绍目录角色，进一步范围限定到管理单元 (AU) 的用户的成员的身份。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="cdc8a-106">这提供了一种机制，以允许租户范围公司 adminsistrator 以委派用户管理用户和组的子集组织 （由 AU 正在定义的子集） 的管理权限。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="cdc8a-107">方法</span><span class="sxs-lookup"><span data-stu-id="cdc8a-107">Methods</span></span>
<span data-ttu-id="cdc8a-108">不支持直接查询到此资源。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="cdc8a-109">请参阅[管理单元](administrativeunit.md)主题，若要查看有关如何查询范围角色成员身份，以及添加和移除范围角色成员身份信息。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="cdc8a-110">属性</span><span class="sxs-lookup"><span data-stu-id="cdc8a-110">Properties</span></span>
| <span data-ttu-id="cdc8a-111">属性</span><span class="sxs-lookup"><span data-stu-id="cdc8a-111">Property</span></span>   | <span data-ttu-id="cdc8a-112">类型</span><span class="sxs-lookup"><span data-stu-id="cdc8a-112">Type</span></span> | <span data-ttu-id="cdc8a-113">说明</span><span class="sxs-lookup"><span data-stu-id="cdc8a-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cdc8a-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="cdc8a-114">administrativeUnitId</span></span>|<span data-ttu-id="cdc8a-115">string</span><span class="sxs-lookup"><span data-stu-id="cdc8a-115">string</span></span>|<span data-ttu-id="cdc8a-116">唯一标识符的目录角色范围限定为管理单元</span><span class="sxs-lookup"><span data-stu-id="cdc8a-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="cdc8a-117">id</span><span class="sxs-lookup"><span data-stu-id="cdc8a-117">id</span></span>|<span data-ttu-id="cdc8a-118">string</span><span class="sxs-lookup"><span data-stu-id="cdc8a-118">string</span></span>| <span data-ttu-id="cdc8a-119">作用域角色成员身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="cdc8a-120">只读。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-120">Read-only.</span></span>|
|<span data-ttu-id="cdc8a-121">roleId</span><span class="sxs-lookup"><span data-stu-id="cdc8a-121">roleId</span></span>|<span data-ttu-id="cdc8a-122">string</span><span class="sxs-lookup"><span data-stu-id="cdc8a-122">string</span></span>| <span data-ttu-id="cdc8a-123">为目录角色中的成员的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="cdc8a-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="cdc8a-124">roleMemberInfo</span></span>|[<span data-ttu-id="cdc8a-125">identity</span><span class="sxs-lookup"><span data-stu-id="cdc8a-125">identity</span></span>](identity.md)| <span data-ttu-id="cdc8a-126">角色成员身份信息。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-126">Role member identity information.</span></span> <span data-ttu-id="cdc8a-127">表示此作用域角色的成员的用户。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdc8a-128">关系</span><span class="sxs-lookup"><span data-stu-id="cdc8a-128">Relationships</span></span>
<span data-ttu-id="cdc8a-129">无</span><span class="sxs-lookup"><span data-stu-id="cdc8a-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cdc8a-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cdc8a-130">JSON representation</span></span>

<span data-ttu-id="cdc8a-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdc8a-131">Here is a JSON representation of the resource.</span></span>

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
