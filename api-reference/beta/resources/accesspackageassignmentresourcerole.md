---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示主题已通过访问包分配分配的资源特定角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4473c303a74cbf9e8e0c17d6c9060960590a3405
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433266"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="3207f-103">accessPackageAssignmentResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="3207f-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="3207f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3207f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3207f-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配资源角色指示主题已通过访问包分配分配的资源特定角色。</span><span class="sxs-lookup"><span data-stu-id="3207f-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="3207f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3207f-106">Methods</span></span>

| <span data-ttu-id="3207f-107">方法</span><span class="sxs-lookup"><span data-stu-id="3207f-107">Method</span></span>       | <span data-ttu-id="3207f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3207f-108">Return Type</span></span> | <span data-ttu-id="3207f-109">说明</span><span class="sxs-lookup"><span data-stu-id="3207f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3207f-110">获取 accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="3207f-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="3207f-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="3207f-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="3207f-112">检索 accessPackageAssignmentResourceRole 对象。</span><span class="sxs-lookup"><span data-stu-id="3207f-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="3207f-113">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="3207f-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="3207f-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3207f-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="3207f-115">检索 accessPackageAssignmentResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3207f-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="3207f-116">属性</span><span class="sxs-lookup"><span data-stu-id="3207f-116">Properties</span></span>

| <span data-ttu-id="3207f-117">属性</span><span class="sxs-lookup"><span data-stu-id="3207f-117">Property</span></span>     | <span data-ttu-id="3207f-118">类型</span><span class="sxs-lookup"><span data-stu-id="3207f-118">Type</span></span>        | <span data-ttu-id="3207f-119">说明</span><span class="sxs-lookup"><span data-stu-id="3207f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3207f-120">id</span><span class="sxs-lookup"><span data-stu-id="3207f-120">id</span></span>|<span data-ttu-id="3207f-121">String</span><span class="sxs-lookup"><span data-stu-id="3207f-121">String</span></span>| <span data-ttu-id="3207f-122">只读。</span><span class="sxs-lookup"><span data-stu-id="3207f-122">Read-only.</span></span>|
|<span data-ttu-id="3207f-123">originId</span><span class="sxs-lookup"><span data-stu-id="3207f-123">originId</span></span>|<span data-ttu-id="3207f-124">String</span><span class="sxs-lookup"><span data-stu-id="3207f-124">String</span></span>|<span data-ttu-id="3207f-125">与源系统相对的唯一标识符，对应于 [accessPackageResourceRole](accesspackageresourcerole.md)的 originId 属性。</span><span class="sxs-lookup"><span data-stu-id="3207f-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="3207f-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="3207f-126">originSystem</span></span>|<span data-ttu-id="3207f-127">String</span><span class="sxs-lookup"><span data-stu-id="3207f-127">String</span></span>|<span data-ttu-id="3207f-128">要创建角色分配或已创建用于访问包分配的系统，例如 ，或 ， `SharePointOnline` `AadGroup` 对应于 `AadApplication` [accessPackageResourceRole](accesspackageresourcerole.md)的 originSystem 属性。</span><span class="sxs-lookup"><span data-stu-id="3207f-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="3207f-129">status</span><span class="sxs-lookup"><span data-stu-id="3207f-129">status</span></span>|<span data-ttu-id="3207f-130">String</span><span class="sxs-lookup"><span data-stu-id="3207f-130">String</span></span>|<span data-ttu-id="3207f-131">该值是访问包分配尚未传递到源系统以及访问包分配已传递到源系统 `PendingFulfillment` `Fulfilled` 时。</span><span class="sxs-lookup"><span data-stu-id="3207f-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3207f-132">关系</span><span class="sxs-lookup"><span data-stu-id="3207f-132">Relationships</span></span>

| <span data-ttu-id="3207f-133">关系</span><span class="sxs-lookup"><span data-stu-id="3207f-133">Relationship</span></span> | <span data-ttu-id="3207f-134">类型</span><span class="sxs-lookup"><span data-stu-id="3207f-134">Type</span></span>        | <span data-ttu-id="3207f-135">说明</span><span class="sxs-lookup"><span data-stu-id="3207f-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3207f-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="3207f-136">accessPackageAssignments</span></span>|<span data-ttu-id="3207f-137">[accessPackageAssignment](accesspackageassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3207f-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="3207f-138">导致出现此限制的访问包角色分配。</span><span class="sxs-lookup"><span data-stu-id="3207f-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="3207f-139">只读。</span><span class="sxs-lookup"><span data-stu-id="3207f-139">Read-only.</span></span> <span data-ttu-id="3207f-140">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="3207f-140">Nullable.</span></span>|
|<span data-ttu-id="3207f-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="3207f-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="3207f-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="3207f-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="3207f-143">只读。</span><span class="sxs-lookup"><span data-stu-id="3207f-143">Read-only.</span></span> <span data-ttu-id="3207f-144">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="3207f-144">Nullable.</span></span>|
|<span data-ttu-id="3207f-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="3207f-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="3207f-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="3207f-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="3207f-147">只读。</span><span class="sxs-lookup"><span data-stu-id="3207f-147">Read-only.</span></span> <span data-ttu-id="3207f-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="3207f-148">Nullable.</span></span>|
|<span data-ttu-id="3207f-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="3207f-149">accessPackageSubject</span></span>|[<span data-ttu-id="3207f-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="3207f-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="3207f-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="3207f-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3207f-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3207f-153">JSON representation</span></span>

<span data-ttu-id="3207f-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3207f-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
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


