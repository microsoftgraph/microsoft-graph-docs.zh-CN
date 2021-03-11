---
title: accessPackageResourceRoleScope 资源类型
description: 访问包资源角色作用域是一个对资源中的作用域和该资源中角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8fa3e0a20646f2acf72d26d31c20bac674e751cd
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720947"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="70e31-103">accessPackageResourceRoleScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="70e31-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="70e31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70e31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70e31-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源角色作用域是一个对资源中的作用域的引用，也是该资源中该范围的角色的引用。</span><span class="sxs-lookup"><span data-stu-id="70e31-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="70e31-106">访问包将具有其目录中与该访问包相关的资源的访问包资源角色作用域。</span><span class="sxs-lookup"><span data-stu-id="70e31-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="70e31-107">当主题收到访问包分配时，主题将在每个访问包资源角色作用域的该范围内使用角色进行预配。</span><span class="sxs-lookup"><span data-stu-id="70e31-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="70e31-108">方法</span><span class="sxs-lookup"><span data-stu-id="70e31-108">Methods</span></span>

| <span data-ttu-id="70e31-109">方法</span><span class="sxs-lookup"><span data-stu-id="70e31-109">Method</span></span>       | <span data-ttu-id="70e31-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="70e31-110">Return Type</span></span> | <span data-ttu-id="70e31-111">说明</span><span class="sxs-lookup"><span data-stu-id="70e31-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="70e31-112">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="70e31-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="70e31-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70e31-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="70e31-114">检索访问包 **的 accessPackageResourceRoleScope** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="70e31-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="70e31-115">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="70e31-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="70e31-116">为访问包 **创建新的 accessPackageResourceRoleScope** 对象。</span><span class="sxs-lookup"><span data-stu-id="70e31-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="70e31-117">属性</span><span class="sxs-lookup"><span data-stu-id="70e31-117">Properties</span></span>

| <span data-ttu-id="70e31-118">属性</span><span class="sxs-lookup"><span data-stu-id="70e31-118">Property</span></span>     | <span data-ttu-id="70e31-119">类型</span><span class="sxs-lookup"><span data-stu-id="70e31-119">Type</span></span>        | <span data-ttu-id="70e31-120">说明</span><span class="sxs-lookup"><span data-stu-id="70e31-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70e31-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="70e31-121">createdBy</span></span>|<span data-ttu-id="70e31-122">String</span><span class="sxs-lookup"><span data-stu-id="70e31-122">String</span></span>|<span data-ttu-id="70e31-123">只读。</span><span class="sxs-lookup"><span data-stu-id="70e31-123">Read-only.</span></span>|
|<span data-ttu-id="70e31-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70e31-124">createdDateTime</span></span>|<span data-ttu-id="70e31-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70e31-125">DateTimeOffset</span></span>|<span data-ttu-id="70e31-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="70e31-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="70e31-127">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="70e31-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="70e31-128">id</span><span class="sxs-lookup"><span data-stu-id="70e31-128">id</span></span>|<span data-ttu-id="70e31-129">String</span><span class="sxs-lookup"><span data-stu-id="70e31-129">String</span></span>| <span data-ttu-id="70e31-130">只读。</span><span class="sxs-lookup"><span data-stu-id="70e31-130">Read-only.</span></span>|
|<span data-ttu-id="70e31-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="70e31-131">modifiedBy</span></span>|<span data-ttu-id="70e31-132">String</span><span class="sxs-lookup"><span data-stu-id="70e31-132">String</span></span>|<span data-ttu-id="70e31-133">只读。</span><span class="sxs-lookup"><span data-stu-id="70e31-133">Read-only.</span></span>|
|<span data-ttu-id="70e31-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70e31-134">modifiedDateTime</span></span>|<span data-ttu-id="70e31-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70e31-135">DateTimeOffset</span></span>|<span data-ttu-id="70e31-136">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="70e31-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="70e31-137">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="70e31-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="70e31-138">关系</span><span class="sxs-lookup"><span data-stu-id="70e31-138">Relationships</span></span>

| <span data-ttu-id="70e31-139">关系</span><span class="sxs-lookup"><span data-stu-id="70e31-139">Relationship</span></span> | <span data-ttu-id="70e31-140">类型</span><span class="sxs-lookup"><span data-stu-id="70e31-140">Type</span></span>        | <span data-ttu-id="70e31-141">说明</span><span class="sxs-lookup"><span data-stu-id="70e31-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70e31-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="70e31-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="70e31-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="70e31-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="70e31-144">只读。</span><span class="sxs-lookup"><span data-stu-id="70e31-144">Read-only.</span></span> <span data-ttu-id="70e31-145">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="70e31-145">Nullable.</span></span>|
|<span data-ttu-id="70e31-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="70e31-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="70e31-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="70e31-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="70e31-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="70e31-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70e31-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70e31-150">JSON representation</span></span>

<span data-ttu-id="70e31-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70e31-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "keyProperty": "id"
}-->

```json
{
   "createdBy":"String",
   "createdDateTime":"String (timestamp)",
   "id":"String (identifier)",
   "modifiedBy":"String",
   "modifiedDateTime":"String (timestamp)",
   "accessPackageResourceRole":{
      "id":"String (identifier)",
      "displayName":"String",
      "originSystem":"String",
      "originId":"String"
   },
   "accessPackageResourceScope":{
      "id":"String (identifier)",
      "displayName":"String",
      "description":"String",
      "originId":"String (identifier)",
      "originSystem":"String"
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


