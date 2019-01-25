---
title: privilegedRole 资源类型
description: 表示 Azure AD 管理员角色，如：**全局管理员、 帐单管理员、 服务管理员、 用户管理员、 密码管理员**等。
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513744"
---
# <a name="privilegedrole-resource-type"></a><span data-ttu-id="df8f7-103">privilegedRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="df8f7-103">privilegedRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df8f7-104">表示 Azure AD 管理员角色，如：**全局管理员、 帐单管理员、 服务管理员、 用户管理员、 密码管理员**等。</span><span class="sxs-lookup"><span data-stu-id="df8f7-104">Represents an Azure AD administrator role, such as: **Global Administrator, Billing Administrator, Service Administrator, User Administrator, Password Administrator**, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="df8f7-105">方法</span><span class="sxs-lookup"><span data-stu-id="df8f7-105">Methods</span></span>

| <span data-ttu-id="df8f7-106">方法</span><span class="sxs-lookup"><span data-stu-id="df8f7-106">Method</span></span>           | <span data-ttu-id="df8f7-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="df8f7-107">Return Type</span></span>    |<span data-ttu-id="df8f7-108">说明</span><span class="sxs-lookup"><span data-stu-id="df8f7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df8f7-109">列表 privilegedRole 对象</span><span class="sxs-lookup"><span data-stu-id="df8f7-109">List privilegedRole objects</span></span>](../api/privilegedrole-list.md) | <span data-ttu-id="df8f7-110">[privilegedRole](privilegedrole.md)集合</span><span class="sxs-lookup"><span data-stu-id="df8f7-110">[privilegedRole](privilegedrole.md) collection</span></span>|<span data-ttu-id="df8f7-111">获取 privilegedRole 的集合。</span><span class="sxs-lookup"><span data-stu-id="df8f7-111">Get the collection of privilegedRole.</span></span>|
|[<span data-ttu-id="df8f7-112">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="df8f7-112">Get privilegedRole</span></span>](../api/privilegedrole-get.md) | [<span data-ttu-id="df8f7-113">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="df8f7-113">privilegedRole</span></span>](privilegedrole.md) |<span data-ttu-id="df8f7-114">读取属性和 privilegedRole 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="df8f7-114">Read properties and relationships of privilegedRole object.</span></span>|
|[<span data-ttu-id="df8f7-115">列表分配</span><span class="sxs-lookup"><span data-stu-id="df8f7-115">List assignments</span></span>](../api/privilegedrole-list-assignments.md) |<span data-ttu-id="df8f7-116">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="df8f7-116">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="df8f7-117">获取此角色分配对象集合。</span><span class="sxs-lookup"><span data-stu-id="df8f7-117">Get a assignment object collection for this role.</span></span>|
|[<span data-ttu-id="df8f7-118">selfActivate</span><span class="sxs-lookup"><span data-stu-id="df8f7-118">selfActivate</span></span>](../api/privilegedrole-selfactivate.md)|[<span data-ttu-id="df8f7-119">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="df8f7-119">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="df8f7-120">激活分配的角色。</span><span class="sxs-lookup"><span data-stu-id="df8f7-120">Activate the assigned role.</span></span>|
|[<span data-ttu-id="df8f7-121">selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="df8f7-121">selfDeactivate</span></span>](../api/privilegedrole-selfdeactivate.md)|[<span data-ttu-id="df8f7-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="df8f7-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="df8f7-123">停用分配的角色。</span><span class="sxs-lookup"><span data-stu-id="df8f7-123">Deactivate the assigned role.</span></span>|

## <a name="properties"></a><span data-ttu-id="df8f7-124">属性</span><span class="sxs-lookup"><span data-stu-id="df8f7-124">Properties</span></span>
| <span data-ttu-id="df8f7-125">属性</span><span class="sxs-lookup"><span data-stu-id="df8f7-125">Property</span></span>     | <span data-ttu-id="df8f7-126">类型</span><span class="sxs-lookup"><span data-stu-id="df8f7-126">Type</span></span>   |<span data-ttu-id="df8f7-127">说明</span><span class="sxs-lookup"><span data-stu-id="df8f7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df8f7-128">id</span><span class="sxs-lookup"><span data-stu-id="df8f7-128">id</span></span>|<span data-ttu-id="df8f7-129">string</span><span class="sxs-lookup"><span data-stu-id="df8f7-129">string</span></span>|<span data-ttu-id="df8f7-130">管理员角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="df8f7-130">The unique identifier for administrator role.</span></span> <span data-ttu-id="df8f7-131">它是一个 GUID 的字符串，并且具有相同的值从给定角色的 Azure AD 的角色模板 id。</span><span class="sxs-lookup"><span data-stu-id="df8f7-131">It is a GUID string and has the same value as the role template id from Azure AD for the given role.</span></span> <span data-ttu-id="df8f7-132">只读。</span><span class="sxs-lookup"><span data-stu-id="df8f7-132">Read-only.</span></span>|
|<span data-ttu-id="df8f7-133">name</span><span class="sxs-lookup"><span data-stu-id="df8f7-133">name</span></span>|<span data-ttu-id="df8f7-134">string</span><span class="sxs-lookup"><span data-stu-id="df8f7-134">string</span></span>|<span data-ttu-id="df8f7-135">角色名称。</span><span class="sxs-lookup"><span data-stu-id="df8f7-135">Role name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df8f7-136">关系</span><span class="sxs-lookup"><span data-stu-id="df8f7-136">Relationships</span></span>
| <span data-ttu-id="df8f7-137">关系</span><span class="sxs-lookup"><span data-stu-id="df8f7-137">Relationship</span></span> | <span data-ttu-id="df8f7-138">类型</span><span class="sxs-lookup"><span data-stu-id="df8f7-138">Type</span></span>   |<span data-ttu-id="df8f7-139">说明</span><span class="sxs-lookup"><span data-stu-id="df8f7-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df8f7-140">assignments</span><span class="sxs-lookup"><span data-stu-id="df8f7-140">assignments</span></span>|<span data-ttu-id="df8f7-141">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="df8f7-141">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>| <span data-ttu-id="df8f7-142">此角色分配。</span><span class="sxs-lookup"><span data-stu-id="df8f7-142">The assignments for this role.</span></span> <span data-ttu-id="df8f7-143">只读。</span><span class="sxs-lookup"><span data-stu-id="df8f7-143">Read-only.</span></span> <span data-ttu-id="df8f7-144">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="df8f7-144">Nullable.</span></span>|
|<span data-ttu-id="df8f7-145">settings</span><span class="sxs-lookup"><span data-stu-id="df8f7-145">settings</span></span>|[<span data-ttu-id="df8f7-146">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="df8f7-146">privilegedRoleSettings</span></span>](privilegedrolesettings.md)| <span data-ttu-id="df8f7-147">此角色的设置。</span><span class="sxs-lookup"><span data-stu-id="df8f7-147">The settings for this role.</span></span> <span data-ttu-id="df8f7-148">只读。</span><span class="sxs-lookup"><span data-stu-id="df8f7-148">Read-only.</span></span> <span data-ttu-id="df8f7-149">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="df8f7-149">Nullable.</span></span>|
|<span data-ttu-id="df8f7-150">摘要</span><span class="sxs-lookup"><span data-stu-id="df8f7-150">summary</span></span>|[<span data-ttu-id="df8f7-151">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="df8f7-151">privilegedRoleSummary</span></span>](privilegedrolesummary.md)| <span data-ttu-id="df8f7-152">此角色的摘要信息。</span><span class="sxs-lookup"><span data-stu-id="df8f7-152">The summary information for this role.</span></span> <span data-ttu-id="df8f7-153">只读。</span><span class="sxs-lookup"><span data-stu-id="df8f7-153">Read-only.</span></span> <span data-ttu-id="df8f7-154">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="df8f7-154">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df8f7-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df8f7-155">JSON representation</span></span>

<span data-ttu-id="df8f7-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df8f7-156">Here is a JSON representation of the resource.</span></span>

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
