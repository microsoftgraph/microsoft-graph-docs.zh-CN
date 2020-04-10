---
title: privilegedRole 资源类型
description: 表示 Azure AD 管理员角色，例如：**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 51114eea797d27886f48c664d06d0b88d4a35a2d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217909"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="b7e68-103">privilegedRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7e68-103">privilegedRole resource type</span></span>

<span data-ttu-id="b7e68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7e68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7e68-105">表示 Azure AD 管理员角色，例如：**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。</span><span class="sxs-lookup"><span data-stu-id="b7e68-105">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="b7e68-106">Methods</span><span class="sxs-lookup"><span data-stu-id="b7e68-106">Methods</span></span>

| <span data-ttu-id="b7e68-107">方法</span><span class="sxs-lookup"><span data-stu-id="b7e68-107">Method</span></span>           | <span data-ttu-id="b7e68-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7e68-108">Return Type</span></span>    |<span data-ttu-id="b7e68-109">说明</span><span class="sxs-lookup"><span data-stu-id="b7e68-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7e68-110">列出 privilegedRole 对象</span><span class="sxs-lookup"><span data-stu-id="b7e68-110">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="b7e68-111">[privilegedRole](privilegedrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7e68-111">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="b7e68-112">获取 privilegedRole 的集合。</span><span class="sxs-lookup"><span data-stu-id="b7e68-112">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="b7e68-113">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="b7e68-113">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="b7e68-114">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="b7e68-114">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="b7e68-115">读取 privilegedRole 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7e68-115">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="b7e68-116">列出作业</span><span class="sxs-lookup"><span data-stu-id="b7e68-116">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="b7e68-117">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7e68-117">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="b7e68-118">获取此角色的工作分配对象集合。</span><span class="sxs-lookup"><span data-stu-id="b7e68-118">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="b7e68-119">selfActivate</span><span class="sxs-lookup"><span data-stu-id="b7e68-119">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="b7e68-120">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b7e68-120">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="b7e68-121">激活分配的角色。</span><span class="sxs-lookup"><span data-stu-id="b7e68-121">Activate the assigned role.</span></span>|
|[<span data-ttu-id="b7e68-122">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="b7e68-122">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="b7e68-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b7e68-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="b7e68-124">停用分配的角色。</span><span class="sxs-lookup"><span data-stu-id="b7e68-124">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7e68-125">属性</span><span class="sxs-lookup"><span data-stu-id="b7e68-125">Properties</span></span>
| <span data-ttu-id="b7e68-126">属性</span><span class="sxs-lookup"><span data-stu-id="b7e68-126">Property</span></span>     | <span data-ttu-id="b7e68-127">类型</span><span class="sxs-lookup"><span data-stu-id="b7e68-127">Type</span></span>   |<span data-ttu-id="b7e68-128">说明</span><span class="sxs-lookup"><span data-stu-id="b7e68-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7e68-129">id</span><span class="sxs-lookup"><span data-stu-id="b7e68-129">id</span></span>|<span data-ttu-id="b7e68-130">string</span><span class="sxs-lookup"><span data-stu-id="b7e68-130">string</span></span>|<span data-ttu-id="b7e68-131">管理员角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b7e68-131">The unique identifier for administrator role.</span></span> <span data-ttu-id="b7e68-132">它是一个 GUID 字符串，与给定角色的 Azure AD 中的角色模板 id 具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="b7e68-132">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="b7e68-133">只读。</span><span class="sxs-lookup"><span data-stu-id="b7e68-133">Read-only.</span></span>|
|<span data-ttu-id="b7e68-134">name</span><span class="sxs-lookup"><span data-stu-id="b7e68-134">name</span></span>|<span data-ttu-id="b7e68-135">string</span><span class="sxs-lookup"><span data-stu-id="b7e68-135">string</span></span>|<span data-ttu-id="b7e68-136">角色名称。</span><span class="sxs-lookup"><span data-stu-id="b7e68-136">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7e68-137">关系</span><span class="sxs-lookup"><span data-stu-id="b7e68-137">Relationships</span></span>
| <span data-ttu-id="b7e68-138">关系</span><span class="sxs-lookup"><span data-stu-id="b7e68-138">Relationship</span></span> | <span data-ttu-id="b7e68-139">类型</span><span class="sxs-lookup"><span data-stu-id="b7e68-139">Type</span></span>   |<span data-ttu-id="b7e68-140">说明</span><span class="sxs-lookup"><span data-stu-id="b7e68-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7e68-141">assignments</span><span class="sxs-lookup"><span data-stu-id="b7e68-141">assignments</span></span>|<span data-ttu-id="b7e68-142">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7e68-142">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="b7e68-143">此角色的分配。</span><span class="sxs-lookup"><span data-stu-id="b7e68-143">The assignments for this role.</span></span> <span data-ttu-id="b7e68-144">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="b7e68-144">Read-only.</span></span> <span data-ttu-id="b7e68-145">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b7e68-145">Nullable.</span></span>|
|<span data-ttu-id="b7e68-146">settings</span><span class="sxs-lookup"><span data-stu-id="b7e68-146">settings</span></span>|[<span data-ttu-id="b7e68-147">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="b7e68-147">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="b7e68-148">此角色的设置。</span><span class="sxs-lookup"><span data-stu-id="b7e68-148">The settings for this role.</span></span> <span data-ttu-id="b7e68-149">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="b7e68-149">Read-only.</span></span> <span data-ttu-id="b7e68-150">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b7e68-150">Nullable.</span></span>|
|<span data-ttu-id="b7e68-151">摘要</span><span class="sxs-lookup"><span data-stu-id="b7e68-151">summary</span></span>|[<span data-ttu-id="b7e68-152">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="b7e68-152">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="b7e68-153">此角色的摘要信息。</span><span class="sxs-lookup"><span data-stu-id="b7e68-153">The summary information for this role.</span></span> <span data-ttu-id="b7e68-154">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="b7e68-154">Read-only.</span></span> <span data-ttu-id="b7e68-155">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b7e68-155">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7e68-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7e68-156">JSON representation</span></span>

<span data-ttu-id="b7e68-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7e68-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
