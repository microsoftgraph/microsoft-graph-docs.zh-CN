---
title: appScope 资源类型
description: '角色分配的范围决定了主体已被授予访问权限的资源集。 应用程序范围是由特定应用程序定义和理解的范围。 另一种类型的作用域是目录作用域。 目录作用域是存储在多个应用程序可理解的目录中的共享作用域。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a996b219df124ac0c287ed4ed32658584acb6ac
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160380"
---
# <a name="appscope-resource-type"></a><span data-ttu-id="7e234-106">appScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e234-106">appScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e234-107">角色分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="7e234-107">The scope of a role assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="7e234-108">应用程序范围是由特定应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="7e234-108">An app scope is a scope defined and understood by a specific application.</span></span> <span data-ttu-id="7e234-109">另一种类型的作用域是目录作用域。</span><span class="sxs-lookup"><span data-stu-id="7e234-109">The other type of scope is directory scope.</span></span> <span data-ttu-id="7e234-110">目录作用域是存储在多个应用程序可理解的目录中的共享作用域。</span><span class="sxs-lookup"><span data-stu-id="7e234-110">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> 

<span data-ttu-id="7e234-111">这在单个主体、单作用域实体和多个主体中均采用了多个作用域实体。</span><span class="sxs-lookup"><span data-stu-id="7e234-111">This is employed in both the single principal, single scope entity and multiple principal, multiple scope entities.</span></span>

## <a name="methods"></a><span data-ttu-id="7e234-112">方法</span><span class="sxs-lookup"><span data-stu-id="7e234-112">Methods</span></span>
<span data-ttu-id="7e234-113">无</span><span class="sxs-lookup"><span data-stu-id="7e234-113">None</span></span>

## <a name="properties"></a><span data-ttu-id="7e234-114">属性</span><span class="sxs-lookup"><span data-stu-id="7e234-114">Properties</span></span>

| <span data-ttu-id="7e234-115">属性</span><span class="sxs-lookup"><span data-stu-id="7e234-115">Property</span></span> | <span data-ttu-id="7e234-116">类型</span><span class="sxs-lookup"><span data-stu-id="7e234-116">Type</span></span> | <span data-ttu-id="7e234-117">说明</span><span class="sxs-lookup"><span data-stu-id="7e234-117">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="7e234-118">id</span><span class="sxs-lookup"><span data-stu-id="7e234-118">id</span></span> | <span data-ttu-id="7e234-119">string</span><span class="sxs-lookup"><span data-stu-id="7e234-119">string</span></span> | <span data-ttu-id="7e234-120">表示工作分配范围的特定于应用程序的容器或资源的 Id。</span><span class="sxs-lookup"><span data-stu-id="7e234-120">Id of an app-specific container or resource representing the scope of the assignment.</span></span> <span data-ttu-id="7e234-121">通常是资源的不可变 id。</span><span class="sxs-lookup"><span data-stu-id="7e234-121">Usually the immutable id of the resource.</span></span> <span data-ttu-id="7e234-122">工作分配的范围决定了主体已被授予访问权限的一组资源。</span><span class="sxs-lookup"><span data-stu-id="7e234-122">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="7e234-123">此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="7e234-123">This property is required.</span></span> |
| <span data-ttu-id="7e234-124">type</span><span class="sxs-lookup"><span data-stu-id="7e234-124">type</span></span> | <span data-ttu-id="7e234-125">String</span><span class="sxs-lookup"><span data-stu-id="7e234-125">String</span></span> | <span data-ttu-id="7e234-126">描述应用程序范围所表示的应用程序特定资源的类型。</span><span class="sxs-lookup"><span data-stu-id="7e234-126">Describes the type of app-specific resource represented by the app scope.</span></span> <span data-ttu-id="7e234-127">出于显示目的而提供，因此用户界面可以向用户传达应用程序范围所表示的应用程序特定资源的类型。</span><span class="sxs-lookup"><span data-stu-id="7e234-127">Provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.</span></span> <span data-ttu-id="7e234-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7e234-128">This property is read only.</span></span> |
| <span data-ttu-id="7e234-129">displayName</span><span class="sxs-lookup"><span data-stu-id="7e234-129">displayName</span></span> | <span data-ttu-id="7e234-130">string</span><span class="sxs-lookup"><span data-stu-id="7e234-130">string</span></span> | <span data-ttu-id="7e234-131">提供应用程序范围所表示的应用程序特定资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7e234-131">Provides the display name of the app-specific resource represented by the app scope.</span></span> <span data-ttu-id="7e234-132">出于显示目的而提供，因为 appScopeId 通常是不可变且不可读的可读 id。此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7e234-132">Provided for display purposes since appScopeId is often an immutable, non-human-readable id. This property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7e234-133">关系</span><span class="sxs-lookup"><span data-stu-id="7e234-133">Relationships</span></span>

<span data-ttu-id="7e234-134">无</span><span class="sxs-lookup"><span data-stu-id="7e234-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e234-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e234-135">JSON representation</span></span>

<span data-ttu-id="7e234-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e234-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appScope"
}-->

```json
{
  "id": "String (identifier)",
  "type": "String",
  "displayName": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->