---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示使用者已通过访问包分配分配的特定于资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dbf73623ddd51cc1172e5610e84cc7861657489
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939192"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="4a2de-103">accessPackageAssignmentResourceRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a2de-103">accessPackageAssignmentResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a2de-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配资源角色指示已通过访问包分配分配的主题的特定于资源的角色。</span><span class="sxs-lookup"><span data-stu-id="4a2de-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="4a2de-105">方法</span><span class="sxs-lookup"><span data-stu-id="4a2de-105">Methods</span></span>

| <span data-ttu-id="4a2de-106">方法</span><span class="sxs-lookup"><span data-stu-id="4a2de-106">Method</span></span>       | <span data-ttu-id="4a2de-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a2de-107">Return Type</span></span> | <span data-ttu-id="4a2de-108">说明</span><span class="sxs-lookup"><span data-stu-id="4a2de-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4a2de-109">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="4a2de-109">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="4a2de-110">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a2de-110">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="4a2de-111">检索 accessPackageAssignmentResourceRole 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4a2de-111">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a2de-112">属性</span><span class="sxs-lookup"><span data-stu-id="4a2de-112">Properties</span></span>

| <span data-ttu-id="4a2de-113">属性</span><span class="sxs-lookup"><span data-stu-id="4a2de-113">Property</span></span>     | <span data-ttu-id="4a2de-114">类型</span><span class="sxs-lookup"><span data-stu-id="4a2de-114">Type</span></span>        | <span data-ttu-id="4a2de-115">说明</span><span class="sxs-lookup"><span data-stu-id="4a2de-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a2de-116">id</span><span class="sxs-lookup"><span data-stu-id="4a2de-116">id</span></span>|<span data-ttu-id="4a2de-117">字符串</span><span class="sxs-lookup"><span data-stu-id="4a2de-117">String</span></span>| <span data-ttu-id="4a2de-118">只读。</span><span class="sxs-lookup"><span data-stu-id="4a2de-118">Read-only.</span></span>|
|<span data-ttu-id="4a2de-119">originId</span><span class="sxs-lookup"><span data-stu-id="4a2de-119">originId</span></span>|<span data-ttu-id="4a2de-120">字符串</span><span class="sxs-lookup"><span data-stu-id="4a2de-120">String</span></span>|<span data-ttu-id="4a2de-121">相对于源系统的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4a2de-121">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="4a2de-122">originSystem</span><span class="sxs-lookup"><span data-stu-id="4a2de-122">originSystem</span></span>|<span data-ttu-id="4a2de-123">字符串</span><span class="sxs-lookup"><span data-stu-id="4a2de-123">String</span></span>|<span data-ttu-id="4a2de-124">要为访问包分配创建角色分配的系统。</span><span class="sxs-lookup"><span data-stu-id="4a2de-124">The system where the role assignment is to be created for an access package assignment.</span></span>|
|<span data-ttu-id="4a2de-125">状态</span><span class="sxs-lookup"><span data-stu-id="4a2de-125">status</span></span>|<span data-ttu-id="4a2de-126">字符串</span><span class="sxs-lookup"><span data-stu-id="4a2de-126">String</span></span>|<span data-ttu-id="4a2de-127">值是`Fulfilled`访问包分配已传递到原始系统。</span><span class="sxs-lookup"><span data-stu-id="4a2de-127">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a2de-128">关系</span><span class="sxs-lookup"><span data-stu-id="4a2de-128">Relationships</span></span>

| <span data-ttu-id="4a2de-129">关系</span><span class="sxs-lookup"><span data-stu-id="4a2de-129">Relationship</span></span> | <span data-ttu-id="4a2de-130">类型</span><span class="sxs-lookup"><span data-stu-id="4a2de-130">Type</span></span>        | <span data-ttu-id="4a2de-131">描述</span><span class="sxs-lookup"><span data-stu-id="4a2de-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a2de-132">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="4a2de-132">accessPackageAssignments</span></span>|<span data-ttu-id="4a2de-133">[accessPackageAssignment](accesspackageassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a2de-133">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="4a2de-134">此角色分配导致的访问包分配。</span><span class="sxs-lookup"><span data-stu-id="4a2de-134">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="4a2de-135">只读。</span><span class="sxs-lookup"><span data-stu-id="4a2de-135">Read-only.</span></span> <span data-ttu-id="4a2de-136">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4a2de-136">Nullable.</span></span>|
|<span data-ttu-id="4a2de-137">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="4a2de-137">accessPackageResourceRole</span></span>|[<span data-ttu-id="4a2de-138">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="4a2de-138">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="4a2de-139">只读。</span><span class="sxs-lookup"><span data-stu-id="4a2de-139">Read-only.</span></span> <span data-ttu-id="4a2de-140">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4a2de-140">Nullable.</span></span>|
|<span data-ttu-id="4a2de-141">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="4a2de-141">accessPackageResourceScope</span></span>|[<span data-ttu-id="4a2de-142">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="4a2de-142">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="4a2de-143">只读。</span><span class="sxs-lookup"><span data-stu-id="4a2de-143">Read-only.</span></span> <span data-ttu-id="4a2de-144">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4a2de-144">Nullable.</span></span>|
|<span data-ttu-id="4a2de-145">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="4a2de-145">accessPackageSubject</span></span>|[<span data-ttu-id="4a2de-146">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="4a2de-146">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="4a2de-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="4a2de-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4a2de-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a2de-149">JSON representation</span></span>

<span data-ttu-id="4a2de-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a2de-150">The following is a JSON representation of the resource.</span></span>

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
