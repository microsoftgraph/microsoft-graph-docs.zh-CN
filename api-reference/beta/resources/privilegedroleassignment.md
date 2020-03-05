---
title: privilegedRoleAssignment 资源类型
description: '表示特定用户的特权角色分配。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2781e601b82e33c260ead70c5d87c9e36c495569
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521507"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="0407d-103">privilegedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0407d-103">privilegedRoleAssignment resource type</span></span>

<span data-ttu-id="0407d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0407d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0407d-105">表示特定用户的特权角色分配。</span><span class="sxs-lookup"><span data-stu-id="0407d-105">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="0407d-106">方法</span><span class="sxs-lookup"><span data-stu-id="0407d-106">Methods</span></span>

| <span data-ttu-id="0407d-107">方法</span><span class="sxs-lookup"><span data-stu-id="0407d-107">Method</span></span>           | <span data-ttu-id="0407d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0407d-108">Return Type</span></span>    |<span data-ttu-id="0407d-109">说明</span><span class="sxs-lookup"><span data-stu-id="0407d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0407d-110">列出 privilegedRoleAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="0407d-110">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="0407d-111">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0407d-111">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="0407d-112">获取 privilegedRoleAssignment 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0407d-112">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="0407d-113">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0407d-113">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="0407d-114">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0407d-114">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="0407d-115">读取 privilegedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0407d-115">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="0407d-116">创建作业</span><span class="sxs-lookup"><span data-stu-id="0407d-116">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="0407d-117">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0407d-117">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="0407d-118">通过发布到工作分配集合来创建新的工作分配。</span><span class="sxs-lookup"><span data-stu-id="0407d-118">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="0407d-119">删除</span><span class="sxs-lookup"><span data-stu-id="0407d-119">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="0407d-120">无</span><span class="sxs-lookup"><span data-stu-id="0407d-120">None</span></span> |<span data-ttu-id="0407d-121">删除 privilegedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="0407d-121">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="0407d-122">makePermanent</span><span class="sxs-lookup"><span data-stu-id="0407d-122">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="0407d-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0407d-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="0407d-124">将角色分配标记为永久。</span><span class="sxs-lookup"><span data-stu-id="0407d-124">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="0407d-125">makeEligible</span><span class="sxs-lookup"><span data-stu-id="0407d-125">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="0407d-126">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0407d-126">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="0407d-127">使角色分配符合资格。</span><span class="sxs-lookup"><span data-stu-id="0407d-127">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="0407d-128">My</span><span class="sxs-lookup"><span data-stu-id="0407d-128">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="0407d-129">[privilegedRoleAssignment](privilegedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0407d-129">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="0407d-130">获取当前用户的特权角色分配。</span><span class="sxs-lookup"><span data-stu-id="0407d-130">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="0407d-131">属性</span><span class="sxs-lookup"><span data-stu-id="0407d-131">Properties</span></span>
| <span data-ttu-id="0407d-132">属性</span><span class="sxs-lookup"><span data-stu-id="0407d-132">Property</span></span>     | <span data-ttu-id="0407d-133">类型</span><span class="sxs-lookup"><span data-stu-id="0407d-133">Type</span></span>   |<span data-ttu-id="0407d-134">说明</span><span class="sxs-lookup"><span data-stu-id="0407d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0407d-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0407d-135">expirationDateTime</span></span>|<span data-ttu-id="0407d-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0407d-136">dateTimeOffset</span></span>|<span data-ttu-id="0407d-137">临时权限角色分配将在何时过期时的 UTC 日期时间。</span><span class="sxs-lookup"><span data-stu-id="0407d-137">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="0407d-138">对于永久角色分配，值为 null。</span><span class="sxs-lookup"><span data-stu-id="0407d-138">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="0407d-139">id</span><span class="sxs-lookup"><span data-stu-id="0407d-139">id</span></span>|<span data-ttu-id="0407d-140">string</span><span class="sxs-lookup"><span data-stu-id="0407d-140">string</span></span>| <span data-ttu-id="0407d-141">特权角色分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0407d-141">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="0407d-142">只读。</span><span class="sxs-lookup"><span data-stu-id="0407d-142">Read-only.</span></span> <span data-ttu-id="0407d-143">它的格式为 "userId_roleId"，其中 userId 是 Azure AD 用户 id 的 GUID 字符串，roleId 是 Azure 管理员角色 id 的 GUID 字符串。</span><span class="sxs-lookup"><span data-stu-id="0407d-143">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="0407d-144">isElevated</span><span class="sxs-lookup"><span data-stu-id="0407d-144">isElevated</span></span>|<span data-ttu-id="0407d-145">boolean</span><span class="sxs-lookup"><span data-stu-id="0407d-145">boolean</span></span>|<span data-ttu-id="0407d-146">如果角色分配已激活，**则为 true** 。</span><span class="sxs-lookup"><span data-stu-id="0407d-146">**true** if the role assignment is activated.</span></span> <span data-ttu-id="0407d-147">**假**如果角色分配被停用。</span><span class="sxs-lookup"><span data-stu-id="0407d-147">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="0407d-148">resultMessage</span><span class="sxs-lookup"><span data-stu-id="0407d-148">resultMessage</span></span>|<span data-ttu-id="0407d-149">string</span><span class="sxs-lookup"><span data-stu-id="0407d-149">string</span></span>|<span data-ttu-id="0407d-150">由服务设置的结果消息。</span><span class="sxs-lookup"><span data-stu-id="0407d-150">Result message set by the service.</span></span>|
|<span data-ttu-id="0407d-151">roleId</span><span class="sxs-lookup"><span data-stu-id="0407d-151">roleId</span></span>|<span data-ttu-id="0407d-152">string</span><span class="sxs-lookup"><span data-stu-id="0407d-152">string</span></span>|<span data-ttu-id="0407d-153">角色标识符。</span><span class="sxs-lookup"><span data-stu-id="0407d-153">Role identifier.</span></span> <span data-ttu-id="0407d-154">以 GUID 字符串格式。</span><span class="sxs-lookup"><span data-stu-id="0407d-154">In GUID string format.</span></span>|
|<span data-ttu-id="0407d-155">userId</span><span class="sxs-lookup"><span data-stu-id="0407d-155">userId</span></span>|<span data-ttu-id="0407d-156">string</span><span class="sxs-lookup"><span data-stu-id="0407d-156">string</span></span>|<span data-ttu-id="0407d-157">用户标识符。</span><span class="sxs-lookup"><span data-stu-id="0407d-157">User identifier.</span></span> <span data-ttu-id="0407d-158">以 GUID 字符串格式。</span><span class="sxs-lookup"><span data-stu-id="0407d-158">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0407d-159">关系</span><span class="sxs-lookup"><span data-stu-id="0407d-159">Relationships</span></span>
| <span data-ttu-id="0407d-160">关系</span><span class="sxs-lookup"><span data-stu-id="0407d-160">Relationship</span></span> | <span data-ttu-id="0407d-161">类型</span><span class="sxs-lookup"><span data-stu-id="0407d-161">Type</span></span>   |<span data-ttu-id="0407d-162">说明</span><span class="sxs-lookup"><span data-stu-id="0407d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0407d-163">roleInfo</span><span class="sxs-lookup"><span data-stu-id="0407d-163">roleInfo</span></span>|[<span data-ttu-id="0407d-164">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="0407d-164">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="0407d-165">只读。</span><span class="sxs-lookup"><span data-stu-id="0407d-165">Read-only.</span></span> <span data-ttu-id="0407d-166">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0407d-166">Nullable.</span></span> <span data-ttu-id="0407d-167">相关联的角色信息。</span><span class="sxs-lookup"><span data-stu-id="0407d-167">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0407d-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0407d-168">JSON representation</span></span>

<span data-ttu-id="0407d-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0407d-169">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
  "suppressions": []
}
-->
