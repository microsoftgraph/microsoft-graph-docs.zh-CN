---
title: privilegedRoleAssignment 资源类型
description: '表示特定用户的特权角色分配。 '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563396"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="0e3dd-103">privilegedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e3dd-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e3dd-104">表示特定用户的特权角色分配。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="0e3dd-105">方法</span><span class="sxs-lookup"><span data-stu-id="0e3dd-105">Methods</span></span>

| <span data-ttu-id="0e3dd-106">方法</span><span class="sxs-lookup"><span data-stu-id="0e3dd-106">Method</span></span>           | <span data-ttu-id="0e3dd-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e3dd-107">Return Type</span></span>    |<span data-ttu-id="0e3dd-108">说明</span><span class="sxs-lookup"><span data-stu-id="0e3dd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e3dd-109">列出 privilegedRoleAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="0e3dd-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="0e3dd-110">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e3dd-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="0e3dd-111">获取 privilegedRoleAssignment 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="0e3dd-112">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0e3dd-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="0e3dd-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0e3dd-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="0e3dd-114">读取 privilegedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="0e3dd-115">创建作业</span><span class="sxs-lookup"><span data-stu-id="0e3dd-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="0e3dd-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0e3dd-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="0e3dd-117">通过发布到工作分配集合来创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="0e3dd-118">删除</span><span class="sxs-lookup"><span data-stu-id="0e3dd-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="0e3dd-119">无</span><span class="sxs-lookup"><span data-stu-id="0e3dd-119">None</span></span> |<span data-ttu-id="0e3dd-120">删除 privilegedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="0e3dd-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="0e3dd-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="0e3dd-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0e3dd-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="0e3dd-123">将角色分配标记为永久。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="0e3dd-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="0e3dd-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="0e3dd-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0e3dd-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="0e3dd-126">使角色分配符合资格。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="0e3dd-127">My</span><span class="sxs-lookup"><span data-stu-id="0e3dd-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="0e3dd-128">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e3dd-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="0e3dd-129">获取当前用户的特权角色分配。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e3dd-130">属性</span><span class="sxs-lookup"><span data-stu-id="0e3dd-130">Properties</span></span>
| <span data-ttu-id="0e3dd-131">属性</span><span class="sxs-lookup"><span data-stu-id="0e3dd-131">Property</span></span>     | <span data-ttu-id="0e3dd-132">类型</span><span class="sxs-lookup"><span data-stu-id="0e3dd-132">Type</span></span>   |<span data-ttu-id="0e3dd-133">说明</span><span class="sxs-lookup"><span data-stu-id="0e3dd-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e3dd-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3dd-134">expirationDateTime</span></span>|<span data-ttu-id="0e3dd-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3dd-135">dateTimeOffset</span></span>|<span data-ttu-id="0e3dd-136">临时权限角色分配将在何时过期时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="0e3dd-137">对于永久角色分配, 值为 null。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="0e3dd-138">id</span><span class="sxs-lookup"><span data-stu-id="0e3dd-138">id</span></span>|<span data-ttu-id="0e3dd-139">string</span><span class="sxs-lookup"><span data-stu-id="0e3dd-139">string</span></span>| <span data-ttu-id="0e3dd-140">特权角色分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="0e3dd-141">只读。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-141">Read-only.</span></span> <span data-ttu-id="0e3dd-142">它的格式为 "userId_roleId", 其中 userId 是 azure AD 用户 id 的 guid 字符串, roleId 是 azure 管理员角色 id 的 guid 字符串。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="0e3dd-143">isElevated</span><span class="sxs-lookup"><span data-stu-id="0e3dd-143">isElevated</span></span>|<span data-ttu-id="0e3dd-144">布尔</span><span class="sxs-lookup"><span data-stu-id="0e3dd-144">boolean</span></span>|<span data-ttu-id="0e3dd-145">如果角色分配已激活,**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="0e3dd-146">**假**如果角色分配被停用。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="0e3dd-147">resultMessage</span><span class="sxs-lookup"><span data-stu-id="0e3dd-147">resultMessage</span></span>|<span data-ttu-id="0e3dd-148">string</span><span class="sxs-lookup"><span data-stu-id="0e3dd-148">string</span></span>|<span data-ttu-id="0e3dd-149">由服务设置的结果消息。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-149">Result message set by the service.</span></span>|
|<span data-ttu-id="0e3dd-150">roleId</span><span class="sxs-lookup"><span data-stu-id="0e3dd-150">roleId</span></span>|<span data-ttu-id="0e3dd-151">string</span><span class="sxs-lookup"><span data-stu-id="0e3dd-151">string</span></span>|<span data-ttu-id="0e3dd-152">角色标识符。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-152">Role identifier.</span></span> <span data-ttu-id="0e3dd-153">以 GUID 字符串格式。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-153">In GUID string format.</span></span>|
|<span data-ttu-id="0e3dd-154">userId</span><span class="sxs-lookup"><span data-stu-id="0e3dd-154">userId</span></span>|<span data-ttu-id="0e3dd-155">string</span><span class="sxs-lookup"><span data-stu-id="0e3dd-155">string</span></span>|<span data-ttu-id="0e3dd-156">用户标识符。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-156">User identifier.</span></span> <span data-ttu-id="0e3dd-157">以 GUID 字符串格式。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e3dd-158">关系</span><span class="sxs-lookup"><span data-stu-id="0e3dd-158">Relationships</span></span>
| <span data-ttu-id="0e3dd-159">关系</span><span class="sxs-lookup"><span data-stu-id="0e3dd-159">Relationship</span></span> | <span data-ttu-id="0e3dd-160">类型</span><span class="sxs-lookup"><span data-stu-id="0e3dd-160">Type</span></span>   |<span data-ttu-id="0e3dd-161">说明</span><span class="sxs-lookup"><span data-stu-id="0e3dd-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e3dd-162">roleInfo</span><span class="sxs-lookup"><span data-stu-id="0e3dd-162">roleInfo</span></span>|[<span data-ttu-id="0e3dd-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="0e3dd-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="0e3dd-164">只读。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-164">Read-only.</span></span> <span data-ttu-id="0e3dd-165">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-165">Nullable.</span></span> <span data-ttu-id="0e3dd-166">相关联的角色信息。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e3dd-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e3dd-167">JSON representation</span></span>

<span data-ttu-id="0e3dd-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e3dd-168">Here is a JSON representation of the resource.</span></span>

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
