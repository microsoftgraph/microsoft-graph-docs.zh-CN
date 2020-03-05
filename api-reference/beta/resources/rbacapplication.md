---
title: rbacApplication 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3fd03ed6bb8f3e5e3548781c29d5d9fe16fcba23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521269"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="a2823-103">rbacApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2823-103">rbacApplication resource type</span></span>

<span data-ttu-id="a2823-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a2823-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2823-105">适用于 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。</span><span class="sxs-lookup"><span data-stu-id="a2823-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="a2823-106">当前 "目录" 是唯一受支持的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a2823-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="a2823-107">方法</span><span class="sxs-lookup"><span data-stu-id="a2823-107">Methods</span></span>

| <span data-ttu-id="a2823-108">方法</span><span class="sxs-lookup"><span data-stu-id="a2823-108">Method</span></span>       | <span data-ttu-id="a2823-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2823-109">Return Type</span></span> | <span data-ttu-id="a2823-110">说明</span><span class="sxs-lookup"><span data-stu-id="a2823-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a2823-111">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a2823-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="a2823-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a2823-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="a2823-113">通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="a2823-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="a2823-114">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="a2823-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="a2823-115">[unifiedRoleAssignment](unifiedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2823-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="a2823-116">获取 unifiedRoleAssignment 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2823-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="a2823-117">通过在 unifiedRoleDefitionId 或 principalId 上进行筛选，只能查询特定的实例。</span><span class="sxs-lookup"><span data-stu-id="a2823-117">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="a2823-118">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a2823-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="a2823-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a2823-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="a2823-120">通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="a2823-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="a2823-121">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="a2823-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="a2823-122">[unifiedRoleDefinition](unifiedroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2823-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="a2823-123">获取 unifiedRoleDefinition 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2823-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2823-124">属性</span><span class="sxs-lookup"><span data-stu-id="a2823-124">Properties</span></span>

<span data-ttu-id="a2823-125">无</span><span class="sxs-lookup"><span data-stu-id="a2823-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a2823-126">关系</span><span class="sxs-lookup"><span data-stu-id="a2823-126">Relationships</span></span>

<span data-ttu-id="a2823-127">无</span><span class="sxs-lookup"><span data-stu-id="a2823-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2823-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2823-128">JSON representation</span></span>

<span data-ttu-id="a2823-129">无</span><span class="sxs-lookup"><span data-stu-id="a2823-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
