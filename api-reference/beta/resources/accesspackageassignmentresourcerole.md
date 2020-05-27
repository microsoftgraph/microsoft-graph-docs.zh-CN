---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示使用者已通过访问包分配分配的特定于资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6ef0827736d16f1dbf3aedfb664467011e75e7b2
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383775"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="82d1a-103">accessPackageAssignmentResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="82d1a-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="82d1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82d1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82d1a-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配资源角色指示已通过访问包分配分配的主题的特定于资源的角色。</span><span class="sxs-lookup"><span data-stu-id="82d1a-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="82d1a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="82d1a-106">Methods</span></span>

| <span data-ttu-id="82d1a-107">方法</span><span class="sxs-lookup"><span data-stu-id="82d1a-107">Method</span></span>       | <span data-ttu-id="82d1a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="82d1a-108">Return Type</span></span> | <span data-ttu-id="82d1a-109">说明</span><span class="sxs-lookup"><span data-stu-id="82d1a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="82d1a-110">获取 accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="82d1a-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="82d1a-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="82d1a-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="82d1a-112">检索 accessPackageAssignmentResourceRole 对象。</span><span class="sxs-lookup"><span data-stu-id="82d1a-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="82d1a-113">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="82d1a-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="82d1a-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="82d1a-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="82d1a-115">检索 accessPackageAssignmentResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="82d1a-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="82d1a-116">属性</span><span class="sxs-lookup"><span data-stu-id="82d1a-116">Properties</span></span>

| <span data-ttu-id="82d1a-117">属性</span><span class="sxs-lookup"><span data-stu-id="82d1a-117">Property</span></span>     | <span data-ttu-id="82d1a-118">类型</span><span class="sxs-lookup"><span data-stu-id="82d1a-118">Type</span></span>        | <span data-ttu-id="82d1a-119">说明</span><span class="sxs-lookup"><span data-stu-id="82d1a-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="82d1a-120">id</span><span class="sxs-lookup"><span data-stu-id="82d1a-120">id</span></span>|<span data-ttu-id="82d1a-121">String</span><span class="sxs-lookup"><span data-stu-id="82d1a-121">String</span></span>| <span data-ttu-id="82d1a-122">只读。</span><span class="sxs-lookup"><span data-stu-id="82d1a-122">Read-only.</span></span>|
|<span data-ttu-id="82d1a-123">originId</span><span class="sxs-lookup"><span data-stu-id="82d1a-123">originId</span></span>|<span data-ttu-id="82d1a-124">String</span><span class="sxs-lookup"><span data-stu-id="82d1a-124">String</span></span>|<span data-ttu-id="82d1a-125">相对于源系统的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="82d1a-125">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="82d1a-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="82d1a-126">originSystem</span></span>|<span data-ttu-id="82d1a-127">String</span><span class="sxs-lookup"><span data-stu-id="82d1a-127">String</span></span>|<span data-ttu-id="82d1a-128">要在其中创建角色分配或为访问包分配创建的系统，例如 `SharePointOnline` 。</span><span class="sxs-lookup"><span data-stu-id="82d1a-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`.</span></span>|
|<span data-ttu-id="82d1a-129">status</span><span class="sxs-lookup"><span data-stu-id="82d1a-129">status</span></span>|<span data-ttu-id="82d1a-130">String</span><span class="sxs-lookup"><span data-stu-id="82d1a-130">String</span></span>|<span data-ttu-id="82d1a-131">值是 `Fulfilled` 访问包分配已传递到原始系统。</span><span class="sxs-lookup"><span data-stu-id="82d1a-131">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82d1a-132">关系</span><span class="sxs-lookup"><span data-stu-id="82d1a-132">Relationships</span></span>

| <span data-ttu-id="82d1a-133">关系</span><span class="sxs-lookup"><span data-stu-id="82d1a-133">Relationship</span></span> | <span data-ttu-id="82d1a-134">类型</span><span class="sxs-lookup"><span data-stu-id="82d1a-134">Type</span></span>        | <span data-ttu-id="82d1a-135">Description</span><span class="sxs-lookup"><span data-stu-id="82d1a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="82d1a-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="82d1a-136">accessPackageAssignments</span></span>|<span data-ttu-id="82d1a-137">[accessPackageAssignment](accesspackageassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="82d1a-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="82d1a-138">此角色分配导致的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="82d1a-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="82d1a-139">只读。</span><span class="sxs-lookup"><span data-stu-id="82d1a-139">Read-only.</span></span> <span data-ttu-id="82d1a-140">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="82d1a-140">Nullable.</span></span>|
|<span data-ttu-id="82d1a-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="82d1a-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="82d1a-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="82d1a-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="82d1a-143">只读。</span><span class="sxs-lookup"><span data-stu-id="82d1a-143">Read-only.</span></span> <span data-ttu-id="82d1a-144">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="82d1a-144">Nullable.</span></span>|
|<span data-ttu-id="82d1a-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="82d1a-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="82d1a-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="82d1a-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="82d1a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="82d1a-147">Read-only.</span></span> <span data-ttu-id="82d1a-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="82d1a-148">Nullable.</span></span>|
|<span data-ttu-id="82d1a-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="82d1a-149">accessPackageSubject</span></span>|[<span data-ttu-id="82d1a-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="82d1a-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="82d1a-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="82d1a-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="82d1a-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82d1a-153">JSON representation</span></span>

<span data-ttu-id="82d1a-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82d1a-154">The following is a JSON representation of the resource.</span></span>

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
