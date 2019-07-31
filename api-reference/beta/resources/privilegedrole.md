---
title: privilegedRole 资源类型
description: 表示 Azure AD 管理员角色, 例如:**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 98e5cd2c53b398339e8db65bec520a16f72d8f39
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965745"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="94202-103">privilegedRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="94202-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94202-104">表示 Azure AD 管理员角色, 例如:**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。</span><span class="sxs-lookup"><span data-stu-id="94202-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="94202-105">方法</span><span class="sxs-lookup"><span data-stu-id="94202-105">Methods</span></span>

| <span data-ttu-id="94202-106">方法</span><span class="sxs-lookup"><span data-stu-id="94202-106">Method</span></span>           | <span data-ttu-id="94202-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="94202-107">Return Type</span></span>    |<span data-ttu-id="94202-108">说明</span><span class="sxs-lookup"><span data-stu-id="94202-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94202-109">列出 privilegedRole 对象</span><span class="sxs-lookup"><span data-stu-id="94202-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="94202-110">[privilegedRole](privilegedrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94202-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="94202-111">获取 privilegedRole 的集合。</span><span class="sxs-lookup"><span data-stu-id="94202-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="94202-112">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="94202-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="94202-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="94202-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="94202-114">读取 privilegedRole 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94202-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="94202-115">列出作业</span><span class="sxs-lookup"><span data-stu-id="94202-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="94202-116">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94202-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="94202-117">获取此角色的工作分配对象集合。</span><span class="sxs-lookup"><span data-stu-id="94202-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="94202-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="94202-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="94202-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="94202-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="94202-120">激活分配的角色。</span><span class="sxs-lookup"><span data-stu-id="94202-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="94202-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="94202-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="94202-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="94202-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="94202-123">停用分配的角色。</span><span class="sxs-lookup"><span data-stu-id="94202-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="94202-124">属性</span><span class="sxs-lookup"><span data-stu-id="94202-124">Properties</span></span>
| <span data-ttu-id="94202-125">属性</span><span class="sxs-lookup"><span data-stu-id="94202-125">Property</span></span>     | <span data-ttu-id="94202-126">类型</span><span class="sxs-lookup"><span data-stu-id="94202-126">Type</span></span>   |<span data-ttu-id="94202-127">说明</span><span class="sxs-lookup"><span data-stu-id="94202-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94202-128">id</span><span class="sxs-lookup"><span data-stu-id="94202-128">id</span></span>|<span data-ttu-id="94202-129">string</span><span class="sxs-lookup"><span data-stu-id="94202-129">string</span></span>|<span data-ttu-id="94202-130">管理员角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="94202-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="94202-131">它是一个 GUID 字符串, 与给定角色的 Azure AD 中的角色模板 id 具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="94202-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="94202-132">只读。</span><span class="sxs-lookup"><span data-stu-id="94202-132">Read-only.</span></span>|
|<span data-ttu-id="94202-133">name</span><span class="sxs-lookup"><span data-stu-id="94202-133">name</span></span>|<span data-ttu-id="94202-134">string</span><span class="sxs-lookup"><span data-stu-id="94202-134">string</span></span>|<span data-ttu-id="94202-135">角色名称。</span><span class="sxs-lookup"><span data-stu-id="94202-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94202-136">关系</span><span class="sxs-lookup"><span data-stu-id="94202-136">Relationships</span></span>
| <span data-ttu-id="94202-137">关系</span><span class="sxs-lookup"><span data-stu-id="94202-137">Relationship</span></span> | <span data-ttu-id="94202-138">类型</span><span class="sxs-lookup"><span data-stu-id="94202-138">Type</span></span>   |<span data-ttu-id="94202-139">说明</span><span class="sxs-lookup"><span data-stu-id="94202-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94202-140">assignments</span><span class="sxs-lookup"><span data-stu-id="94202-140">assignments</span></span>|<span data-ttu-id="94202-141">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94202-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="94202-142">此角色的分配。</span><span class="sxs-lookup"><span data-stu-id="94202-142">The assignments for this role.</span></span> <span data-ttu-id="94202-143">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="94202-143">Read-only.</span></span> <span data-ttu-id="94202-144">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="94202-144">Nullable.</span></span>|
|<span data-ttu-id="94202-145">settings</span><span class="sxs-lookup"><span data-stu-id="94202-145">settings</span></span>|[<span data-ttu-id="94202-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="94202-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="94202-147">此角色的设置。</span><span class="sxs-lookup"><span data-stu-id="94202-147">The settings for this role.</span></span> <span data-ttu-id="94202-148">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="94202-148">Read-only.</span></span> <span data-ttu-id="94202-149">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="94202-149">Nullable.</span></span>|
|<span data-ttu-id="94202-150">摘要</span><span class="sxs-lookup"><span data-stu-id="94202-150">summary</span></span>|[<span data-ttu-id="94202-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="94202-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="94202-152">此角色的摘要信息。</span><span class="sxs-lookup"><span data-stu-id="94202-152">The summary information for this role.</span></span> <span data-ttu-id="94202-153">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="94202-153">Read-only.</span></span> <span data-ttu-id="94202-154">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="94202-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94202-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94202-155">JSON representation</span></span>

<span data-ttu-id="94202-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94202-156">Here is a JSON representation of the resource.</span></span>

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
