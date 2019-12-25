---
title: accessPackageResourceRoleScope 资源类型
description: 访问包资源角色作用域是对资源中的作用域和该资源中的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ee4ec63c9c2efb60850ee7915e62dc0e284f8ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870958"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="ba577-103">accessPackageResourceRoleScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba577-103">accessPackageResourceRoleScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba577-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色作用域是对资源中的作用域的引用，以及该作用域在该资源中的角色。</span><span class="sxs-lookup"><span data-stu-id="ba577-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="ba577-105">访问包将具有与该访问包相关的目录中的资源的访问包资源角色作用域。</span><span class="sxs-lookup"><span data-stu-id="ba577-105">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="ba577-106">当主题收到访问包分配时，将使用每个访问包资源角色作用域的作用域中的角色设置该主题。</span><span class="sxs-lookup"><span data-stu-id="ba577-106">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="ba577-107">方法</span><span class="sxs-lookup"><span data-stu-id="ba577-107">Methods</span></span>

| <span data-ttu-id="ba577-108">方法</span><span class="sxs-lookup"><span data-stu-id="ba577-108">Method</span></span>       | <span data-ttu-id="ba577-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba577-109">Return Type</span></span> | <span data-ttu-id="ba577-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba577-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ba577-111">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="ba577-111">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="ba577-112">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合</span><span class="sxs-lookup"><span data-stu-id="ba577-112">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="ba577-113">检索访问包的**accessPackageResourceRoleScope**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ba577-113">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="ba577-114">创建 accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="ba577-114">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="ba577-115">为 access 包创建一个新的**accessPackageResourceRoleScope**对象。</span><span class="sxs-lookup"><span data-stu-id="ba577-115">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="ba577-116">属性</span><span class="sxs-lookup"><span data-stu-id="ba577-116">Properties</span></span>

| <span data-ttu-id="ba577-117">属性</span><span class="sxs-lookup"><span data-stu-id="ba577-117">Property</span></span>     | <span data-ttu-id="ba577-118">类型</span><span class="sxs-lookup"><span data-stu-id="ba577-118">Type</span></span>        | <span data-ttu-id="ba577-119">说明</span><span class="sxs-lookup"><span data-stu-id="ba577-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba577-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="ba577-120">createdBy</span></span>|<span data-ttu-id="ba577-121">String</span><span class="sxs-lookup"><span data-stu-id="ba577-121">String</span></span>|<span data-ttu-id="ba577-122">只读。</span><span class="sxs-lookup"><span data-stu-id="ba577-122">Read-only.</span></span>|
|<span data-ttu-id="ba577-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba577-123">createdDateTime</span></span>|<span data-ttu-id="ba577-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba577-124">DateTimeOffset</span></span>|<span data-ttu-id="ba577-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ba577-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ba577-127">id</span><span class="sxs-lookup"><span data-stu-id="ba577-127">id</span></span>|<span data-ttu-id="ba577-128">String</span><span class="sxs-lookup"><span data-stu-id="ba577-128">String</span></span>| <span data-ttu-id="ba577-129">只读。</span><span class="sxs-lookup"><span data-stu-id="ba577-129">Read-only.</span></span>|
|<span data-ttu-id="ba577-130">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="ba577-130">modifiedBy</span></span>|<span data-ttu-id="ba577-131">String</span><span class="sxs-lookup"><span data-stu-id="ba577-131">String</span></span>|<span data-ttu-id="ba577-132">只读。</span><span class="sxs-lookup"><span data-stu-id="ba577-132">Read-only.</span></span>|
|<span data-ttu-id="ba577-133">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba577-133">modifiedDateTime</span></span>|<span data-ttu-id="ba577-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba577-134">DateTimeOffset</span></span>|<span data-ttu-id="ba577-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ba577-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba577-137">关系</span><span class="sxs-lookup"><span data-stu-id="ba577-137">Relationships</span></span>

| <span data-ttu-id="ba577-138">关系</span><span class="sxs-lookup"><span data-stu-id="ba577-138">Relationship</span></span> | <span data-ttu-id="ba577-139">类型</span><span class="sxs-lookup"><span data-stu-id="ba577-139">Type</span></span>        | <span data-ttu-id="ba577-140">说明</span><span class="sxs-lookup"><span data-stu-id="ba577-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ba577-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="ba577-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="ba577-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="ba577-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="ba577-143">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="ba577-143">Read-only.</span></span> <span data-ttu-id="ba577-144">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ba577-144">Nullable.</span></span>|
|<span data-ttu-id="ba577-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="ba577-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="ba577-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="ba577-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="ba577-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="ba577-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba577-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba577-149">JSON representation</span></span>

<span data-ttu-id="ba577-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba577-150">The following is a JSON representation of the resource.</span></span>

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
