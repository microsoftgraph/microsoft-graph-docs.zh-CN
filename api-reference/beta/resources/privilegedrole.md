---
title: privilegedRole 资源类型
description: 表示 Azure AD 管理员角色，如：**全局管理员、 帐单管理员、 服务管理员、 用户管理员、 密码管理员**等。
localization_priority: Normal
ms.openlocfilehash: 75763e18731cb969623cc4df6360d50abc018b41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860856"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="907e3-103">privilegedRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="907e3-103">privilegedRole resource type</span></span>

> <span data-ttu-id="907e3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="907e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="907e3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="907e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="907e3-106">表示 Azure AD 管理员角色，如：**全局管理员、 帐单管理员、 服务管理员、 用户管理员、 密码管理员**等。</span><span class="sxs-lookup"><span data-stu-id="907e3-106">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="907e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="907e3-107">Methods</span></span>

| <span data-ttu-id="907e3-108">方法</span><span class="sxs-lookup"><span data-stu-id="907e3-108">Method</span></span>           | <span data-ttu-id="907e3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="907e3-109">Return Type</span></span>    |<span data-ttu-id="907e3-110">说明</span><span class="sxs-lookup"><span data-stu-id="907e3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="907e3-111">列表 privilegedRole 对象</span><span class="sxs-lookup"><span data-stu-id="907e3-111">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="907e3-112">[privilegedRole](privilegedrole.md)集合</span><span class="sxs-lookup"><span data-stu-id="907e3-112">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="907e3-113">获取 privilegedRole 的集合。</span><span class="sxs-lookup"><span data-stu-id="907e3-113">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="907e3-114">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="907e3-114">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="907e3-115">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="907e3-115">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="907e3-116">读取属性和 privilegedRole 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="907e3-116">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="907e3-117">列表分配</span><span class="sxs-lookup"><span data-stu-id="907e3-117">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="907e3-118">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="907e3-118">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="907e3-119">获取此角色分配对象集合。</span><span class="sxs-lookup"><span data-stu-id="907e3-119">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="907e3-120">selfActivate</span><span class="sxs-lookup"><span data-stu-id="907e3-120">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="907e3-121">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="907e3-121">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="907e3-122">激活分配的角色。</span><span class="sxs-lookup"><span data-stu-id="907e3-122">Activate the assigned role.</span></span>|
|[<span data-ttu-id="907e3-123">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="907e3-123">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="907e3-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="907e3-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="907e3-125">停用分配的角色。</span><span class="sxs-lookup"><span data-stu-id="907e3-125">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="907e3-126">属性</span><span class="sxs-lookup"><span data-stu-id="907e3-126">Properties</span></span>
| <span data-ttu-id="907e3-127">属性</span><span class="sxs-lookup"><span data-stu-id="907e3-127">Property</span></span>     | <span data-ttu-id="907e3-128">类型</span><span class="sxs-lookup"><span data-stu-id="907e3-128">Type</span></span>   |<span data-ttu-id="907e3-129">说明</span><span class="sxs-lookup"><span data-stu-id="907e3-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="907e3-130">ID</span><span class="sxs-lookup"><span data-stu-id="907e3-130">id</span></span>|<span data-ttu-id="907e3-131">string</span><span class="sxs-lookup"><span data-stu-id="907e3-131">string</span></span>|<span data-ttu-id="907e3-132">管理员角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="907e3-132">The unique identifier for administrator role.</span></span> <span data-ttu-id="907e3-133">它是一个 GUID 的字符串，并且具有相同的值从给定角色的 Azure AD 的角色模板 id。</span><span class="sxs-lookup"><span data-stu-id="907e3-133">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="907e3-134">只读。</span><span class="sxs-lookup"><span data-stu-id="907e3-134">Read-only.</span></span>|
|<span data-ttu-id="907e3-135">name</span><span class="sxs-lookup"><span data-stu-id="907e3-135">name</span></span>|<span data-ttu-id="907e3-136">string</span><span class="sxs-lookup"><span data-stu-id="907e3-136">string</span></span>|<span data-ttu-id="907e3-137">角色名称。</span><span class="sxs-lookup"><span data-stu-id="907e3-137">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="907e3-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="907e3-138">Relationships</span></span>
| <span data-ttu-id="907e3-139">关系</span><span class="sxs-lookup"><span data-stu-id="907e3-139">Relationship</span></span> | <span data-ttu-id="907e3-140">类型</span><span class="sxs-lookup"><span data-stu-id="907e3-140">Type</span></span>   |<span data-ttu-id="907e3-141">说明</span><span class="sxs-lookup"><span data-stu-id="907e3-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="907e3-142">assignments</span><span class="sxs-lookup"><span data-stu-id="907e3-142">assignments</span></span>|<span data-ttu-id="907e3-143">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="907e3-143">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="907e3-144">此角色分配。</span><span class="sxs-lookup"><span data-stu-id="907e3-144">The assignments for this role.</span></span> <span data-ttu-id="907e3-145">只读。</span><span class="sxs-lookup"><span data-stu-id="907e3-145">Read-only.</span></span> <span data-ttu-id="907e3-146">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="907e3-146">Nullable.</span></span>|
|<span data-ttu-id="907e3-147">settings</span><span class="sxs-lookup"><span data-stu-id="907e3-147">settings</span></span>|[<span data-ttu-id="907e3-148">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="907e3-148">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="907e3-149">此角色的设置。</span><span class="sxs-lookup"><span data-stu-id="907e3-149">The settings for this role.</span></span> <span data-ttu-id="907e3-150">只读。</span><span class="sxs-lookup"><span data-stu-id="907e3-150">Read-only.</span></span> <span data-ttu-id="907e3-151">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="907e3-151">Nullable.</span></span>|
|<span data-ttu-id="907e3-152">摘要</span><span class="sxs-lookup"><span data-stu-id="907e3-152">summary</span></span>|[<span data-ttu-id="907e3-153">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="907e3-153">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="907e3-154">此角色的摘要信息。</span><span class="sxs-lookup"><span data-stu-id="907e3-154">The summary information for this role.</span></span> <span data-ttu-id="907e3-155">只读。</span><span class="sxs-lookup"><span data-stu-id="907e3-155">Read-only.</span></span> <span data-ttu-id="907e3-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="907e3-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="907e3-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="907e3-157">JSON representation</span></span>

<span data-ttu-id="907e3-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="907e3-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
