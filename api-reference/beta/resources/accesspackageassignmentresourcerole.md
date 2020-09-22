---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示使用者已通过访问包分配分配的特定于资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8bf839d68db3f54df5a27601a4a05463e013fbef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089859"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="8301f-103">accessPackageAssignmentResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="8301f-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="8301f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8301f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8301f-105">在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配资源角色指示已通过访问包分配分配的主题的特定于资源的角色。</span><span class="sxs-lookup"><span data-stu-id="8301f-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="8301f-106">方法</span><span class="sxs-lookup"><span data-stu-id="8301f-106">Methods</span></span>

| <span data-ttu-id="8301f-107">方法</span><span class="sxs-lookup"><span data-stu-id="8301f-107">Method</span></span>       | <span data-ttu-id="8301f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8301f-108">Return Type</span></span> | <span data-ttu-id="8301f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8301f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8301f-110">获取 accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="8301f-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="8301f-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="8301f-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="8301f-112">检索 accessPackageAssignmentResourceRole 对象。</span><span class="sxs-lookup"><span data-stu-id="8301f-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="8301f-113">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="8301f-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="8301f-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8301f-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="8301f-115">检索 accessPackageAssignmentResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8301f-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="8301f-116">属性</span><span class="sxs-lookup"><span data-stu-id="8301f-116">Properties</span></span>

| <span data-ttu-id="8301f-117">属性</span><span class="sxs-lookup"><span data-stu-id="8301f-117">Property</span></span>     | <span data-ttu-id="8301f-118">类型</span><span class="sxs-lookup"><span data-stu-id="8301f-118">Type</span></span>        | <span data-ttu-id="8301f-119">说明</span><span class="sxs-lookup"><span data-stu-id="8301f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8301f-120">id</span><span class="sxs-lookup"><span data-stu-id="8301f-120">id</span></span>|<span data-ttu-id="8301f-121">字符串</span><span class="sxs-lookup"><span data-stu-id="8301f-121">String</span></span>| <span data-ttu-id="8301f-122">只读。</span><span class="sxs-lookup"><span data-stu-id="8301f-122">Read-only.</span></span>|
|<span data-ttu-id="8301f-123">originId</span><span class="sxs-lookup"><span data-stu-id="8301f-123">originId</span></span>|<span data-ttu-id="8301f-124">字符串</span><span class="sxs-lookup"><span data-stu-id="8301f-124">String</span></span>|<span data-ttu-id="8301f-125">相对于原始系统的唯一标识符，对应于 [accessPackageResourceRole](accesspackageresourcerole.md)的 originId 属性。</span><span class="sxs-lookup"><span data-stu-id="8301f-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="8301f-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="8301f-126">originSystem</span></span>|<span data-ttu-id="8301f-127">字符串</span><span class="sxs-lookup"><span data-stu-id="8301f-127">String</span></span>|<span data-ttu-id="8301f-128">要在其中创建角色分配或为访问包分配创建的系统（如或），该系统 `SharePointOnline` `AadGroup` `AadApplication` 对应于 [accessPackageResourceRole](accesspackageresourcerole.md)的 originSystem 属性。</span><span class="sxs-lookup"><span data-stu-id="8301f-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="8301f-129">状态</span><span class="sxs-lookup"><span data-stu-id="8301f-129">status</span></span>|<span data-ttu-id="8301f-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8301f-130">String</span></span>|<span data-ttu-id="8301f-131">值是 `PendingFulfillment` 访问包分配尚未传递到原始系统，以及 `Fulfilled` 访问包分配已传递到原始系统。。</span><span class="sxs-lookup"><span data-stu-id="8301f-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8301f-132">关系</span><span class="sxs-lookup"><span data-stu-id="8301f-132">Relationships</span></span>

| <span data-ttu-id="8301f-133">关系</span><span class="sxs-lookup"><span data-stu-id="8301f-133">Relationship</span></span> | <span data-ttu-id="8301f-134">类型</span><span class="sxs-lookup"><span data-stu-id="8301f-134">Type</span></span>        | <span data-ttu-id="8301f-135">说明</span><span class="sxs-lookup"><span data-stu-id="8301f-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8301f-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="8301f-136">accessPackageAssignments</span></span>|<span data-ttu-id="8301f-137">[accessPackageAssignment](accesspackageassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8301f-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="8301f-138">此角色分配导致的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="8301f-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="8301f-139">只读。</span><span class="sxs-lookup"><span data-stu-id="8301f-139">Read-only.</span></span> <span data-ttu-id="8301f-140">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8301f-140">Nullable.</span></span>|
|<span data-ttu-id="8301f-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="8301f-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="8301f-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="8301f-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="8301f-143">只读。</span><span class="sxs-lookup"><span data-stu-id="8301f-143">Read-only.</span></span> <span data-ttu-id="8301f-144">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8301f-144">Nullable.</span></span>|
|<span data-ttu-id="8301f-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="8301f-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="8301f-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="8301f-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="8301f-147">只读。</span><span class="sxs-lookup"><span data-stu-id="8301f-147">Read-only.</span></span> <span data-ttu-id="8301f-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8301f-148">Nullable.</span></span>|
|<span data-ttu-id="8301f-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="8301f-149">accessPackageSubject</span></span>|[<span data-ttu-id="8301f-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="8301f-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="8301f-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="8301f-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8301f-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8301f-153">JSON representation</span></span>

<span data-ttu-id="8301f-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8301f-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


