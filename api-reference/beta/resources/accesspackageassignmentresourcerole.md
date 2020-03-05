---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示使用者已通过访问包分配分配的特定于资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eddff042af5b2cd724e87e3438f398e8d68c19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508539"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="ff39c-103">accessPackageAssignmentResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff39c-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="ff39c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ff39c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff39c-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配资源角色指示已通过访问包分配分配的主题的特定于资源的角色。</span><span class="sxs-lookup"><span data-stu-id="ff39c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="ff39c-106">方法</span><span class="sxs-lookup"><span data-stu-id="ff39c-106">Methods</span></span>

| <span data-ttu-id="ff39c-107">方法</span><span class="sxs-lookup"><span data-stu-id="ff39c-107">Method</span></span>       | <span data-ttu-id="ff39c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ff39c-108">Return Type</span></span> | <span data-ttu-id="ff39c-109">说明</span><span class="sxs-lookup"><span data-stu-id="ff39c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ff39c-110">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="ff39c-110">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="ff39c-111">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff39c-111">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="ff39c-112">检索 accessPackageAssignmentResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ff39c-112">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff39c-113">属性</span><span class="sxs-lookup"><span data-stu-id="ff39c-113">Properties</span></span>

| <span data-ttu-id="ff39c-114">属性</span><span class="sxs-lookup"><span data-stu-id="ff39c-114">Property</span></span>     | <span data-ttu-id="ff39c-115">类型</span><span class="sxs-lookup"><span data-stu-id="ff39c-115">Type</span></span>        | <span data-ttu-id="ff39c-116">说明</span><span class="sxs-lookup"><span data-stu-id="ff39c-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff39c-117">id</span><span class="sxs-lookup"><span data-stu-id="ff39c-117">id</span></span>|<span data-ttu-id="ff39c-118">String</span><span class="sxs-lookup"><span data-stu-id="ff39c-118">String</span></span>| <span data-ttu-id="ff39c-119">只读。</span><span class="sxs-lookup"><span data-stu-id="ff39c-119">Read-only.</span></span>|
|<span data-ttu-id="ff39c-120">originId</span><span class="sxs-lookup"><span data-stu-id="ff39c-120">originId</span></span>|<span data-ttu-id="ff39c-121">String</span><span class="sxs-lookup"><span data-stu-id="ff39c-121">String</span></span>|<span data-ttu-id="ff39c-122">相对于源系统的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ff39c-122">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="ff39c-123">originSystem</span><span class="sxs-lookup"><span data-stu-id="ff39c-123">originSystem</span></span>|<span data-ttu-id="ff39c-124">String</span><span class="sxs-lookup"><span data-stu-id="ff39c-124">String</span></span>|<span data-ttu-id="ff39c-125">要为访问包分配创建角色分配的系统。</span><span class="sxs-lookup"><span data-stu-id="ff39c-125">The system where the role assignment is to be created for an access package assignment.</span></span>|
|<span data-ttu-id="ff39c-126">status</span><span class="sxs-lookup"><span data-stu-id="ff39c-126">status</span></span>|<span data-ttu-id="ff39c-127">String</span><span class="sxs-lookup"><span data-stu-id="ff39c-127">String</span></span>|<span data-ttu-id="ff39c-128">值是`Fulfilled`访问包分配已传递到原始系统。</span><span class="sxs-lookup"><span data-stu-id="ff39c-128">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff39c-129">关系</span><span class="sxs-lookup"><span data-stu-id="ff39c-129">Relationships</span></span>

| <span data-ttu-id="ff39c-130">关系</span><span class="sxs-lookup"><span data-stu-id="ff39c-130">Relationship</span></span> | <span data-ttu-id="ff39c-131">类型</span><span class="sxs-lookup"><span data-stu-id="ff39c-131">Type</span></span>        | <span data-ttu-id="ff39c-132">说明</span><span class="sxs-lookup"><span data-stu-id="ff39c-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff39c-133">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="ff39c-133">accessPackageAssignments</span></span>|<span data-ttu-id="ff39c-134">[accessPackageAssignment](accesspackageassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="ff39c-134">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="ff39c-135">此角色分配导致的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="ff39c-135">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="ff39c-136">只读。</span><span class="sxs-lookup"><span data-stu-id="ff39c-136">Read-only.</span></span> <span data-ttu-id="ff39c-137">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ff39c-137">Nullable.</span></span>|
|<span data-ttu-id="ff39c-138">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="ff39c-138">accessPackageResourceRole</span></span>|[<span data-ttu-id="ff39c-139">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="ff39c-139">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="ff39c-140">只读。</span><span class="sxs-lookup"><span data-stu-id="ff39c-140">Read-only.</span></span> <span data-ttu-id="ff39c-141">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ff39c-141">Nullable.</span></span>|
|<span data-ttu-id="ff39c-142">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="ff39c-142">accessPackageResourceScope</span></span>|[<span data-ttu-id="ff39c-143">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="ff39c-143">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="ff39c-144">只读。</span><span class="sxs-lookup"><span data-stu-id="ff39c-144">Read-only.</span></span> <span data-ttu-id="ff39c-145">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ff39c-145">Nullable.</span></span>|
|<span data-ttu-id="ff39c-146">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ff39c-146">accessPackageSubject</span></span>|[<span data-ttu-id="ff39c-147">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="ff39c-147">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ff39c-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="ff39c-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ff39c-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff39c-150">JSON representation</span></span>

<span data-ttu-id="ff39c-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff39c-151">The following is a JSON representation of the resource.</span></span>

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
