---
title: accessPackageResourceRoleScope 资源类型
description: 访问包资源角色作用域是对资源中的作用域和该资源中的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719f2ac275a19c9e4cef4cb2403166933e2e5925
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508504"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="22c58-103">accessPackageResourceRoleScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="22c58-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="22c58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22c58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22c58-105">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色作用域是对资源中的作用域的引用，以及该作用域在该资源中的角色。</span><span class="sxs-lookup"><span data-stu-id="22c58-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="22c58-106">访问包将具有与该访问包相关的目录中的资源的访问包资源角色作用域。</span><span class="sxs-lookup"><span data-stu-id="22c58-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="22c58-107">当主题收到访问包分配时，将使用每个访问包资源角色作用域的作用域中的角色设置该主题。</span><span class="sxs-lookup"><span data-stu-id="22c58-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="22c58-108">方法</span><span class="sxs-lookup"><span data-stu-id="22c58-108">Methods</span></span>

| <span data-ttu-id="22c58-109">方法</span><span class="sxs-lookup"><span data-stu-id="22c58-109">Method</span></span>       | <span data-ttu-id="22c58-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="22c58-110">Return Type</span></span> | <span data-ttu-id="22c58-111">说明</span><span class="sxs-lookup"><span data-stu-id="22c58-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="22c58-112">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="22c58-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="22c58-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="22c58-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="22c58-114">检索访问包的**accessPackageResourceRoleScope**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="22c58-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="22c58-115">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="22c58-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="22c58-116">为 access 包创建一个新的**accessPackageResourceRoleScope**对象。</span><span class="sxs-lookup"><span data-stu-id="22c58-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="22c58-117">属性</span><span class="sxs-lookup"><span data-stu-id="22c58-117">Properties</span></span>

| <span data-ttu-id="22c58-118">属性</span><span class="sxs-lookup"><span data-stu-id="22c58-118">Property</span></span>     | <span data-ttu-id="22c58-119">类型</span><span class="sxs-lookup"><span data-stu-id="22c58-119">Type</span></span>        | <span data-ttu-id="22c58-120">说明</span><span class="sxs-lookup"><span data-stu-id="22c58-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22c58-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="22c58-121">createdBy</span></span>|<span data-ttu-id="22c58-122">String</span><span class="sxs-lookup"><span data-stu-id="22c58-122">String</span></span>|<span data-ttu-id="22c58-123">只读。</span><span class="sxs-lookup"><span data-stu-id="22c58-123">Read-only.</span></span>|
|<span data-ttu-id="22c58-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22c58-124">createdDateTime</span></span>|<span data-ttu-id="22c58-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22c58-125">DateTimeOffset</span></span>|<span data-ttu-id="22c58-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="22c58-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="22c58-128">id</span><span class="sxs-lookup"><span data-stu-id="22c58-128">id</span></span>|<span data-ttu-id="22c58-129">String</span><span class="sxs-lookup"><span data-stu-id="22c58-129">String</span></span>| <span data-ttu-id="22c58-130">只读。</span><span class="sxs-lookup"><span data-stu-id="22c58-130">Read-only.</span></span>|
|<span data-ttu-id="22c58-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="22c58-131">modifiedBy</span></span>|<span data-ttu-id="22c58-132">String</span><span class="sxs-lookup"><span data-stu-id="22c58-132">String</span></span>|<span data-ttu-id="22c58-133">只读。</span><span class="sxs-lookup"><span data-stu-id="22c58-133">Read-only.</span></span>|
|<span data-ttu-id="22c58-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22c58-134">modifiedDateTime</span></span>|<span data-ttu-id="22c58-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22c58-135">DateTimeOffset</span></span>|<span data-ttu-id="22c58-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="22c58-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="22c58-138">关系</span><span class="sxs-lookup"><span data-stu-id="22c58-138">Relationships</span></span>

| <span data-ttu-id="22c58-139">关系</span><span class="sxs-lookup"><span data-stu-id="22c58-139">Relationship</span></span> | <span data-ttu-id="22c58-140">类型</span><span class="sxs-lookup"><span data-stu-id="22c58-140">Type</span></span>        | <span data-ttu-id="22c58-141">说明</span><span class="sxs-lookup"><span data-stu-id="22c58-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22c58-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="22c58-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="22c58-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="22c58-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="22c58-144">只读。</span><span class="sxs-lookup"><span data-stu-id="22c58-144">Read-only.</span></span> <span data-ttu-id="22c58-145">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="22c58-145">Nullable.</span></span>|
|<span data-ttu-id="22c58-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="22c58-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="22c58-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="22c58-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="22c58-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="22c58-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22c58-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22c58-150">JSON representation</span></span>

<span data-ttu-id="22c58-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22c58-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "accessPackageResourceRole": {
    "id": "String (identifier)",
     "displayName": "String",
     "originSystem": "String",
     "originId": "String"
  },
  "accessPackageResourceScope": {
     "id": "String (identifier)",
     "displayName": "String",
     "description": "String",
     "originId": "String (identifier)",
     "originSystem": "String"
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
