---
title: privilegedRoleAssignment 资源类型
description: '表示特定用户特权的角色分配。 '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515116"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="d70ac-103">privilegedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d70ac-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d70ac-104">表示特定用户特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="d70ac-105">方法</span><span class="sxs-lookup"><span data-stu-id="d70ac-105">Methods</span></span>

| <span data-ttu-id="d70ac-106">方法</span><span class="sxs-lookup"><span data-stu-id="d70ac-106">Method</span></span>           | <span data-ttu-id="d70ac-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d70ac-107">Return Type</span></span>    |<span data-ttu-id="d70ac-108">说明</span><span class="sxs-lookup"><span data-stu-id="d70ac-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d70ac-109">列表 privilegedRoleAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="d70ac-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="d70ac-110">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d70ac-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="d70ac-111">获取 privilegedRoleAssignment 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d70ac-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="d70ac-112">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d70ac-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="d70ac-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d70ac-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="d70ac-114">读取属性和 privilegedRoleAssignment 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d70ac-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="d70ac-115">创建工作分配</span><span class="sxs-lookup"><span data-stu-id="d70ac-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="d70ac-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d70ac-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="d70ac-117">通过发布到 assignments 集合中创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="d70ac-118">删除</span><span class="sxs-lookup"><span data-stu-id="d70ac-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="d70ac-119">无</span><span class="sxs-lookup"><span data-stu-id="d70ac-119">None</span></span> |<span data-ttu-id="d70ac-120">删除 privilegedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="d70ac-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="d70ac-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="d70ac-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="d70ac-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d70ac-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="d70ac-123">请为永久的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="d70ac-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="d70ac-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="d70ac-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d70ac-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="d70ac-126">请作为合格的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="d70ac-127">My</span><span class="sxs-lookup"><span data-stu-id="d70ac-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="d70ac-128">[privilegedRoleAssignment](privilegedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d70ac-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="d70ac-129">获取当前用户的特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="d70ac-130">属性</span><span class="sxs-lookup"><span data-stu-id="d70ac-130">Properties</span></span>
| <span data-ttu-id="d70ac-131">属性</span><span class="sxs-lookup"><span data-stu-id="d70ac-131">Property</span></span>     | <span data-ttu-id="d70ac-132">类型</span><span class="sxs-lookup"><span data-stu-id="d70ac-132">Type</span></span>   |<span data-ttu-id="d70ac-133">说明</span><span class="sxs-lookup"><span data-stu-id="d70ac-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d70ac-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d70ac-134">expirationDateTime</span></span>|<span data-ttu-id="d70ac-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d70ac-135">dateTimeOffset</span></span>|<span data-ttu-id="d70ac-136">UTC DateTime 时将过期的临时特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="d70ac-137">永久角色分配的值为 null。</span><span class="sxs-lookup"><span data-stu-id="d70ac-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="d70ac-138">id</span><span class="sxs-lookup"><span data-stu-id="d70ac-138">id</span></span>|<span data-ttu-id="d70ac-139">string</span><span class="sxs-lookup"><span data-stu-id="d70ac-139">string</span></span>| <span data-ttu-id="d70ac-140">特权的角色分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d70ac-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="d70ac-141">只读。</span><span class="sxs-lookup"><span data-stu-id="d70ac-141">Read-only.</span></span> <span data-ttu-id="d70ac-142">处于 userId_roleId，其中 userId 是 Azure AD 用户 id 的 GUID 字符串，roleId 是 Azure 管理员角色 id 的 GUID 字符串的格式。</span><span class="sxs-lookup"><span data-stu-id="d70ac-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="d70ac-143">isElevated</span><span class="sxs-lookup"><span data-stu-id="d70ac-143">isElevated</span></span>|<span data-ttu-id="d70ac-144">布尔</span><span class="sxs-lookup"><span data-stu-id="d70ac-144">boolean</span></span>|<span data-ttu-id="d70ac-145">**true**如果激活该角色分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="d70ac-146">**false**如果停用的角色分配。</span><span class="sxs-lookup"><span data-stu-id="d70ac-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="d70ac-147">resultMessage</span><span class="sxs-lookup"><span data-stu-id="d70ac-147">resultMessage</span></span>|<span data-ttu-id="d70ac-148">string</span><span class="sxs-lookup"><span data-stu-id="d70ac-148">string</span></span>|<span data-ttu-id="d70ac-149">结果消息由服务设置。</span><span class="sxs-lookup"><span data-stu-id="d70ac-149">Result message set by the service.</span></span>|
|<span data-ttu-id="d70ac-150">roleId</span><span class="sxs-lookup"><span data-stu-id="d70ac-150">roleId</span></span>|<span data-ttu-id="d70ac-151">string</span><span class="sxs-lookup"><span data-stu-id="d70ac-151">string</span></span>|<span data-ttu-id="d70ac-152">角色标识符</span><span class="sxs-lookup"><span data-stu-id="d70ac-152">Role identifier.</span></span> <span data-ttu-id="d70ac-153">格式字符串 GUID。</span><span class="sxs-lookup"><span data-stu-id="d70ac-153">In GUID string format.</span></span>|
|<span data-ttu-id="d70ac-154">userId</span><span class="sxs-lookup"><span data-stu-id="d70ac-154">userId</span></span>|<span data-ttu-id="d70ac-155">string</span><span class="sxs-lookup"><span data-stu-id="d70ac-155">string</span></span>|<span data-ttu-id="d70ac-156">用户标识符。</span><span class="sxs-lookup"><span data-stu-id="d70ac-156">User identifier.</span></span> <span data-ttu-id="d70ac-157">格式字符串 GUID。</span><span class="sxs-lookup"><span data-stu-id="d70ac-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d70ac-158">关系</span><span class="sxs-lookup"><span data-stu-id="d70ac-158">Relationships</span></span>
| <span data-ttu-id="d70ac-159">关系</span><span class="sxs-lookup"><span data-stu-id="d70ac-159">Relationship</span></span> | <span data-ttu-id="d70ac-160">类型</span><span class="sxs-lookup"><span data-stu-id="d70ac-160">Type</span></span>   |<span data-ttu-id="d70ac-161">说明</span><span class="sxs-lookup"><span data-stu-id="d70ac-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d70ac-162">roleInfo</span><span class="sxs-lookup"><span data-stu-id="d70ac-162">roleInfo</span></span>|[<span data-ttu-id="d70ac-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="d70ac-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="d70ac-164">只读。</span><span class="sxs-lookup"><span data-stu-id="d70ac-164">Read-only.</span></span> <span data-ttu-id="d70ac-165">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d70ac-165">Nullable.</span></span> <span data-ttu-id="d70ac-166">相关联的角色的信息。</span><span class="sxs-lookup"><span data-stu-id="d70ac-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d70ac-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d70ac-167">JSON representation</span></span>

<span data-ttu-id="d70ac-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d70ac-168">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
