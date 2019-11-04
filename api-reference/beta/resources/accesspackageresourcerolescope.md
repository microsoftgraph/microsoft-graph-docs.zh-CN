---
title: accessPackageResourceRoleScope 资源类型
description: 访问包资源角色作用域是对资源中的作用域和该资源中的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4f10d297e59f9665d493060362a27e1c4b11a5a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938910"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="7cc31-103">accessPackageResourceRoleScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="7cc31-103">accessPackageResourceRoleScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cc31-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色作用域是对资源中的作用域和该资源中的角色的引用。</span><span class="sxs-lookup"><span data-stu-id="7cc31-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource.</span></span>

## <a name="properties"></a><span data-ttu-id="7cc31-105">属性</span><span class="sxs-lookup"><span data-stu-id="7cc31-105">Properties</span></span>

| <span data-ttu-id="7cc31-106">属性</span><span class="sxs-lookup"><span data-stu-id="7cc31-106">Property</span></span>     | <span data-ttu-id="7cc31-107">类型</span><span class="sxs-lookup"><span data-stu-id="7cc31-107">Type</span></span>        | <span data-ttu-id="7cc31-108">说明</span><span class="sxs-lookup"><span data-stu-id="7cc31-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7cc31-109">createdBy</span><span class="sxs-lookup"><span data-stu-id="7cc31-109">createdBy</span></span>|<span data-ttu-id="7cc31-110">字符串</span><span class="sxs-lookup"><span data-stu-id="7cc31-110">String</span></span>|<span data-ttu-id="7cc31-111">只读。</span><span class="sxs-lookup"><span data-stu-id="7cc31-111">Read-only.</span></span>|
|<span data-ttu-id="7cc31-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cc31-112">createdDateTime</span></span>|<span data-ttu-id="7cc31-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cc31-113">DateTimeOffset</span></span>|<span data-ttu-id="7cc31-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7cc31-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7cc31-116">id</span><span class="sxs-lookup"><span data-stu-id="7cc31-116">id</span></span>|<span data-ttu-id="7cc31-117">字符串</span><span class="sxs-lookup"><span data-stu-id="7cc31-117">String</span></span>| <span data-ttu-id="7cc31-118">只读。</span><span class="sxs-lookup"><span data-stu-id="7cc31-118">Read-only.</span></span>|
|<span data-ttu-id="7cc31-119">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="7cc31-119">modifiedBy</span></span>|<span data-ttu-id="7cc31-120">字符串</span><span class="sxs-lookup"><span data-stu-id="7cc31-120">String</span></span>|<span data-ttu-id="7cc31-121">只读。</span><span class="sxs-lookup"><span data-stu-id="7cc31-121">Read-only.</span></span>|
|<span data-ttu-id="7cc31-122">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cc31-122">modifiedDateTime</span></span>|<span data-ttu-id="7cc31-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cc31-123">DateTimeOffset</span></span>|<span data-ttu-id="7cc31-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7cc31-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cc31-126">关系</span><span class="sxs-lookup"><span data-stu-id="7cc31-126">Relationships</span></span>

| <span data-ttu-id="7cc31-127">关系</span><span class="sxs-lookup"><span data-stu-id="7cc31-127">Relationship</span></span> | <span data-ttu-id="7cc31-128">类型</span><span class="sxs-lookup"><span data-stu-id="7cc31-128">Type</span></span>        | <span data-ttu-id="7cc31-129">描述</span><span class="sxs-lookup"><span data-stu-id="7cc31-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7cc31-130">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="7cc31-130">accessPackageResourceRole</span></span>|[<span data-ttu-id="7cc31-131">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="7cc31-131">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="7cc31-132">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="7cc31-132">Read-only.</span></span> <span data-ttu-id="7cc31-133">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7cc31-133">Nullable.</span></span>|
|<span data-ttu-id="7cc31-134">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="7cc31-134">accessPackageResourceScope</span></span>|[<span data-ttu-id="7cc31-135">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="7cc31-135">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="7cc31-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="7cc31-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cc31-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7cc31-138">JSON representation</span></span>

<span data-ttu-id="7cc31-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cc31-139">The following is a JSON representation of the resource.</span></span>

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
  "modifiedDateTime": "String (timestamp)"
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
