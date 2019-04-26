---
title: privilegedRole 资源类型
description: 表示 Azure AD 管理员角色, 例如:**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563399"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="f47e5-103">privilegedRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="f47e5-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47e5-104">表示 Azure AD 管理员角色, 例如:**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。</span><span class="sxs-lookup"><span data-stu-id="f47e5-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="f47e5-105">方法</span><span class="sxs-lookup"><span data-stu-id="f47e5-105">Methods</span></span>

| <span data-ttu-id="f47e5-106">方法</span><span class="sxs-lookup"><span data-stu-id="f47e5-106">Method</span></span>           | <span data-ttu-id="f47e5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f47e5-107">Return Type</span></span>    |<span data-ttu-id="f47e5-108">说明</span><span class="sxs-lookup"><span data-stu-id="f47e5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f47e5-109">列出 privilegedRole 对象</span><span class="sxs-lookup"><span data-stu-id="f47e5-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="f47e5-110">[privilegedRole](privilegedrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f47e5-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="f47e5-111">获取 privilegedRole 的集合。</span><span class="sxs-lookup"><span data-stu-id="f47e5-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="f47e5-112">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f47e5-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="f47e5-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f47e5-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="f47e5-114">读取 privilegedRole 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f47e5-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="f47e5-115">列出作业</span><span class="sxs-lookup"><span data-stu-id="f47e5-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="f47e5-116">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f47e5-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="f47e5-117">获取此角色的工作分配对象集合。</span><span class="sxs-lookup"><span data-stu-id="f47e5-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="f47e5-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="f47e5-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="f47e5-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f47e5-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="f47e5-120">激活分配的角色。</span><span class="sxs-lookup"><span data-stu-id="f47e5-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="f47e5-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="f47e5-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="f47e5-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f47e5-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="f47e5-123">停用分配的角色。</span><span class="sxs-lookup"><span data-stu-id="f47e5-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="f47e5-124">属性</span><span class="sxs-lookup"><span data-stu-id="f47e5-124">Properties</span></span>
| <span data-ttu-id="f47e5-125">属性</span><span class="sxs-lookup"><span data-stu-id="f47e5-125">Property</span></span>     | <span data-ttu-id="f47e5-126">类型</span><span class="sxs-lookup"><span data-stu-id="f47e5-126">Type</span></span>   |<span data-ttu-id="f47e5-127">说明</span><span class="sxs-lookup"><span data-stu-id="f47e5-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f47e5-128">id</span><span class="sxs-lookup"><span data-stu-id="f47e5-128">id</span></span>|<span data-ttu-id="f47e5-129">string</span><span class="sxs-lookup"><span data-stu-id="f47e5-129">string</span></span>|<span data-ttu-id="f47e5-130">管理员角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f47e5-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="f47e5-131">它是一个 GUID 字符串, 与给定角色的 Azure AD 中的角色模板 id 具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="f47e5-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="f47e5-132">只读。</span><span class="sxs-lookup"><span data-stu-id="f47e5-132">Read-only.</span></span>|
|<span data-ttu-id="f47e5-133">name</span><span class="sxs-lookup"><span data-stu-id="f47e5-133">name</span></span>|<span data-ttu-id="f47e5-134">string</span><span class="sxs-lookup"><span data-stu-id="f47e5-134">string</span></span>|<span data-ttu-id="f47e5-135">角色名称。</span><span class="sxs-lookup"><span data-stu-id="f47e5-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f47e5-136">关系</span><span class="sxs-lookup"><span data-stu-id="f47e5-136">Relationships</span></span>
| <span data-ttu-id="f47e5-137">关系</span><span class="sxs-lookup"><span data-stu-id="f47e5-137">Relationship</span></span> | <span data-ttu-id="f47e5-138">类型</span><span class="sxs-lookup"><span data-stu-id="f47e5-138">Type</span></span>   |<span data-ttu-id="f47e5-139">说明</span><span class="sxs-lookup"><span data-stu-id="f47e5-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f47e5-140">assignments</span><span class="sxs-lookup"><span data-stu-id="f47e5-140">assignments</span></span>|<span data-ttu-id="f47e5-141">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f47e5-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="f47e5-142">此角色的分配。</span><span class="sxs-lookup"><span data-stu-id="f47e5-142">The assignments for this role.</span></span> <span data-ttu-id="f47e5-143">只读。</span><span class="sxs-lookup"><span data-stu-id="f47e5-143">Read-only.</span></span> <span data-ttu-id="f47e5-144">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f47e5-144">Nullable.</span></span>|
|<span data-ttu-id="f47e5-145">settings</span><span class="sxs-lookup"><span data-stu-id="f47e5-145">settings</span></span>|[<span data-ttu-id="f47e5-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="f47e5-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="f47e5-147">此角色的设置。</span><span class="sxs-lookup"><span data-stu-id="f47e5-147">The settings for this role.</span></span> <span data-ttu-id="f47e5-148">只读。</span><span class="sxs-lookup"><span data-stu-id="f47e5-148">Read-only.</span></span> <span data-ttu-id="f47e5-149">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f47e5-149">Nullable.</span></span>|
|<span data-ttu-id="f47e5-150">摘要</span><span class="sxs-lookup"><span data-stu-id="f47e5-150">summary</span></span>|[<span data-ttu-id="f47e5-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="f47e5-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="f47e5-152">此角色的摘要信息。</span><span class="sxs-lookup"><span data-stu-id="f47e5-152">The summary information for this role.</span></span> <span data-ttu-id="f47e5-153">只读。</span><span class="sxs-lookup"><span data-stu-id="f47e5-153">Read-only.</span></span> <span data-ttu-id="f47e5-154">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f47e5-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f47e5-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f47e5-155">JSON representation</span></span>

<span data-ttu-id="f47e5-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f47e5-156">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
