---
title: privilegedRoleAssignment 资源类型
description: '表示特定用户特权的角色分配。 '
ms.openlocfilehash: 40cfe6487184171fc0d120f9a0e2cd98070f96f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043584"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="aef5d-103">privilegedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="aef5d-103">privilegedRoleAssignment resource type</span></span>

> <span data-ttu-id="aef5d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aef5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aef5d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aef5d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aef5d-106">表示特定用户特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-106">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="aef5d-107">方法</span><span class="sxs-lookup"><span data-stu-id="aef5d-107">Methods</span></span>

| <span data-ttu-id="aef5d-108">方法</span><span class="sxs-lookup"><span data-stu-id="aef5d-108">Method</span></span>           | <span data-ttu-id="aef5d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aef5d-109">Return Type</span></span>    |<span data-ttu-id="aef5d-110">说明</span><span class="sxs-lookup"><span data-stu-id="aef5d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aef5d-111">列表 privilegedRoleAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="aef5d-111">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="aef5d-112">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="aef5d-112">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="aef5d-113">获取 privilegedRoleAssignment 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="aef5d-113">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="aef5d-114">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="aef5d-114">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="aef5d-115">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="aef5d-115">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="aef5d-116">读取属性和 privilegedRoleAssignment 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="aef5d-116">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="aef5d-117">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="aef5d-117">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="aef5d-118">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="aef5d-118">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="aef5d-119">通过发布到 assignments 集合中创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-119">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="aef5d-120">删除</span><span class="sxs-lookup"><span data-stu-id="aef5d-120">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="aef5d-121">无</span><span class="sxs-lookup"><span data-stu-id="aef5d-121">None</span></span> |<span data-ttu-id="aef5d-122">删除 privilegedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="aef5d-122">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="aef5d-123">makePermanent</span><span class="sxs-lookup"><span data-stu-id="aef5d-123">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="aef5d-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="aef5d-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="aef5d-125">请为永久的角色分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-125">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="aef5d-126">makeEligible</span><span class="sxs-lookup"><span data-stu-id="aef5d-126">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="aef5d-127">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="aef5d-127">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="aef5d-128">请作为合格的角色分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-128">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="aef5d-129">我</span><span class="sxs-lookup"><span data-stu-id="aef5d-129">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="aef5d-130">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="aef5d-130">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="aef5d-131">获取当前用户的特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-131">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="aef5d-132">属性</span><span class="sxs-lookup"><span data-stu-id="aef5d-132">Properties</span></span>
| <span data-ttu-id="aef5d-133">属性</span><span class="sxs-lookup"><span data-stu-id="aef5d-133">Property</span></span>     | <span data-ttu-id="aef5d-134">类型</span><span class="sxs-lookup"><span data-stu-id="aef5d-134">Type</span></span>   |<span data-ttu-id="aef5d-135">说明</span><span class="sxs-lookup"><span data-stu-id="aef5d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aef5d-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="aef5d-136">expirationDateTime</span></span>|<span data-ttu-id="aef5d-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aef5d-137">dateTimeOffset</span></span>|<span data-ttu-id="aef5d-138">UTC DateTime 时将过期的临时特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-138">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="aef5d-139">永久角色分配的值为 null。</span><span class="sxs-lookup"><span data-stu-id="aef5d-139">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="aef5d-140">id</span><span class="sxs-lookup"><span data-stu-id="aef5d-140">id</span></span>|<span data-ttu-id="aef5d-141">string</span><span class="sxs-lookup"><span data-stu-id="aef5d-141">string</span></span>| <span data-ttu-id="aef5d-142">特权的角色分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aef5d-142">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="aef5d-143">只读。</span><span class="sxs-lookup"><span data-stu-id="aef5d-143">Read-only.</span></span> <span data-ttu-id="aef5d-144">处于 userId_roleId，其中 userId 是 Azure AD 用户 id 的 GUID 字符串，roleId 是 Azure 管理员角色 id 的 GUID 字符串的格式。</span><span class="sxs-lookup"><span data-stu-id="aef5d-144">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="aef5d-145">isElevated</span><span class="sxs-lookup"><span data-stu-id="aef5d-145">isElevated</span></span>|<span data-ttu-id="aef5d-146">boolean</span><span class="sxs-lookup"><span data-stu-id="aef5d-146">boolean</span></span>|<span data-ttu-id="aef5d-147">**true**如果激活该角色分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-147">**true** if the role assignment is activated.</span></span> <span data-ttu-id="aef5d-148">**false**如果停用的角色分配。</span><span class="sxs-lookup"><span data-stu-id="aef5d-148">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="aef5d-149">resultMessage</span><span class="sxs-lookup"><span data-stu-id="aef5d-149">resultMessage</span></span>|<span data-ttu-id="aef5d-150">string</span><span class="sxs-lookup"><span data-stu-id="aef5d-150">string</span></span>|<span data-ttu-id="aef5d-151">结果消息由服务设置。</span><span class="sxs-lookup"><span data-stu-id="aef5d-151">Result message set by the service.</span></span>|
|<span data-ttu-id="aef5d-152">roleId</span><span class="sxs-lookup"><span data-stu-id="aef5d-152">roleId</span></span>|<span data-ttu-id="aef5d-153">string</span><span class="sxs-lookup"><span data-stu-id="aef5d-153">string</span></span>|<span data-ttu-id="aef5d-154">角色标识符。</span><span class="sxs-lookup"><span data-stu-id="aef5d-154">Role identifier.</span></span> <span data-ttu-id="aef5d-155">格式字符串 GUID。</span><span class="sxs-lookup"><span data-stu-id="aef5d-155">In GUID string format.</span></span>|
|<span data-ttu-id="aef5d-156">userId</span><span class="sxs-lookup"><span data-stu-id="aef5d-156">userId</span></span>|<span data-ttu-id="aef5d-157">string</span><span class="sxs-lookup"><span data-stu-id="aef5d-157">string</span></span>|<span data-ttu-id="aef5d-158">用户标识符。</span><span class="sxs-lookup"><span data-stu-id="aef5d-158">User identifier.</span></span> <span data-ttu-id="aef5d-159">格式字符串 GUID。</span><span class="sxs-lookup"><span data-stu-id="aef5d-159">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aef5d-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="aef5d-160">Relationships</span></span>
| <span data-ttu-id="aef5d-161">关系</span><span class="sxs-lookup"><span data-stu-id="aef5d-161">Relationship</span></span> | <span data-ttu-id="aef5d-162">类型</span><span class="sxs-lookup"><span data-stu-id="aef5d-162">Type</span></span>   |<span data-ttu-id="aef5d-163">说明</span><span class="sxs-lookup"><span data-stu-id="aef5d-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aef5d-164">roleInfo</span><span class="sxs-lookup"><span data-stu-id="aef5d-164">roleInfo</span></span>|[<span data-ttu-id="aef5d-165">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="aef5d-165">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="aef5d-166">只读。</span><span class="sxs-lookup"><span data-stu-id="aef5d-166">Read-only.</span></span> <span data-ttu-id="aef5d-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="aef5d-167">Nullable.</span></span> <span data-ttu-id="aef5d-168">相关联的角色的信息。</span><span class="sxs-lookup"><span data-stu-id="aef5d-168">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aef5d-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aef5d-169">JSON representation</span></span>

<span data-ttu-id="aef5d-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aef5d-170">Here is a JSON representation of the resource.</span></span>

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