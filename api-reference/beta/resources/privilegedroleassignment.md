---
title: privilegedRoleAssignment 资源类型
description: '表示特定用户特权的角色分配。 '
localization_priority: Normal
ms.openlocfilehash: ec6bc34ecd56839c764592ff298475e8648f300b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823315"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="59689-103">privilegedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="59689-103">privilegedRoleAssignment resource type</span></span>

> <span data-ttu-id="59689-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="59689-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59689-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="59689-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59689-106">表示特定用户特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="59689-106">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="59689-107">方法</span><span class="sxs-lookup"><span data-stu-id="59689-107">Methods</span></span>

| <span data-ttu-id="59689-108">方法</span><span class="sxs-lookup"><span data-stu-id="59689-108">Method</span></span>           | <span data-ttu-id="59689-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="59689-109">Return Type</span></span>    |<span data-ttu-id="59689-110">说明</span><span class="sxs-lookup"><span data-stu-id="59689-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="59689-111">列表 privilegedRoleAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="59689-111">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="59689-112">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="59689-112">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="59689-113">获取 privilegedRoleAssignment 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="59689-113">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="59689-114">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="59689-114">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="59689-115">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="59689-115">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="59689-116">读取属性和 privilegedRoleAssignment 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="59689-116">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="59689-117">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="59689-117">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="59689-118">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="59689-118">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="59689-119">通过发布到 assignments 集合中创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="59689-119">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="59689-120">删除</span><span class="sxs-lookup"><span data-stu-id="59689-120">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="59689-121">无</span><span class="sxs-lookup"><span data-stu-id="59689-121">None</span></span> |<span data-ttu-id="59689-122">删除 privilegedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="59689-122">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="59689-123">makePermanent</span><span class="sxs-lookup"><span data-stu-id="59689-123">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="59689-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="59689-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="59689-125">请为永久的角色分配。</span><span class="sxs-lookup"><span data-stu-id="59689-125">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="59689-126">makeEligible</span><span class="sxs-lookup"><span data-stu-id="59689-126">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="59689-127">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="59689-127">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="59689-128">请作为合格的角色分配。</span><span class="sxs-lookup"><span data-stu-id="59689-128">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="59689-129">我</span><span class="sxs-lookup"><span data-stu-id="59689-129">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="59689-130">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="59689-130">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="59689-131">获取当前用户的特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="59689-131">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="59689-132">属性</span><span class="sxs-lookup"><span data-stu-id="59689-132">Properties</span></span>
| <span data-ttu-id="59689-133">属性</span><span class="sxs-lookup"><span data-stu-id="59689-133">Property</span></span>     | <span data-ttu-id="59689-134">类型</span><span class="sxs-lookup"><span data-stu-id="59689-134">Type</span></span>   |<span data-ttu-id="59689-135">说明</span><span class="sxs-lookup"><span data-stu-id="59689-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59689-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="59689-136">expirationDateTime</span></span>|<span data-ttu-id="59689-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59689-137">dateTimeOffset</span></span>|<span data-ttu-id="59689-138">UTC DateTime 时将过期的临时特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="59689-138">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="59689-139">永久角色分配的值为 null。</span><span class="sxs-lookup"><span data-stu-id="59689-139">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="59689-140">id</span><span class="sxs-lookup"><span data-stu-id="59689-140">id</span></span>|<span data-ttu-id="59689-141">string</span><span class="sxs-lookup"><span data-stu-id="59689-141">string</span></span>| <span data-ttu-id="59689-142">特权的角色分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="59689-142">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="59689-143">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="59689-143">Read-only.</span></span> <span data-ttu-id="59689-144">处于 userId_roleId，其中 userId 是 Azure AD 用户 id 的 GUID 字符串，roleId 是 Azure 管理员角色 id 的 GUID 字符串的格式。</span><span class="sxs-lookup"><span data-stu-id="59689-144">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="59689-145">isElevated</span><span class="sxs-lookup"><span data-stu-id="59689-145">isElevated</span></span>|<span data-ttu-id="59689-146">boolean</span><span class="sxs-lookup"><span data-stu-id="59689-146">boolean</span></span>|<span data-ttu-id="59689-147">**true**如果激活该角色分配。</span><span class="sxs-lookup"><span data-stu-id="59689-147">**true** if the role assignment is activated.</span></span> <span data-ttu-id="59689-148">**false**如果停用的角色分配。</span><span class="sxs-lookup"><span data-stu-id="59689-148">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="59689-149">resultMessage</span><span class="sxs-lookup"><span data-stu-id="59689-149">resultMessage</span></span>|<span data-ttu-id="59689-150">string</span><span class="sxs-lookup"><span data-stu-id="59689-150">string</span></span>|<span data-ttu-id="59689-151">结果消息由服务设置。</span><span class="sxs-lookup"><span data-stu-id="59689-151">Result message set by the service.</span></span>|
|<span data-ttu-id="59689-152">roleId</span><span class="sxs-lookup"><span data-stu-id="59689-152">roleId</span></span>|<span data-ttu-id="59689-153">string</span><span class="sxs-lookup"><span data-stu-id="59689-153">string</span></span>|<span data-ttu-id="59689-154">角色标识符。</span><span class="sxs-lookup"><span data-stu-id="59689-154">Role identifier.</span></span> <span data-ttu-id="59689-155">格式字符串 GUID。</span><span class="sxs-lookup"><span data-stu-id="59689-155">In GUID string format.</span></span>|
|<span data-ttu-id="59689-156">userId</span><span class="sxs-lookup"><span data-stu-id="59689-156">userId</span></span>|<span data-ttu-id="59689-157">string</span><span class="sxs-lookup"><span data-stu-id="59689-157">string</span></span>|<span data-ttu-id="59689-158">用户标识符。</span><span class="sxs-lookup"><span data-stu-id="59689-158">User identifier.</span></span> <span data-ttu-id="59689-159">格式字符串 GUID。</span><span class="sxs-lookup"><span data-stu-id="59689-159">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59689-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="59689-160">Relationships</span></span>
| <span data-ttu-id="59689-161">关系</span><span class="sxs-lookup"><span data-stu-id="59689-161">Relationship</span></span> | <span data-ttu-id="59689-162">类型</span><span class="sxs-lookup"><span data-stu-id="59689-162">Type</span></span>   |<span data-ttu-id="59689-163">Description</span><span class="sxs-lookup"><span data-stu-id="59689-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59689-164">roleInfo</span><span class="sxs-lookup"><span data-stu-id="59689-164">roleInfo</span></span>|[<span data-ttu-id="59689-165">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="59689-165">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="59689-166">只读。</span><span class="sxs-lookup"><span data-stu-id="59689-166">Read-only.</span></span> <span data-ttu-id="59689-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="59689-167">Nullable.</span></span> <span data-ttu-id="59689-168">相关联的角色的信息。</span><span class="sxs-lookup"><span data-stu-id="59689-168">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59689-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59689-169">JSON representation</span></span>

<span data-ttu-id="59689-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59689-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
