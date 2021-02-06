---
title: appScope 资源类型
description: 应用范围是由特定应用程序定义和理解的范围。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: de49425bddc5905d1b1bf17afeb5fb7c5363038c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136008"
---
# <a name="appscope-resource-type"></a><span data-ttu-id="a35c5-103">appScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="a35c5-103">appScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a35c5-104">作用域角色分配确定主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="a35c5-104">The scope of a role assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="a35c5-105">应用范围是由特定应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="a35c5-105">An app scope is a scope defined and understood by a specific application.</span></span> <span data-ttu-id="a35c5-106">另一种类型的作用域是目录范围。</span><span class="sxs-lookup"><span data-stu-id="a35c5-106">The other type of scope is directory scope.</span></span> <span data-ttu-id="a35c5-107">目录范围是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="a35c5-107">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> 

<span data-ttu-id="a35c5-108">这同时在单个主体、单个范围实体和多个主体、多个范围实体中采用。</span><span class="sxs-lookup"><span data-stu-id="a35c5-108">This is employed in both the single principal, single scope entity and multiple principal, multiple scope entities.</span></span>

## <a name="methods"></a><span data-ttu-id="a35c5-109">方法</span><span class="sxs-lookup"><span data-stu-id="a35c5-109">Methods</span></span>
<span data-ttu-id="a35c5-110">无</span><span class="sxs-lookup"><span data-stu-id="a35c5-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="a35c5-111">属性</span><span class="sxs-lookup"><span data-stu-id="a35c5-111">Properties</span></span>

| <span data-ttu-id="a35c5-112">属性</span><span class="sxs-lookup"><span data-stu-id="a35c5-112">Property</span></span> | <span data-ttu-id="a35c5-113">类型</span><span class="sxs-lookup"><span data-stu-id="a35c5-113">Type</span></span> | <span data-ttu-id="a35c5-114">说明</span><span class="sxs-lookup"><span data-stu-id="a35c5-114">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="a35c5-115">id</span><span class="sxs-lookup"><span data-stu-id="a35c5-115">id</span></span> | <span data-ttu-id="a35c5-116">string</span><span class="sxs-lookup"><span data-stu-id="a35c5-116">string</span></span> | <span data-ttu-id="a35c5-117">表示分配范围的特定于应用的容器或资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="a35c5-117">Id of an app-specific container or resource representing the scope of the assignment.</span></span> <span data-ttu-id="a35c5-118">通常是资源的不可变 ID。</span><span class="sxs-lookup"><span data-stu-id="a35c5-118">Usually the immutable id of the resource.</span></span> <span data-ttu-id="a35c5-119">工作分配的范围决定了主体已被授予访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="a35c5-119">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="a35c5-120">此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="a35c5-120">This property is required.</span></span> |
| <span data-ttu-id="a35c5-121">type</span><span class="sxs-lookup"><span data-stu-id="a35c5-121">type</span></span> | <span data-ttu-id="a35c5-122">字符串</span><span class="sxs-lookup"><span data-stu-id="a35c5-122">String</span></span> | <span data-ttu-id="a35c5-123">描述应用范围所代表的特定于应用的资源的类型。</span><span class="sxs-lookup"><span data-stu-id="a35c5-123">Describes the type of app-specific resource represented by the app scope.</span></span> <span data-ttu-id="a35c5-124">提供用于显示目的，以便用户界面可以向用户传达应用范围表示的应用特定资源类型。</span><span class="sxs-lookup"><span data-stu-id="a35c5-124">Provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.</span></span> <span data-ttu-id="a35c5-125">此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="a35c5-125">This property is read only.</span></span> |
| <span data-ttu-id="a35c5-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a35c5-126">displayName</span></span> | <span data-ttu-id="a35c5-127">string</span><span class="sxs-lookup"><span data-stu-id="a35c5-127">string</span></span> | <span data-ttu-id="a35c5-128">提供显示名称范围表示的特定于应用的资源的源。</span><span class="sxs-lookup"><span data-stu-id="a35c5-128">Provides the display name of the app-specific resource represented by the app scope.</span></span> <span data-ttu-id="a35c5-129">提供用于显示目的，因为 appScopeId 通常是不可变的不可读 ID。此属性为只读。</span><span class="sxs-lookup"><span data-stu-id="a35c5-129">Provided for display purposes since appScopeId is often an immutable, non-human-readable id. This property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a35c5-130">关系</span><span class="sxs-lookup"><span data-stu-id="a35c5-130">Relationships</span></span>

<span data-ttu-id="a35c5-131">无</span><span class="sxs-lookup"><span data-stu-id="a35c5-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a35c5-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a35c5-132">JSON representation</span></span>

<span data-ttu-id="a35c5-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a35c5-133">The following is a JSON representation of the resource.</span></span>

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

