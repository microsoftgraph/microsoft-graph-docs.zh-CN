---
title: scopedRoleMembership 资源类型
description: 作用域角色成员资格介绍目录角色，进一步范围限定到管理单元 (AU) 的用户的成员的身份。  这提供了一种机制，以允许租户范围公司 adminsistrator 以委派用户管理用户和组的子集组织 （由 AU 正在定义的子集） 的管理权限。
ms.openlocfilehash: bd635a5b1b06b98657ba24c397e2f67afb76fa8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044794"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="dd3bf-104">scopedRoleMembership 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd3bf-104">scopedRoleMembership resource type</span></span>

> <span data-ttu-id="dd3bf-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd3bf-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd3bf-107">作用域角色成员资格介绍目录角色，进一步范围限定到管理单元 (AU) 的用户的成员的身份。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-107">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="dd3bf-108">这提供了一种机制，以允许租户范围公司 adminsistrator 以委派用户管理用户和组的子集组织 （由 AU 正在定义的子集） 的管理权限。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-108">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="dd3bf-109">方法</span><span class="sxs-lookup"><span data-stu-id="dd3bf-109">Methods</span></span>
<span data-ttu-id="dd3bf-110">不支持直接查询到此资源。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-110">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="dd3bf-111">请参阅[管理单元](administrativeunit.md)主题，若要查看有关如何查询范围角色成员身份，以及添加和移除范围角色成员身份信息。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-111">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="dd3bf-112">属性</span><span class="sxs-lookup"><span data-stu-id="dd3bf-112">Properties</span></span>
| <span data-ttu-id="dd3bf-113">属性</span><span class="sxs-lookup"><span data-stu-id="dd3bf-113">Property</span></span>   | <span data-ttu-id="dd3bf-114">类型</span><span class="sxs-lookup"><span data-stu-id="dd3bf-114">Type</span></span> | <span data-ttu-id="dd3bf-115">说明</span><span class="sxs-lookup"><span data-stu-id="dd3bf-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dd3bf-116">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="dd3bf-116">administrativeUnitId</span></span>|<span data-ttu-id="dd3bf-117">string</span><span class="sxs-lookup"><span data-stu-id="dd3bf-117">string</span></span>|<span data-ttu-id="dd3bf-118">唯一标识符的目录角色范围限定为管理单元</span><span class="sxs-lookup"><span data-stu-id="dd3bf-118">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="dd3bf-119">id</span><span class="sxs-lookup"><span data-stu-id="dd3bf-119">id</span></span>|<span data-ttu-id="dd3bf-120">string</span><span class="sxs-lookup"><span data-stu-id="dd3bf-120">string</span></span>| <span data-ttu-id="dd3bf-121">作用域角色成员身份的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-121">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="dd3bf-122">只读。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-122">Read-only.</span></span>|
|<span data-ttu-id="dd3bf-123">roleId</span><span class="sxs-lookup"><span data-stu-id="dd3bf-123">roleId</span></span>|<span data-ttu-id="dd3bf-124">string</span><span class="sxs-lookup"><span data-stu-id="dd3bf-124">string</span></span>| <span data-ttu-id="dd3bf-125">为目录角色中的成员的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-125">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="dd3bf-126">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="dd3bf-126">roleMemberInfo</span></span>|[<span data-ttu-id="dd3bf-127">identity</span><span class="sxs-lookup"><span data-stu-id="dd3bf-127">identity</span></span>](identity.md)| <span data-ttu-id="dd3bf-128">角色成员身份信息。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-128">Role member identity information.</span></span> <span data-ttu-id="dd3bf-129">表示此作用域角色的成员的用户。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-129">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd3bf-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="dd3bf-130">Relationships</span></span>
<span data-ttu-id="dd3bf-131">无</span><span class="sxs-lookup"><span data-stu-id="dd3bf-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd3bf-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd3bf-132">JSON representation</span></span>

<span data-ttu-id="dd3bf-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd3bf-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->